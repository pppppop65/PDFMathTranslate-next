<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="título">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Destaque｜HelloGitHub" /></a>
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

Tradução de artigos científicos em PDF e comparação bilíngue.

- 📊 Preserve fórmulas, gráficos, sumários e anotações _([pré-visualização](#pré-visualização))_.
- 🌐 Suporta [múltiplos idiomas](https://pdf2zh-next.com/supported_languages.html) e diversos [serviços de tradução](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 Oferece [ferramenta de linha de comando](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [interface de usuário interativa](https://pdf2zh-next.com/getting-started/USAGE_webui.html) e [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

Sinta-se à vontade para fornecer feedback em [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) ou [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl).

Para obter detalhes sobre como contribuir, consulte o [Guia de Contribuição](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="updates">Atualizações</h2>

- [4 de jun. de 2025] O projeto foi renomeado e movido para [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (por [@awwaawwa](https://github.com/awwaawwa))  
- [3 de mar. de 2025] Suporte experimental para o novo backend [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI adicionado como uma opção experimental (por [@awwaawwa](https://github.com/awwaawwa))  
- [22 de fev. de 2025] Melhor CI de lançamento e exe bem empacotado para windows-amd64 (por [@awwaawwa](https://github.com/awwaawwa))  
- [24 de dez. de 2024] O tradutor agora suporta modelos locais no [Xinference](https://github.com/xorbitsai/inference) _(por [@imClumsyPanda](https://github.com/imClumsyPanda))_  
- [19 de dez. de 2024] Documentos não-PDF/A agora são suportados usando `-cp` _(por [@reycn](https://github.com/reycn))_  
- [13 de dez. de 2024] Suporte adicional para backend por _(por [@YadominJinta](https://github.com/YadominJinta))_  
- [10 de dez. de 2024] O tradutor agora suporta modelos OpenAI no Azure _(por [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="preview">Pré-visualização</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Serviço Online 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 atualmente não oferece uma demonstração online

Você pode experimentar nosso aplicativo usando qualquer um dos seguintes demonstrações:

- [Serviço público gratuito v1.x](https://pdf2zh.com/) online sem instalação _(recomendado)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 páginas gratuitas por mês. _(recomendado)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

Observe que os recursos computacionais da demonstração são limitados, portanto, evite abusar deles.

<h2 id="install">Instalação e Uso</h2>

### Instalação

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Recomendado para Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Recomendado para Linux</small>
3. [**uv** (um gerenciador de pacotes Python)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Recomendado para macOS</small>

---

### Uso

1. [Usando a **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Usando o **Plugin do Zotero**](https://github.com/guaguastandup/zotero-pdf2zh) (Programa de terceiros)
3. [Usando a **Linha de comando**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Para diferentes casos de uso, fornecemos métodos distintos para usar nosso programa. Confira [esta página](./getting-started/getting-started.md) para mais informações.

<h2 id="usage">Opções avançadas</h2>

Para explicações detalhadas, consulte nosso documento sobre [Uso avançado](https://pdf2zh-next.com/advanced/advanced.html) para uma lista completa de cada opção.

<h2 id="downstream">Desenvolvimento secundário (APIs)</h2>

> [!NOTE]
>
> Atualmente, nenhuma documentação relevante é fornecida. Será complementada posteriormente. Por favor, aguarde pacientemente.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">Código do idioma</h2>

Se você não sabe qual código usar para traduzir para o idioma que precisa, confira [esta documentação](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="reconhecimento">Reconhecimentos</h2>

- [Immersive Translation](https://immersivetranslate.com) patrocina mensalmente códigos de resgate para assinaturas Pro para contribuidores ativos deste projeto, consulte os detalhes em: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- Versão 1.x: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- Novo backend: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Fusão de documentos: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Análise de documentos: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Extração de documentos: [MinerU](https://github.com/opendatalab/MinerU)

- Visualização de documentos: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Tradução multithread: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- Análise de layout: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Padrão de documento: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Fonte multilíngue: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Registro avançado com multiprocessamento](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">Antes de enviar seu código</h2>

Agradecemos a participação ativa dos contribuidores para tornar o pdf2zh melhor. Antes de estar pronto para enviar seu código, consulte nosso [Código de Conduta](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) e [Guia de Contribuição](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Contribuidores</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="hist_estrela">Histórico de Estrelas</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>