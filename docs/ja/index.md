<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="タイトル">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
<a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
<a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
<a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
<a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Featured｜HelloGitHub" /></a>
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

PDF 科学論文の翻訳とバイリンガル比較。

- 📊 数式、チャート、目次、注釈を保持 _([プレビュー](#プレビュー))_。
- 🌐 [複数言語](https://pdf2zh-next.com/supported_languages.html)をサポートし、多様な[翻訳サービス](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html)に対応。
- 🤖 [コマンドラインツール](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)、[インタラクティブユーザーインターフェース](https://pdf2zh-next.com/getting-started/USAGE_webui.html)、[Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)を提供

フィードバックは[GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues)または[Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl)でお気軽にお寄せください。

貢献方法の詳細については、[Contribution Guide](https://pdf2zh-next.com/community/Contribution-Guide.html)をご参照ください。

<h2 id="updates">更新情報</h2>

- [2025 年 6 月 4 日] プロジェクト名が変更され、[PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) に移動しました (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 年 3 月 3 日] 新しいバックエンド [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI の実験的サポートが追加され、実験的オプションとして利用可能になりました (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 年 2 月 22 日] リリース CI の改善と、Windows-amd64 用の exe ファイルの適切なパッケージ化 (by [@awwaawwa](https://github.com/awwaawwa))
- [2024 年 12 月 24 日] 翻訳ツールが [Xinference](https://github.com/xorbitsai/inference) 上のローカルモデルをサポート _(by [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [2024 年 12 月 19 日] `-cp` を使用して非 PDF/A ドキュメントがサポートされるようになりました _(by [@reycn](https://github.com/reycn))_
- [2024 年 12 月 13 日] 追加のバックエンドサポート _(by [@YadominJinta](https://github.com/YadominJinta))_
- [2024 年 12 月 10 日] 翻訳ツールが Azure 上の OpenAI モデルをサポート _(by [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="preview">プレビュー</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">オンラインサービス 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 は現在オンラインデモを提供していません

以下のデモのいずれかを使用して、アプリケーションをお試しいただけます：

- [v1.x パブリック無料サービス](https://pdf2zh.com/) インストール不要でオンライン利用可能 _(推奨)_
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 月間 1000 ページ無料 _(推奨)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

デモの計算リソースは限られているため、乱用は避けてください。

<h2 id="install">インストールと使い方</h2>

### インストール

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Windows 向け推奨</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Linux 向け推奨</small>
3. [**uv** (Python パッケージマネージャー)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>macOS 向け推奨</small>

---

### 使い方

1. [**WebUI**を使う](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [**Zotero Plugin**を使う](https://github.com/guaguastandup/zotero-pdf2zh) (サードパーティプログラム)
3. [**コマンドライン**を使う](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

様々な使用ケースに対応するため、当プログラムには複数の利用方法が用意されています。詳細は[このページ](./getting-started/getting-started.md)をご覧ください。

<h2 id="usage">高度なオプション</h2>

各オプションの詳細な説明については、[高度な使い方](https://pdf2zh-next.com/advanced/advanced.html)のドキュメントを参照してください。

<h2 id="downstream">二次開発（API）</h2>

> [!NOTE]
>
> 現在、関連するドキュメントは提供されていません。後日追加されますので、しばらくお待ちください。


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">言語コード</h2>

必要な言語に翻訳するためのコードがわからない場合は、[このドキュメント](https://pdf2zh-next.com/advanced/Language-Codes.html)を確認してください

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="acknowledgement">謝辞</h2>

- [没入型翻訳](https://immersivetranslate.com) はこのプロジェクトの積極的な貢献者向けに月額 Pro メンバーシップの引き換えコードを提供しています。詳細はこちら：[CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- 1.x バージョン：[Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- 新しいバックエンド：[BabelDOC](https://github.com/funstory-ai/BabelDOC)

- ドキュメント結合：[PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- ドキュメント解析：[Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- ドキュメント抽出：[MinerU](https://github.com/opendatalab/MinerU)

- ドキュメントプレビュー: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- マルチスレッド翻訳：[MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- レイアウト解析：[DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- ドキュメント標準：[PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多言語フォント：[Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [マルチプロセス対応のリッチロギング](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">コードを提出する前に</h2>

pdf2zh をより良くするために、貢献者の積極的な参加を歓迎します。コードを提出する準備が整う前に、[行動規範](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)と[貢献ガイド](https://pdf2zh-next.com/community/Contribution-Guide.html)を参照してください。

<h2 id="contrib">貢献者</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">スターの歴史</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
</picture>
</a>

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>