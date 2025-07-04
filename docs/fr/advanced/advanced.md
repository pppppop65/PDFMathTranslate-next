[**Options avancées**](./introduction.md) > **Options avancées** _(current)_

---

<h3 id="toc">Table des matières</h3>

- [Arguments de ligne de commande](#arguments-de-ligne-de-commande)
- [Traduction partielle](#traduction-partielle)
- [Spécifier les langues source et cible](#spécifier-les-langues-source-et-cible)
- [Traduire avec exceptions](#traduire-avec-exceptions)
- [Invite personnalisé](#invite-personnalisé)
- [Configuration personnalisée](#configuration-personnalisée)
- [Ignorer le nettoyage](#ignorer-le-nettoyage)
- [Cache de traduction](#cache-de-traduction)
- [Déploiement en tant que services publics](#déploiement-en-tant-que-services-publics)
- [Authentification et page d'accueil](#authentification-et-page-daccueil)
- [Support du glossaire](#support-du-glossaire)

---

#### Arguments de ligne de commande

Exécutez la commande de traduction dans la ligne de commande pour générer le document traduit `example-mono.pdf` et le document bilingue `example-dual.pdf` dans le répertoire de travail actuel. Utilisez Google comme service de traduction par défaut. Plus de services de traduction supportés peuvent être trouvés [ICI](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/docs/ADVANCED.md#services).

<img src="./../images/cmd_light.svg" width="580px"  alt="cmd"/>

Dans le tableau suivant, nous listons toutes les options avancées pour référence :

##### Arguments

| Option                          | Fonction                                                                               | Exemple                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `files`                         | Chemin local du fichier PDF                                                           | `pdf2zh ~/local.pdf`                                                                                                 |
| `links`                         | Fichiers en ligne                                                                           | `pdf2zh http://arxiv.org/paper.pdf`                                                                                  |
| `--output`                      | Répertoire de sortie pour les fichiers                                                | `pdf2zh example.pdf --output /outputpath`                                                                            |
| `--<Services>`                  | Utiliser un [**service spécifique**](./Documentation-des-services-de-traduction.md) pour la traduction | `pdf2zh example.pdf --openai`<br>`pdf2zh example.pdf --deepseek`                                                     |
| `--help`, `-h`                  | Afficher le message d'aide et quitter                                                  | `pdf2zh -h`                                                                                                          |
| `--config-file`                 | Chemin vers le fichier de configuration                                                         | `pdf2zh --config-file /path/to/config/config.toml`                                                                   |
| `--report-interval`             | Intervalle de rapport de progression en secondes                                                    | `pdf2zh example.pdf --report-interval 5`                                                                             |
| `--debug`                       | Utiliser le niveau de journalisation de débogage                                                                | `pdf2zh example.pdf --debug`                                                                                         |
| `--gui`                         | Interagir avec l'interface graphique                                                   | `pdf2zh --gui`                                                                                                       |
| `--warmup`                      | Télécharge et vérifie uniquement les ressources nécessaires puis quitte               | `pdf2zh example.pdf --warmup`                                                                                        |
| `--generate-offline-assets`     | Générer un package d'assets hors ligne dans le répertoire spécifié                     | `pdf2zh example.pdf --generate-offline-assets /path`                                                                 |
| `--restore-offline-assets`      | Restaurer le package d'assets hors ligne depuis le répertoire spécifié                 | `pdf2zh example.pdf --restore-offline-assets /chemin`                                                                  |
| `--version`                     | Afficher la version puis quitter                                                                 | `pdf2zh --version`                                                                                                   |
| `--pages`                       | Traduction partielle du document                                                      | `pdf2zh example.pdf --pages 1,2,1-,-3,3-5`                                                                           |
| `--lang-in`                     | Le code de la langue source                                                            | `pdf2zh example.pdf --lang-in en`                                                                                    |
| `--lang-out`                    | Le code de la langue cible                                                            | `pdf2zh example.pdf --lang-out zh-CN`                                                                                |
| `--min-text-length`             | Longueur minimale du texte à traduire                                                  | `pdf2zh example.pdf --min-text-length 5`                                                                             |
| `--rpc-doclayout`               | Adresse hôte du service RPC pour l'analyse de la mise en page des documents            |                                                                                                                      |
| `--qps`                         | Limite de QPS pour le service de traduction                                            | `pdf2zh example.pdf --qps 200`                                                                                       |
| `--ignore-cache`                | Ignorer le cache de traduction                                                         | `pdf2zh example.pdf --ignore-cache`                                                                                  |
| `--custom-system-prompt`        | Invite système personnalisée pour la traduction. Utilisée pour `/no_think` dans Qwen 3                   | `pdf2zh example.pdf --custom-system-prompt "/no_think You are a professional, authentic machine translation engine"` |
| `--pool-max-worker`             | Nombre maximum de travailleurs pour le pool de traduction. Si non défini, utilisera le qps comme nombre de travailleurs | `pdf2zh example.pdf --pool-max-worker 100`                                                                |
| `--no-auto-extract-glossary`    | Désactiver l'extraction automatique du glossaire                                                          | `pdf2zh example.pdf --no-auto-extract-glossary`                                                                      |
| `--primary-font-family`         | Remplace la famille de police principale pour le texte traduit. Choix : 'serif' pour les polices serif, 'sans-serif' pour les polices sans-serif, 'script' pour les polices script/italiques. Si non spécifié, utilise une sélection automatique de police basée sur les propriétés du texte original. | `pdf2zh example.pdf --primary-font-family serif` |
| `--no-dual`                     | Ne pas générer de fichiers PDF bilingues                                               | `pdf2zh example.pdf --no-dual`                                                                                       |
| `--no-mono`                     | Ne pas générer de fichiers PDF monolingues                                             | `pdf2zh example.pdf --no-mono`                                                                                       |
| `--formular-font-pattern`       | Modèle de police pour identifier le texte des formules                                                  | `pdf2zh example.pdf --formular-font-pattern "(MS.*)"`                                                                |
| `--formular-char-pattern`       | Modèle de caractères pour identifier le texte des formules                                             | `pdf2zh example.pdf --formular-char-pattern "(MS.*)"`                                                                |
| `--split-short-line`            | Forcer la séparation des lignes courtes en paragraphes distincts                      | `pdf2zh example.pdf --split-short-line`                                                                              |
| `--short-line-split-factor`     | Facteur de seuil de division pour les lignes courtes                                                 |                                                                                                                      |
| `--skip-clean`                  | Ignorer l'étape de nettoyage du PDF                                                   | `pdf2zh example.pdf --skip-clean`                                                                                    |
| `--dual-translate-first`        | Dans le mode PDF double, prioriser le placement de la page traduite                                          | `pdf2zh example.pdf --dual-translate-first`                                                                                            |
| `--disable-rich-text-translate` | Désactiver la traduction de texte enrichi                                                          | `pdf2zh example.pdf --disable-rich-text-translate`                                                                   |
| `--enhance-compatibility`       | Activer toutes les options d'amélioration de la compatibilité                         | `pdf2zh example.pdf --enhance-compatibility`                                                                         |
| `--use-alternating-pages-dual`  | Utiliser le mode pages alternées pour les PDF doubles                                                | `pdf2zh example.pdf --use-alternating-pages-dual`                                                                    |
| `--watermark-output-mode`       | Mode de filigrane pour les fichiers PDF                                                | `pdf2zh example.pdf --watermark-output-mode "NoWaterMark"`                                                           |
| `--max-pages-per-part`          | Nombre maximum de pages par partie pour une traduction divisée                                           | `pdf2zh example.pdf --max-pages-per-part 1`                                                                          |
| `--translate-table-text`        | Traduire le texte des tableaux (expérimental)                                                    | `pdf2zh example.pdf --translate-table-text`                                                                          |
| `--skip-scanned-detection`      | Ignorer la détection de documents scannés                                               | `pdf2zh example.pdf --skip-scanned-detection`                                                                        |
| `--ocr-workaround`              | Forcer le texte traduit à être noir et ajouter un fond blanc                             | `pdf2zh example.pdf --ocr-workaround`                                                                                |
| `--auto-enable-ocr-workaround`  | Active la solution de contournement OCR automatique. Si un document est détecté comme étant fortement scanné, cela tentera d'activer le traitement OCR et ignorera toute détection de scan supplémentaire. Voir la documentation pour plus de détails. (par défaut : False) | `pdf2zh example.pdf --auto-enable-ocr-workaround True`                    |
| `--only-include-translated-page`| N'inclure que les pages traduites dans le PDF de sortie. Efficace uniquement lorsque --pages est utilisé. | `pdf2zh example.pdf --pages 1-5 --only-include-translated-page`                                                       |
| `--glossaries`                  | Glossaire personnalisé pour la traduction.                                                      | `pdf2zh example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"`                                         |
| `--save-auto-extracted-glossary`| enregistrer le glossaire extrait automatiquement.                                                | `pdf2zh example.pdf --save-auto-extracted-glossary`                                                                   |


##### Arguments de l'interface graphique

| Option                          | Fonction                               | Exemple                                         |
| ------------------------------- | -------------------------------------- | ----------------------------------------------- |
| `--share`                       | Activer le mode partage                | `pdf2zh --gui --share`                          |
| `--auth-file`                   | Chemin vers le fichier d'authentification        | `pdf2zh --gui --auth-file /path`                |
| `--welcome-page`                | Chemin vers le fichier html de bienvenue | `pdf2zh --gui --welcome-page /path`             |
| `--enabled-services`            | Services de traduction activés           | `pdf2zh --gui --enabled-services "Bing,OpenAI"` |
| `--disable-gui-sensitive-input` | Désactiver l'entrée sensible de l'interface graphique            | `pdf2zh --gui --disable-gui-sensitive-input`    |
| `--disable-config-auto-save`    | Désactiver l'enregistrement automatique de la configuration | `pdf2zh --gui --disable-config-auto-save`       |
| `--server-port`                 | Port de l'interface web               | `pdf2zh --gui --server-port 7860`               |

[⬆️ Retour en haut](#toc)

---

#### Traduction partielle

Utilisez le paramètre `--pages` pour traduire une partie d'un document.

- Si les numéros de page sont consécutifs, vous pouvez l'écrire comme ceci :

```bash
pdf2zh_next example.pdf --pages 1-3
```

```bash
pdf2zh_next example.pdf --pages 25-
```

> [!TIP]
> `25-` inclut toutes les pages après la page 25. Si votre document comporte 100 pages, cela équivaut à `25-100`.
> 
> De même, `-25` inclut toutes les pages avant la page 25, ce qui équivaut à `1-25`.

- Si les pages ne sont pas consécutives, vous pouvez utiliser une virgule `,` pour les séparer.

Par exemple, si vous souhaitez traduire la première et la troisième page, vous pouvez utiliser la commande suivante :

```bash
pdf2zh_next example.pdf --pages "1,3"
```

- Si les pages incluent à la fois des plages consécutives et non consécutives, vous pouvez également les connecter avec une virgule, comme ceci :

```bash
pdf2zh_next example.pdf --pages "1,3,10-20,25-"
```

Cette commande traduira la première page, la troisième page, les pages 10 à 20, et toutes les pages de 25 jusqu'à la fin.


[⬆️ Retour en haut](#toc)

---

#### Spécifier les langues source et cible

Voir [Codes de langue Google](https://developers.google.com/admin-sdk/directory/v1/languages), [Codes de langue DeepL](https://developers.deepl.com/docs/resources/supported-languages)

```bash
pdf2zh_next example.pdf --lang-in en -lang-out ja
```

[⬆️ Retour en haut](#toc)

---

#### Traduire avec exceptions

Utiliser des expressions régulières pour spécifier les polices de formule et les caractères à préserver :

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^RT].*|MS.*|.*Ital)" --formular-char-pattern "(\(|\||\)|\+|=|\d|[\u0080-\ufaff])"
```

Préserver par défaut les polices `Latex`, `Mono`, `Code`, `Italic`, `Symbol` et `Math` :

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^R]|MS.M|XY|MT|BL|RM|EU|LA|RS|LINE|LCIRCLE|TeX-|rsfs|txsy|wasy|stmary|.*Mono|.*Code|.*Ital|.*Sym|.*Math)"
```

[⬆️ Retour en haut](#toc)

---

#### Invite personnalisé

<!-- Note: System prompt is currently not supported. See [this change](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pull/637). -->

Invite système personnalisée pour la traduction. Elle est principalement utilisée pour ajouter l'instruction '/no_think' de Qwen 3 dans l'invite.

```bash
pdf2zh_next example.pdf --custom-system-prompt "/no_think You are a professional and reliable machine translation engine responsible for translating the input text into zh_CN.When translating, strictly follow the instructions below to ensure translation quality and preserve all formatting, tags, and placeholders:"
```

[⬆️ Retour en haut](#toc)

---

#### Configuration personnalisée

Il existe plusieurs façons de modifier et d'importer le fichier de configuration.

> [!NOTE]
> **Hiérarchie des fichiers de configuration**
>
> Lors de la modification d'un même paramètre à l'aide de différentes méthodes, le logiciel appliquera les modifications selon l'ordre de priorité ci-dessous.
>
> Les modifications de rang supérieur remplaceront celles de rang inférieur.
>
> **cli/gui > env > fichier de configuration utilisateur > fichier de configuration par défaut**

- Modification de la configuration via **Arguments de ligne de commande**

Pour la plupart des cas, vous pouvez directement passer vos paramètres souhaités via les arguments de ligne de commande. Veuillez vous référer à [Arguments de ligne de commande](#arguments-de-ligne-de-commande) pour plus d'informations.

Par exemple, si vous souhaitez activer une fenêtre d'interface graphique, vous pouvez utiliser la commande suivante :

```bash
pdf2zh_next --gui
```

- Modification de la configuration via **Variables d'environnement**

Vous pouvez remplacer le `--` dans les arguments de ligne de commande par `PDF2ZH_`, connecter les paramètres en utilisant `=`, et remplacer `-` par `_` comme variables d'environnement.

Par exemple, si vous souhaitez activer une fenêtre d'interface graphique, vous pouvez utiliser la commande suivante :

```bash
PDF2ZH_GUI=TRUE pdf2zh_next
```

<img src="./../images/ev_light.svg" width="580px"  alt="env"/>

- Fichier de **configuration** spécifié par l'utilisateur

Vous pouvez spécifier un fichier de configuration en utilisant l'argument de ligne de commande ci-dessous :

```bash
pdf2zh_next --config-file '/path/config.toml'
```

Si vous n'êtes pas sûr du format du fichier de configuration, veuillez vous référer au fichier de configuration par défaut décrit ci-dessous.

- **Fichier de configuration par défaut**

Le fichier de configuration par défaut se trouve dans `~/.config/pdf2zh`. 
Veuillez ne pas modifier les fichiers de configuration dans le répertoire `default`. 
Il est fortement recommandé de se référer au contenu de ce fichier de configuration et d'utiliser **Configuration personnalisée** pour implémenter votre propre fichier de configuration.

> [!TIP]
> - Par défaut, pdf2zh 2.0 enregistre automatiquement la configuration actuelle dans `~/.config/pdf2zh/config.v3.toml` chaque fois que vous cliquez sur le bouton de traduction dans l'interface graphique. Ce fichier de configuration sera chargé par défaut au prochain démarrage.
> - Les fichiers de configuration dans le répertoire `default` sont générés automatiquement par le programme. Vous pouvez les copier pour les modifier, mais veuillez ne pas les modifier directement.
> - Les fichiers de configuration peuvent inclure des numéros de version tels que "v2", "v3", etc. Ce sont **des numéros de version des fichiers de configuration**, **et non** le numéro de version de pdf2zh lui-même.


[⬆️ Retour en haut](#toc)

---

#### Ignorer le nettoyage

Lorsque ce paramètre est défini sur True, l'étape de nettoyage du PDF sera ignorée, ce qui peut améliorer la compatibilité et éviter certains problèmes de traitement des polices.

Utilisation :

```bash
pdf2zh_next example.pdf --skip-clean
```

Ou en utilisant des variables d'environnement :

```bash
PDF2ZH_SKIP_CLEAN=TRUE pdf2zh_next example.pdf
```

> [!TIP]
> Lorsque `--enhance-compatibility` est activé, Ignorer le nettoyage est automatiquement activé.

---

#### Cache de traduction

PDFMathTranslate met en cache les textes traduits pour augmenter la vitesse et éviter les appels API inutiles pour les mêmes contenus. Vous pouvez utiliser l'option `--ignore-cache` pour ignorer le cache de traduction et forcer une nouvelle traduction.

```bash
pdf2zh_next example.pdf --ignore-cache
```

[⬆️ Retour en haut](#toc)

---

#### Déploiement en tant que services publics

Lors du déploiement d'une interface graphique pdf2zh sur des services publics, vous devez modifier le fichier de configuration comme décrit ci-dessous.

> [!TIP]
> - Lors d'un déploiement public, `disable_gui_sensitive_input` et `disable_config_auto_save` doivent tous deux être activés.
> - Séparez les différents services disponibles avec des *virgules anglaises* <kbd>,</kbd> .

Une configuration utilisable est la suivante :

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
enabled_services = "Bing,OpenAI"
disable_gui_sensitive_input = true
disable_config_auto_save = true
```

[⬆️ Retour en haut](#toc)

---

#### Authentification et page d'accueil

Lors de l'utilisation de Authentification et page d'accueil pour spécifier quel utilisateur doit utiliser l'interface Web et personnaliser la page de connexion :

exemple auth.txt
Chaque ligne contient deux éléments, nom d'utilisateur et mot de passe, séparés par une virgule.

```
admin,123456
user1,password1
user2,abc123
guest,guest123
test,test123
```

exemple welcome.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple HTML</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my simple HTML page.</p>
</body>
</html>
```

> [!NOTE]
> La page d'accueil fonctionnera uniquement si le fichier d'authentification n'est pas vide.
> Si le fichier d'authentification est vide, il n'y aura pas d'authentification. :)

Une configuration utilisable est la suivante :

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
auth_file = "/path/to/auth/file"
welcome_page = "/path/to/welcome/html/file"
```

[⬆️ Retour en haut](#toc)

---

#### Support du glossaire

PDFMathTranslate prend en charge la table de glossaire. Le fichier de table de glossaire doit être un fichier `csv`.
Il y a trois colonnes dans le fichier. Voici un exemple de fichier de glossaire :

| source | target  | tgt_lng |
|--------|---------|---------|
| AutoML | 自动 ML  | zh-CN   |
| a,a    | a       | zh-CN   |
| "      | "       | zh-CN   |


Pour les utilisateurs de la ligne de commande :
Vous pouvez utiliser plusieurs fichiers pour le glossaire. Et les différents fichiers doivent être séparés par `,`.

```bash
pdf2zh_next example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"
```

Pour les utilisateurs de l'interface Web :

Vous pouvez maintenant télécharger votre propre fichier de glossaire. Après avoir téléchargé le fichier, vous pouvez le consulter en cliquant sur son nom et le contenu s'affichera ci-dessous.

[⬆️ Retour en haut](#toc)

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>