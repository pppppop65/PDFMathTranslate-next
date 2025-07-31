<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="заголовок">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Рекомендуется｜HelloGitHub" /></a>
  <!-- <a href="https://gitcode.com/PDFMathTranslate/PDFMathTranslate-next/overview">
    <img src="https://gitcode.com/PDFMathTranslate/PDFMathTranslate-next/star/badge.svg"></a> -->
  <!-- <a href="https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker">
    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Online%20Demo-FF9E0D"></a> -->
  <!-- <a href="https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate"> -->
    <!-- <img src="https://img.shields.io/badge/ModelScope-Demo-blue"></a> -->
  <!-- <a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/pulls">
    <img src="https://img.shields.io/badge/contributions-welcome-green"></a> -->
  <a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>
  <!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

Перевод научных статей в формате PDF и их двуязычное сравнение.

- 📊 Сохраняет формулы, диаграммы, оглавление и аннотации _([предпросмотр](#preview))_.
- 🌐 Поддерживает [несколько языков](https://pdf2zh-next.com/supported_languages.html) и различные [службы перевода](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 Предоставляет [инструмент командной строки](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [интерактивный пользовательский интерфейс](https://pdf2zh-next.com/getting-started/USAGE_webui.html) и [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

Не стесняйтесь оставлять отзывы в [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) или [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl).

Для получения подробной информации о том, как внести свой вклад, обратитесь к [Руководству по участию](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="updates">Обновления</h2>

- [4 июня 2025] Проект переименован и перемещён в [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (от [@awwaawwa](https://github.com/awwaawwa))
- [3 марта 2025] Добавлена экспериментальная поддержка нового бэкенда [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI в качестве экспериментальной опции (от [@awwaawwa](https://github.com/awwaawwa))
- [22 февраля 2025] Улучшен CI для релизов и хорошо упакованный exe-файл для windows-amd64 (от [@awwaawwa](https://github.com/awwaawwa))
- [24 декабря 2024] Переводчик теперь поддерживает локальные модели на [Xinference](https://github.com/xorbitsai/inference) _(от [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19 декабря 2024] Теперь поддерживаются документы не в формате PDF/A с использованием `-cp` _(от [@reycn](https://github.com/reycn))_
- [13 декабря 2024] Дополнительная поддержка бэкенда _(от [@YadominJinta](https://github.com/YadominJinta))_
- [10 декабря 2024] Переводчик теперь поддерживает модели OpenAI на Azure _(от [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="preview">Предварительный просмотр</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Онлайн-сервис 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 в настоящее время не предоставляет онлайн-демонстрацию

Вы можете попробовать наше приложение, используя одно из следующих демо:

- [v1.x Бесплатный публичный сервис](https://pdf2zh.com/) доступен онлайн без установки _(рекомендуется)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 бесплатных страниц в месяц. _(рекомендуется)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

Обратите внимание, что вычислительные ресурсы демо-версии ограничены, поэтому, пожалуйста, избегайте их злоупотребления.

<h2 id="install">Установка и использование</h2>

### Установка

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Рекомендуется для Windows</small>  
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Рекомендуется для Linux</small>  
3. [**uv** (менеджер пакетов Python)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Рекомендуется для macOS</small>

---

### Использование

1. [Использование **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Использование **Zotero Plugin**](https://github.com/guaguastandup/zotero-pdf2zh) (Сторонняя программа)
3. [Использование **Командной строки**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Для различных случаев использования мы предоставляем различные методы работы с нашей программой. Подробнее можно узнать на [этой странице](./getting-started/getting-started.md).

<h2 id="usage">Расширенные параметры</h2>

Подробные объяснения можно найти в нашем документе о [Расширенном использовании](https://pdf2zh-next.com/advanced/advanced.html), где приведен полный список каждого параметра.

<h2 id="downstream">Вторичная разработка (API)</h2>

> [!NOTE]
>
> В настоящее время соответствующая документация не предоставлена. Она будет дополнена позже. Пожалуйста, ожидайте терпеливо.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">Код языка</h2>

Если вы не знаете, какой код использовать для перевода на нужный вам язык, ознакомьтесь с [этой документацией](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="благодарности">Благодарности</h2>

- [Immersive Translation](https://immersivetranslate.com) предоставляет ежемесячные коды для активации Pro-подписки активным участникам этого проекта. Подробности см. в: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- Версия 1.x: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- Новый бэкенд: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Объединение документов: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Парсинг документов: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Извлечение документов: [MinerU](https://github.com/opendatalab/MinerU)

- Просмотр документов: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Многопоточный перевод: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- Анализ макета: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Стандарт документов: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Многоязычные шрифты: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Богатое логирование с многопроцессорностью](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">Перед отправкой вашего кода</h2>

Мы приветствуем активное участие участников, чтобы сделать pdf2zh лучше. Прежде чем вы будете готовы отправить свой код, пожалуйста, ознакомьтесь с нашим [Кодексом поведения](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) и [Руководством по вкладу](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Участники</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">История звезд</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>