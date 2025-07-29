[**高級選項**](./introduction.md) > **翻譯服務文檔** _(current)_

---

### 通過命令行查看可用的翻譯服務

您可以通過在命令行中打印幫助訊息來確認可用的翻譯服務及其使用方法。

```bash
pdf2zh_next -h
```

在幫助訊息的結尾，您可以查看不同翻譯服務的詳細資訊。

---

> [!CAUTION]
> 以下內容是為 pdf2zh 1.x 版本準備的，尚未針對 2.x 版本進行更新。因此，這些資訊可能**已過時**。
>
> 一旦文章內容與新版本保持一致，此警告訊息將被移除。

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### 使用不同服務進行翻譯

我們提供了一份詳細的表格，列出了每個翻譯服務所需的[環境變量](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4)。請確保在使用相應服務前設置好這些變量。

| **翻譯器**           | **服務**       | **環境變數**                                                          | **預設值**                                               | **備註**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (預設)**    | `google`       | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[您的金鑰]`                                             | 參閱 [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | 參見 [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | 參見 [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | 參閱 [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[您的金鑰]`, `gpt-4o-mini` | 參閱 [OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[您的端點]`, `[您的金鑰]`, `gpt-4o-mini`           | 參閱 [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | 參見 [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[您的金鑰]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | 參見 [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | 參閱 [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | 參見 [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | 參見 [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | 參閱 [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[您的 DIFY URL]`, `[您的金鑰]`                          | 參見 [Dify](https://github.com/langgenius/dify)，需在 Dify 的工作流輸入中定義三個變量：lang_out、lang_in 和 text。                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[您的 AnythingLLM URL]`, `[您的金鑰]`                   | 參閱 [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | 參見 [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[您的 GORK_API_KEY]`, `grok-2-1212`                     | 參閱 [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[您的 GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | 參見 [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[您的 DEEPSEEK_API_KEY]`, `deepseek-chat`               | 參見 [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **阿里通義翻譯** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[您的密鑰]`, `scientific paper`        | 目前尚未支持繁體中文，將被翻譯為簡體中文。更多資訊請參閱 [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

對於與 OpenAI API 相容但未在上表中列出的大型語言模型，您可以使用表格中針對 OpenAI 所述的相同方法設定環境變數。

使用 `-s service` 或 `-s service:model` 來指定服務：

```

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

或者透過環境變數指定模型：

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

對於 PowerShell 使用者：

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>