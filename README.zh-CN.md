<h1 align="center">
	<a href="https://github.com/mnfst/awesome-free-llm-apis">
		<img src="media/awesome-free-llm-apis.png" width="500" alt="Awesome 免费 LLM API">
	</a>
</h1>

<p align="center">
	<a href="README.md">English</a> | 简体中文
</p>

<p align="center">
	<a href="https://awesome.re">
		<img src="https://awesome.re/badge-flat2.svg" alt="Awesome">
	</a>
</p>

<p align="center">提供永久免费额度、用于文本推理的 LLM API。</p>

<p align="center"><sub>大多数提供商都提供 OpenAI 兼容端点。原生基础 URL 与兼容基础 URL 可能不同。每个链接都指向该提供商的 API 密钥页面。</sub></p>

<p align="center"><sub>上述所有免费 LLM API 都可以在 <a href="https://manifest.build">manifest.build</a> 使用——构建可靠的智能体。</sub></p>

<hr>

<h3 align="center">赞助商</h3>

<p align="center">
	<a href="https://okapi.bot/go/awesome-free-llm-apis">
		<picture>
			<source media="(prefers-color-scheme: dark)" srcset="media/okapi-logo-dark.svg">
			<img src="media/okapi-logo-light.svg" width="180" alt="Okapi">
		</picture>
	</a>
	<br>
	<sub>免费 API 监控。不再有破坏性变更。</sub>
</p>

<hr>

## 目录

- [提供商 API](#提供商-api)
- [推理提供商](#推理提供商)
- [术语表](#术语表)

## 提供商 API

由自行训练或微调模型的公司运营的 API。

### [Aion Labs](https://www.aionlabs.ai/app/api-keys/) 🇮🇱

永久免费额度，无需信用卡。15 RPM，每天 20K token。专用于角色扮演与故事叙述。

基础 URL：`https://api.aionlabs.ai/v1`

| 模型名称                         | 上下文 | 最大输出 | 模态         | 速率限制        |
| -------------------------------- | ------ | -------- | ------------ | --------------- |
| `aion-labs/aion-2.0`             | 128K   | 32K      | 文本（推理） | 15 RPM, 20K TPD |
| `aion-labs/aion-rp-llama-3.1-8b` | 32K    | 32K      | 文本         | 15 RPM, 20K TPD |
| `aion-labs/aion-3.0`             | 128K   | 32K      | 文本（推理） | 15 RPM, 20K TPD |
| `aion-labs/aion-3.0-mini`        | 128K   | 32K      | 文本（推理） | 15 RPM, 20K TPD |

### [Cohere](https://dashboard.cohere.com/api-keys) 🇨🇦

免费 “Trial” API 密钥，无需信用卡。每月 1,000 次 API 调用。仅限非商业用途。

原生 API 基础 URL：`https://api.cohere.com/v2`

OpenAI 兼容基础 URL：`https://api.cohere.ai/compatibility/v1`

| 模型名称            | 上下文 | 最大输出 | 模态         | 速率限制 |
| ------------------- | ------ | -------- | ------------ | -------- |
| Command A+ (218B)   | 128K   | 64K      | 文本 + 图像  | 20 RPM   |
| Command A (111B)    | 256K   | 8K       | 文本         | 20 RPM   |
| Command R+          | 128K   | 4K       | 文本         | 20 RPM   |
| Command R           | 128K   | 4K       | 文本         | 20 RPM   |
| Command R7B         | 128K   | 4K       | 文本         | 20 RPM   |
| Command A Reasoning | 256K   | 32K      | 文本（推理） | 20 RPM   |
| Command A Translate | 8K     | 8K       | 文本         | 20 RPM   |
| Command A Vision    | 128K   | 8K       | 文本 + 图像  | 20 RPM   |
| Command R7B Arabic  | 128K   | ~4K      | 文本         | 20 RPM   |
| Aya Expanse 32B     | 128K   | 4K       | 文本         | 20 RPM   |
| Aya Vision 32B      | 16K    | 4K       | 文本 + 图像  | 20 RPM   |

### [Google Gemini](https://aistudio.google.com/app/apikey) 🇺🇸

免费额度，无需信用卡。免费额度下的提示词可能会被 Google 用于改进产品。[^1]

原生 API 基础 URL：`https://generativelanguage.googleapis.com/v1beta`

OpenAI 兼容基础 URL：`https://generativelanguage.googleapis.com/v1beta/openai/`

| 模型名称              | 上下文 | 最大输出 | 模态                         | 速率限制 |
| --------------------- | ------ | -------- | ---------------------------- | -------- |
| Gemini 3.8 Flash      | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemini 3.6 Flash      | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemini 3.5 Flash-Lite | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemini 3.1 Flash-Lite | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemini 2.5 Flash      | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemini 2.5 Flash-Lite | 1M     | 65K      | 文本 + 图像 + 音频 + 视频    | —        |
| Gemma 4 31B           | 256K   | 32K      | 文本 + 图像                  | —        |
| Gemma 4 26B A4B       | 256K   | 32K      | 文本 + 图像                  | —        |

### [Mistral AI](https://console.mistral.ai/api-keys) 🇫🇷

免费模式默认开启，无需信用卡。除非你选择退出，否则免费模式的提示词可能会被用于训练 Mistral 模型。[^13]

基础 URL：`https://api.mistral.ai/v1`

| 模型名称                  | 上下文 | 最大输出 | 模态                | 速率限制         |
| ------------------------- | ------ | -------- | ------------------- | ---------------- |
| Mistral Medium 3.5 (128B) | 256K   | —        | 文本 + 图像 + 代码  | ~1 RPS, 500K TPM |
| Mistral Small 4           | 256K   | —        | 文本 + 图像 + 代码  | ~1 RPS, 500K TPM |
| Mistral Large 3           | 256K   | —        | 多模态              | ~1 RPS, 500K TPM |
| Ministral 3 8B            | 256K   | —        | 文本 + 视觉         | ~1 RPS, 500K TPM |
| Codestral                 | 128K   | —        | 代码                | ~1 RPS, 500K TPM |
| Ministral 3 3B            | 256K   | —        | 文本 + 视觉         | ~1 RPS, 500K TPM |
| Ministral 3 14B           | 256K   | —        | 文本 + 视觉         | ~1 RPS, 500K TPM |

### [Z AI (Zhipu AI)](https://open.bigmodel.cn/usercenter/apikeys) 🇨🇳

永久免费模型，无需信用卡。[^12]

基础 URL：`https://open.bigmodel.cn/api/paas/v4`

| 模型名称                             | 上下文 | 最大输出 | 模态         | 速率限制     |
| ------------------------------------ | ------ | -------- | ------------ | ------------ |
| GLM-4.7-Flash                        | 200K   | 128K     | 文本（推理） | 1 个并发请求 |
| GLM-4.5-Flash（已宣布停用）          | 128K   | 96K      | 文本（推理） | 1 个并发请求 |
| GLM-4.6V-Flash                       | 128K   | 32K      | 多模态       | 1 个并发请求 |

## 推理提供商

托管来自不同来源的开放权重模型的第三方平台。

### [Cloudflare Workers AI](https://dash.cloudflare.com/profile/api-tokens) 🇺🇸

每天免费 10,000 Neurons，无需信用卡。免费额度可用 60 余个模型。[^11]

原生 API 基础 URL：`https://api.cloudflare.com/client/v4/accounts/{account_id}/ai/run`

OpenAI 兼容基础 URL：`https://api.cloudflare.com/client/v4/accounts/{account_id}/ai/v1`

| 模型名称                                       | 上下文 | 最大输出     | 模态                       | 速率限制                 |
| ---------------------------------------------- | ------ | ------------ | -------------------------- | ------------------------ |
| `@cf/meta/llama-3.3-70b-instruct-fp8-fast`     | 24K    | 与上下文共享 | 文本                       | 每天 10K neurons（共享） |
| `@cf/meta/llama-4-scout-17b-16e-instruct`      | 131K   | 与上下文共享 | 多模态                     | 每天 10K neurons（共享） |
| `@cf/openai/gpt-oss-120b`                      | 128K   | 与上下文共享 | 文本                       | 每天 10K neurons（共享） |
| `@cf/google/gemma-4-26b-a4b-it`                | 256K   | 与上下文共享 | 文本 + 视觉                | 每天 10K neurons（共享） |
| `@cf/zai-org/glm-4.7-flash`                    | 131K   | 与上下文共享 | 文本                       | 每天 10K neurons（共享） |
| `@cf/mistralai/mistral-small-3.1-24b-instruct` | 128K   | 与上下文共享 | 文本 + 视觉                | 每天 10K neurons（共享） |
| `@cf/deepseek-ai/deepseek-r1-distill-qwen-32b` | 80K    | 与上下文共享 | 文本（推理）               | 每天 10K neurons（共享） |
| + 另外 55 个模型                               | 各异   | 各异         | 文本、图像、音频、嵌入     | 每天 10K neurons（共享） |

### [Gonka Broker](https://app.gonkabroker.com/signup) 🇺🇸

永久免费额度，无需信用卡；需要手机验证。每月约 1M token（共享，因模型而异），按月重置。模型阵容随网络治理轮换——实时列表见 /v1/models。[^14]

基础 URL：`https://proxy.gonkabroker.com/v1`

| 模型名称                             | 上下文 | 最大输出 | 模态         | 速率限制                               |
| ------------------------------------ | ------ | -------- | ------------ | -------------------------------------- |
| `MiniMaxAI/MiniMax-M2.7`             | 200K   | 16K      | 文本（推理） | 每月约 1M token（共享，因模型而异）    |
| `deepseek-ai/DeepSeek-V4-Flash-0731` | 400K   | 16K      | 文本（推理） | 每月约 1M token（共享，因模型而异）    |
| `zai-org/GLM-5.3-Flash`              | 400K   | 16K      | 文本（推理） | 每月约 1M token（共享，因模型而异）    |
| `BAAI/bge-m3`                        | 8K     | —        | 嵌入         | 每月约 1M token（共享，因模型而异）    |

### [Groq](https://console.groq.com/keys) 🇺🇸

免费额度，无需信用卡。超高速 LPU 推理。[^2]

基础 URL：`https://api.groq.com/openai/v1`

| 模型名称              | 上下文 | 最大输出 | 模态         | 速率限制          |
| --------------------- | ------ | -------- | ------------ | ----------------- |
| `openai/gpt-oss-120b` | 131K   | 65K      | 文本         | 30 RPM, 1,000 RPD |
| `openai/gpt-oss-20b`  | 131K   | 65K      | 文本         | 30 RPM, 1,000 RPD |
| `qwen/qwen3.8-27b`    | 131K   | 16K      | 文本 + 图像  | 30 RPM, 1,000 RPD |

### [Kilo Code](https://app.kilo.ai/profile) 🇺🇸

免费模型，无需信用卡，也无需 API 密钥。`kilo-auto/free` 自动路由器会动态路由到免费池中的模型。[^5]

基础 URL：`https://api.kilo.ai/api/gateway`

| 模型名称                                             | 上下文 | 最大输出 | 模态          | 速率限制         |
| ---------------------------------------------------- | ------ | -------- | ------------- | ---------------- |
| `nvidia/nemotron-3-ultra-550b-a55b:free`             | 1M     | 65K      | 文本          | 每小时 200 次请求 |
| `nvidia/nemotron-3-nano-omni-30b-a3b-reasoning:free` | 256K   | 65K      | 多模态        | 每小时 200 次请求 |
| `cohere/north-mini-code:free`                        | 256K   | 64K      | 文本（代码）  | 每小时 200 次请求 |
| `openrouter/free`                                    | 各异   | 各异     | 文本          | 每小时 200 次请求 |
| `nvidia/nemotron-3.5-lightning:free`                 | 1M     | 65K      | 文本          | 每小时 200 次请求 |
| `kilo-auto/free`                                     | 256K   | 32K      | 文本          | 每小时 200 次请求 |
| `dots-studio/dots-3-note-preview:free`               | 512K   | 460K     | 文本 + 视觉   | 每小时 200 次请求 |
| `nvidia/nemotron-3.5-super-vl:free`                  | 1M     | 131K     | 多模态        | 每小时 200 次请求 |
| `reflection/beam-free`                               | 1M     | 131K     | 文本          | 每小时 200 次请求 |
| `stealth/glyph-cluster`                              | 256K   | 256K     | 文本（代码）  | 每小时 200 次请求 |

### [LLM7.io](https://token.llm7.io) 🇬🇧

提供免费额度的 API 网关。匿名访问无需密钥即可使用 `turbo` 模型；从 token.llm7.io 获取的免费 token 会提高速率与 token 上限，但能访问的仍是同一批模型。[^10]

基础 URL：`https://api.llm7.io/v1`

| 模型名称                   | 上下文 | 最大输出 | 模态         | 速率限制                              |
| -------------------------- | ------ | -------- | ------------ | ------------------------------------- |
| `gpt-oss:20b`              | 128K   | —        | 文本         | 60 RPM，每小时 250 次请求（免费 token） |
| mistral-Nemo-Instruct-2407 | 128K   | —        | 文本         | 60 RPM，每小时 250 次请求（免费 token） |
| `nemotron-3-nano:30b`      | 1M     | —        | 文本（推理） | 60 RPM，每小时 250 次请求（免费 token） |
| codestral-latest           | 32K    | —        | 文本         | 60 RPM，每小时 250 次请求（免费 token） |

### [ModelScope](https://modelscope.cn/my/myaccesstoken) 🇨🇳

面向注册用户的免费 API-Inference。需要绑定阿里云账号并完成实名认证。[^6]

基础 URL：`https://api-inference.modelscope.cn/v1`

| 模型名称                       | 上下文 | 最大输出 | 模态      | 速率限制                                 |
| ------------------------------ | ------ | -------- | --------- | ---------------------------------------- |
| `Qwen/Qwen3.5-35B-A3B`         | 256K   | —        | 文本      | 合计 2,000 RPD；每模型 ≤500 RPD（动态）  |
| `Qwen/Qwen3.5-27B`             | 256K   | —        | 文本      | 合计 2,000 RPD；每模型 ≤500 RPD（动态）  |
| + 已启用 API-Inference 的模型  | 各异   | 各异     | LLM、MLLM | 动态配额 + 动态并发                      |

### [NVIDIA NIM](https://build.nvidia.com/explore/discover) 🇺🇸

加入 NVIDIA Developer Program 即可免费使用。100 余个模型。按模型限速。

基础 URL：`https://integrate.api.nvidia.com/v1`

| 模型名称                            | 上下文 | 最大输出 | 模态                               | 速率限制           |
| ----------------------------------- | ------ | -------- | ---------------------------------- | ------------------ |
| `google/gemma-4-31b-it`             | 262K   | 8K       | 文本 + 图像 + 视频                 | 40 RPM, 10,000 RPD |
| `nvidia/nemotron-3-ultra-550b-a55b` | 1M     | 262K     | 文本                               | 40 RPM, 10,000 RPD |
| `openai/gpt-oss-20b`                | 131K   | 131K     | 文本                               | 40 RPM, 10,000 RPD |
| + 另外 92 个模型                    | 各异   | 各异     | 文本、图像、视频、语音、嵌入       | 40 RPM, 10,000 RPD |

### [OpenRouter](https://openrouter.ai/keys) 🇺🇸

17 个免费模型（以 `:free` 后缀标记）。兼容 OpenAI SDK。[^4]

基础 URL：`https://openrouter.ai/api/v1`

| 模型名称                                             | 上下文 | 最大输出 | 模态                         | 速率限制       |
| ---------------------------------------------------- | ------ | -------- | ---------------------------- | -------------- |
| `cohere/north-mini-code:free`                        | 256K   | 64K      | 文本（代码）                 | 20 RPM, 50 RPD |
| `google/gemma-4-26b-a4b-it:free`                     | 262K   | 32K      | 文本 + 图像 + 视频           | 20 RPM, 50 RPD |
| `google/gemma-4-31b-it:free`                         | 262K   | 32K      | 文本 + 图像 + 视频           | 20 RPM, 50 RPD |
| `dots-studio/dots-3-note-preview:free`               | 512K   | 460K     | 文本 + 图像                  | 20 RPM, 50 RPD |
| `liquid/lfm-2.5-2.6b:free`                           | 64K    | 8K       | 文本                         | 20 RPM, 50 RPD |
| `nvidia/nemotron-3.5-lightning:free`                 | 1M     | 65K      | 文本                         | 20 RPM, 50 RPD |
| `nvidia/nemotron-3-ultra-550b-a55b:free`             | 1M     | 65K      | 文本                         | 20 RPM, 50 RPD |
| `recursive/flint-v1.0:free`                          | 262K   | 235K     | 文本                         | 20 RPM, 50 RPD |
| `xingchen-agi/xing4.0-29b-a4b:free`                  | 262K   | 235K     | 文本                         | 20 RPM, 50 RPD |
| `nvidia/nemotron-3.5-super-vl:free`                  | 1M     | 131K     | 文本 + 图像 + 视频           | 20 RPM, 50 RPD |
| `nvidia/nemotron-3-nano-omni-30b-a3b-reasoning:free` | 256K   | 65K      | 文本 + 图像 + 音频 + 视频    | 20 RPM, 50 RPD |

### [OVHcloud AI Endpoints](https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/) 🇫🇷

免费匿名额度（无需 API 密钥，无需注册）：每个 IP、每个模型 2 RPM。20 余个开放权重模型托管于欧盟。兼容 OpenAI SDK。[^7]

基础 URL：`https://oai.endpoints.kepler.ai.cloud.ovh.net/v1`

| 模型名称                       | 上下文 | 最大输出 | 模态          | 速率限制      |
| ------------------------------ | ------ | -------- | ------------- | ------------- |
| Qwen3.5-397B-A17B              | 262K   | ~32K     | 文本 + 视觉   | 2 RPM（匿名） |
| gpt-oss-120b                   | 131K   | ~32K     | 文本          | 2 RPM（匿名） |
| gpt-oss-20b                    | 131K   | ~8K      | 文本          | 2 RPM（匿名） |
| Meta-Llama-3_3-70B-Instruct    | 131K   | ~4K      | 文本          | 2 RPM（匿名） |
| Qwen3.8-27B                    | 262K   | —        | 文本 + 视觉   | 2 RPM（匿名） |
| Qwen3.6-27B                    | 262K   | ~32K     | 文本 + 视觉   | 2 RPM（匿名） |
| Qwen3.5-9B                     | 262K   | ~8K      | 文本 + 视觉   | 2 RPM（匿名） |
| Qwen2.5-VL-72B-Instruct        | 32K    | ~8K      | 文本 + 视觉   | 2 RPM（匿名） |
| Mistral-Small-3.2-24B-Instruct | 128K   | ~4K      | 文本 + 视觉   | 2 RPM（匿名） |

### [SiliconFlow](https://cloud.siliconflow.cn/account/ak) 🇨🇳

永久免费模型，无需信用卡。需要身份验证。目录中有 100 余个模型，其中大多数为付费模型。[^9]

基础 URL：`https://api.siliconflow.cn/v1`

| 模型名称                  | 上下文 | 最大输出 | 模态 | 速率限制 |
| ------------------------- | ------ | -------- | ---- | -------- |
| `tencent/Hunyuan-MT-7B`   | —      | —        | 文本 | —        |
| `XingChenAGI/Xing4.0-29B` | —      | —        | 文本 | —        |

## 术语表

| 缩写    | 含义           |
| ------- | -------------- |
| **RPM** | 每分钟请求数   |
| **RPD** | 每天请求数     |
| **TPM** | 每分钟 token 数 |
| **TPD** | 每天 token 数  |
| **RPS** | 每秒请求数     |

## 贡献

知道还有遗漏的免费额度？[提交 PR](contributing.md)。请写明提供商、端点、速率限制（附上其文档链接）以及若干值得关注的模型。试用额度与限时促销不算。

[^1]: Gemini API 免费额度向欧盟、英国和瑞士的开发者开放；[可用地区](https://ai.google.dev/gemini-api/docs/available-regions)页面列出了这些地区。[条款](https://ai.google.dev/gemini-api/terms)仍要求：当你向欧洲经济区、瑞士或英国的用户提供 API Client 时，只能使用 Paid Services（付费服务）。Google 不再公布各模型的免费额度速率限制；请在 [AI Studio](https://aistudio.google.com/) 中查看你的配额。免费额度下的提示词可能会被 Google 用于改进产品，但欧洲经济区、瑞士和英国的用户除外：这些地区的未付费配额同样适用付费服务的数据条款，因此这些提示词不会被用于改进 Google 产品。`gemini-3.1-flash-lite` 已列入[弃用时间表](https://ai.google.dev/gemini-api/docs/deprecations)，关停日期为 2027 年 5 月 7 日，替代模型为 `gemini-3.5-flash-lite`；该行仍予保留，因为该模型目前仍在线且免费。
[^2]: Groq 已于 2026 年 9 月 14 日下线 qwen/qwen3.6-27b（由 qwen/qwen3.8-27b 替代），并于 2026 年 9 月 21 日下线 groq/compound 与 groq/compound-mini（[弃用说明](https://console.groq.com/docs/deprecations)）。免费计划的限制因模型而异；所列对话模型的额度为 1,000 RPD（[速率限制](https://console.groq.com/docs/rate-limits)）。
[^4]: 免费模型允许每分钟 20 次请求、每天 50 次请求，在所有免费模型之间合计计算。至少购买过 10 credits 的账户每天可获得 1,000 次请求（[限制](https://openrouter.ai/docs/api-reference/limits)）。OpenRouter 还提供 [Free Models Router](https://openrouter.ai/docs/guides/routing/routers/free-router)（`openrouter/free`）以及[模型回退](https://openrouter.ai/docs/guides/routing/model-fallbacks)，可按优先级串联模型。免费提供商可能会记录提示词用于训练。
[^5]: Kilo Code 的免费池变动频繁，而且 /api/gateway/models 目录可能滞后于实际提供的服务：探测结果已确认，目录中未列出的模型仍会应答。截至 liquid/lfm-2.5-2.6b:free 的各行曾在 2026-08-19 至 2026-08-21 之间响应过实时请求；其后的各行分别于 2026-10-05（截至 dots-studio/dots-3-note-preview:free）、2026-10-23 和 2026-10-25 从目录中加入，目录中标价为 $0，且尚未经过探测。目录将 reflection/beam-free 描述为经由 Vercel AI Gateway 提供，并注明提示词可能会被保留用于训练。免费模型无需 API 密钥即可访问，每个 IP 每小时 200 次请求（[身份验证](https://kilo.ai/docs/gateway/authentication)）。kilo-auto/free 路由器从免费池中挑选模型，Kilo 的文档警告它 “may route your requests to providers that log prompts and outputs”（可能会把你的请求路由到会记录提示词与输出的提供商）。NVIDIA 免费端点附带 NVIDIA 自己的条件，引述自 Kilo 的[模型页面](https://kilo.ai/docs/gateway/models-and-providers)：“Trial use only - do not submit personal or confidential data. Your use is logged for security purposes and to improve NVIDIA products and services.”（仅供试用——请勿提交个人或机密数据。你的使用会被记录，用于安全目的以及改进 NVIDIA 的产品与服务。）
[^6]: API-Inference 对注册用户免费。目前公布的限制为每用户每天 2,000 次请求（跨模型合计），各模型的每日配额会动态调整且上限为 500；并发同样受动态限速。需要绑定阿里云账号并完成实名认证（[限制](https://modelscope.cn/docs/model-service/API-Inference/limits)、[介绍](https://modelscope.cn/docs/model-service/API-Inference/intro)）。本条目依据 ModelScope 的文档编写。无法从中国大陆以外进行测试。
[^7]: OVHcloud AI Endpoints 提供永久免费匿名额度（每个 IP、每个模型每分钟 2 次请求），无需注册或 API 密钥。更高的速率限制（每个 Public Cloud 项目、每个模型 400 RPM）需要 API 密钥，并按 token 即用即付计费；新的 Public Cloud 账户最多可获得 $200 免费试用额度。模型托管在欧盟的数据中心。目录列出 Mistral-Small-3.2-24B-Instruct-2506 与 Mistral-Nemo-Instruct-2407 的生命周期结束日期为 2026 年 11 月 4 日。
[^9]: 使用 SiliconFlow 的免费模型需要实名身份验证（据[发布说明](https://api-docs.siliconflow.cn/docs/release-notes/overview)，自 2026 年 5 月 15 日起生效）。验证支持中国大陆证件；国际用户必须联系支持人员。本条目依据 SiliconFlow 的[定价页面](https://siliconflow.cn/pricing)，该页面将这些模型标为免费。无法从中国大陆以外进行测试。
[^10]: LLM7.io 频繁轮换其目录，因此两次核查之间模型列表会发生变化。访问按层级划分，而不是按 token 划分：`turbo` 模型可匿名访问，也可使用免费 token 访问；`pro` 模型需要付费计划（[模型 API](https://docs.llm7.io/guides/models-api)）。免费 token 的上限为 1 RPS、60 RPM、每小时 250 次请求以及每 24 小时 100,000 token，免费配额可能在不另行通知的情况下被下调（[限制](https://docs.llm7.io/limits)）。付费 Pro 计划的价格为每月 $12。文档不再列出匿名（无密钥）限制；匿名访问最近一次由实时请求确认是在 2026-08-21。
[^11]: 10,000 个免费 Neurons 在全部 Workers AI 用量之间共享，而不是按模型计算，并且所有限制都在每天 00:00 UTC 重置。超出后不会向你计费，该请求会失败。有七个模型被排除在 Workers Free 计费之外，需要 Workers Paid 计划或预付的 AI Gateway 额度：`@cf/moonshotai/kimi-k2.6`、`@cf/moonshotai/kimi-k2.7-code`、`@cf/zai-org/glm-5.2`、`@cf/zai-org/glm-5.3`、`@cf/zai-org/glm-5.3-flash`、`@cf/deepseek-ai/deepseek-v4-flash-0731`、`@cf/deepseek-ai/deepseek-v4-pro-0813`（[定价](https://developers.cloudflare.com/workers-ai/platform/pricing/)）。
[^12]: 注册接受海外手机号（[注册常见问题](https://docs.bigmodel.cn/cn/faq/registration-login.md)），且对话 API 不要求实名认证：目前调用 API 并不强制要求实名认证（[认证常见问题](https://docs.bigmodel.cn/cn/faq/authentication-issues.md)）。Batch API 则需要实名认证（[Batch API 常见问题](https://docs.bigmodel.cn/cn/faq/batch-api-issues.md)）。同一批免费模型也由国际平台 `https://api.z.ai/api/paas/v4` 提供（[端点](https://docs.z.ai/guides/develop/http/introduction)），其中 GLM-4.7-Flash、GLM-4.5-Flash 与 GLM-4.6V-Flash 均标价为 Free（[定价](https://docs.z.ai/guides/overview/pricing.md)）。Z AI 已宣布 GLM-4.5-Flash 将被停用，其请求会自动路由到 GLM-4.7-Flash（[模型页面](https://docs.bigmodel.cn/cn/guide/models/free/glm-4.5-flash.md)）；所宣布的日期已经过去，而该模型仍在目录中且仍标价为 Free，因此请将该行视为已超期存续、随时可能下线。
[^13]: Mistral 的计划是全局的：每月额度在 Studio、API 与 Vibe Code 之间共享，因此 CLI 用量会消耗同一份预算（[订阅](https://docs.mistral.ai/admin/billing-usage/subscriptions)）。免费模式是新账户的默认设置，无需信用卡（[快速入门](https://docs.mistral.ai/getting-started/quickstarts/studio/activate-and-generate-api-key)），定价页面上的 Free 计划卡片没有列出 API 额度金额（[定价页面](https://mistral.ai/pricing)）。免费模式的输入与输出可能会被用于训练 Mistral 模型，你可以随时选择退出（[数据使用](https://help.mistral.ai/en/articles/347617-do-you-use-my-user-data-to-train-your-artificial-intelligence-models)）。Mistral 不再公布免费额度的具体速率限制数字，而是引导你查看管理面板中的 Limits 页面（[速率限制](https://help.mistral.ai/en/articles/698531-why-am-i-hitting-api-rate-limits-and-how-do-i-increase-them)）；速率限制一列保留的是最后一次公布的数值。
[^14]: 免费赠额仅在使用真实（非 VoIP）手机号完成短信验证后发放，每个号码一份（[计费文档](https://docs.gonkabroker.com/guides/billing-and-deposits/)）。未使用的免费 token 不会结转到下个月。赠额按最贵模型至少 1M token 来计算；更便宜的模型可以用得更多（例如 BGE-M3 约 6M token）（[免费额度页面](https://gonkabroker.com/free-llm-api/)）。仅使用免费额度资金时，请求会被限制在较低速率；当前上限由 `/test-auth` 以 `maxRpm` 返回（[限制](https://docs.gonkabroker.com/reference/limits-and-quotas/)）。
