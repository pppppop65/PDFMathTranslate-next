[**開始**](./getting-started.md) > **インストール** > **Windows EXE** _(current)_

---

### .exe ファイル経由で PDFMathTranslate をインストールする

***ステップ 1*** | [リリースページ](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases)から`pdf2zh-<version>-with-assets-win64.zip`をダウンロードしてください。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip`と`pdf2zh-<version>-win64.zip`の違いは何ですか？**
>
> - PDFMathTranslate を初めてダウンロードして使用する場合は、`pdf2zh-<version>-with-assets-win64.zip`をダウンロードすることをお勧めします。
> - `pdf2zh-<version>-with-assets-win64.zip`には、`pdf2zh-<version>-win64.zip`と比較してリソースファイル（フォントやモデルなど）が含まれています。
> - アセットなしのバージョンも実行時にリソースを動的にダウンロードしますが、ネットワークの問題によりダウンロードが失敗する可能性があります。

***ステップ 2*** | `pdf2zh-<version>-with-assets-win64.zip`を解凍し、`pdf2zh`フォルダに移動します。解凍には時間がかかる場合がありますので、しばらくお待ちください。

***ステップ 3*** | `pdf2zh`フォルダに移動し、`pdf2zh.exe`をダブルクリックします。

> [!TIP]
> **.exe ファイルを実行できない場合**
>
> pdf2zh.exe の実行に問題がある場合は、`https://aka.ms/vs/17/release/vc_redist.x64.exe`をインストールしてから再度お試しください。

***ステップ 4*** | exe ファイルをダブルクリックするとターミナルが表示されます。約 30 秒から 1 分後に、デフォルトのブラウザでウェブページが開きます。開かない場合は、手動で`http://localhost:7860/`にアクセスしてみてください。

> [!NOTE]
>
> WebUI の使用中に問題が発生した場合は、[このウェブページ](./USAGE_webui.md)を参照してください。

***ステップ 5*** | お楽しみください！

> [!TIP]
> **.exe ファイルはコマンドラインから使用可能**
>
> 以下の手順で.exe ファイルをコマンドラインから使用できます：
>
> - ターミナルを起動し、.exe ファイルが含まれるフォルダに移動：
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - .exe ファイルを呼び出し：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> 通常通り他のコマンドラインパラメータも使用可能：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> コマンドラインの使い方についてさらに情報が必要な場合は、こちらの記事を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>