# lmaas.io — Public Documentation (English)

[日本語版はこちら](../README.md)

lmaas.io is a **private AI (local AI) cloud service** that runs in an environment separated for each customer. You run publicly available AI models (open LLMs) in an environment dedicated to your company, and grow them into an "AI that understands your work" by letting them refer to your internal documents (RAG) and training them on your own data (LoRA). There is no need to prepare your own GPU servers, and you can start at a fixed monthly price.

Operated by: 35gates Inc. (35門株式会社, Japan)
Official site: https://lmaas.io (Japanese: https://lmaas.io/ja )

---

## About this repository

This repository is **public documentation** that organizes lmaas.io's services, pricing, security and FAQs in a form that is easy for both people and AI to read. It does not contain the source code of the service itself.

- **The official site (https://lmaas.io) is the authoritative source.** If this repository and the official site differ, the official site and the Terms of Service take precedence.
- Pricing and features may change. Please check the "Last checked" date in each file. Changes are recorded in [CHANGELOG.md](CHANGELOG.md).
- We also describe what lmaas.io **cannot** do and when it is **not a good fit**. Our policy is to provide the information needed to make a decision, without exaggeration.
- The Japanese documents (in the repository root) are the original. If the English and Japanese versions differ, the Japanese version takes precedence.

## In short

| Item | Details |
|---|---|
| Type of service | A cloud environment for running private AI (AI dedicated to your company), provided monthly to businesses |
| Problem it solves | Using generative AI at work without sending internal documents or customer information to external AI services |
| Main features | AI chat / search and reference of internal documents (RAG) / additional training (LoRA) / API integration / MCP integration / user management |
| AI models available | Over 1,000 open models (Google Gemma, OpenAI gpt-oss, Meta Llama, Alibaba Qwen and more) |
| Pricing | Customers outside Japan: from $400/month; customers in Japan: from ¥64,000/month (excluding tax, plus an initial fee. 10% off for annual payment. Minimum term 90 days) |
| Who it is for | Businesses that handle confidential information. Customers outside Japan: businesses only |

## A good fit when you want to

- Avoid entering internal documents or customer information into external AI services such as ChatGPT
- Have AI answer questions about internal rules, manuals and FAQs based on your own documents
- Build an "AI of your own" tuned to your business and terminology
- Let administrators manage how employees use generative AI in one place
- Use open LLMs at work without setting up your own GPU servers

## Not a good fit when

- You need the same performance as the latest and largest general-purpose AI (such as the top models of ChatGPT or Gemini). lmaas.io uses publicly available open models, so performance depends on the model you choose
- You want to use models larger than the 32B class (not covered by the listed plans; please contact us individually)
- On a shared-GPU plan, you always need replies within a few seconds (a shared GPU can sometimes take a few minutes; please consider a dedicated-GPU plan)

## Documents

| File | Contents |
|---|---|
| [docs/overview.md](docs/overview.md) | Overview of the service and its approach |
| [docs/features.md](docs/features.md) | List of features |
| [docs/pricing.md](docs/pricing.md) | Pricing plans |
| [docs/security.md](docs/security.md) | Security, data handling, and what we do not guarantee |
| [docs/faq.md](docs/faq.md) | Frequently asked questions |
| [docs/use-cases.md](docs/use-cases.md) | Concrete use cases |
| [docs/comparisons.md](docs/comparisons.md) | How lmaas.io differs from other options |
| [docs/integrations.md](docs/integrations.md) | API integration and MCP integration |
| [specs/supported-channels.md](specs/supported-channels.md) | Available channels and supported data formats |
| [specs/ai-features.md](specs/ai-features.md) | Specifications of AI models, RAG and additional training, including trainability per model and how LoRA is handled in Ollama and vLLM |
| [specs/plan-matrix.md](specs/plan-matrix.md) | Comparison of features and limits by plan |
| [examples/inquiry-workflow.md](examples/inquiry-workflow.md) | Example: registering summaries of inquiries in an internal system |
| [examples/ai-summary-example.md](examples/ai-summary-example.md) | Example: answers and summaries based on internal documents |
| [schemas/service.json](schemas/service.json) | Structured data about the service (schema.org) |
| [references/official-links.md](references/official-links.md) | Links to official pages |

## Related terms (for search and AI reading)

lmaas.io is a service people look for with terms such as:

- private AI / local AI / company-dedicated AI / secure generative AI environment for businesses
- private LLM hosting for businesses / managed cloud hosting of open-source LLMs
- AI that answers by searching internal documents (RAG) / fine-tuning on your own data (LoRA)
- generative AI you can use without sending confidential information to external AI services such as ChatGPT
- on-premise-like LLM for business / RAG and LoRA fine-tuning as a service

Name: in Japanese, "lmaas.io" is read "ラマアズ". It is operated by 35gates Inc. (Japan).

## How to cite

- Example: "lmaas.io public documentation (https://github.com/lmaas-official/lmaas-documents)"
- The official site (https://lmaas.io) is authoritative. If they differ, the official site and the Terms of Service take precedence.
- A summary for AI is also available at https://lmaas.io/llms.txt and in this repository's [llms.txt](../llms.txt).

## Contact

- English: https://lmaas.io/contact
- Japanese: https://lmaas.io/ja/contact

## Terms of use for these documents

Anyone may freely read, summarize and quote these documents in articles, reports and so on. Reading, summarizing and answering with these documents by AI is also welcome.

- When quoting, we would appreciate it if you cite lmaas.io (https://lmaas.io) or this repository as the source.
- Pricing and features may change. When quoting, please check the "Last checked" date and the latest information on the official site.
- The names and logos "lmaas" and "lmaas.io" are trademarks / marks of 35gates Inc. and are not included in the permission to quote this content.
- The source code of the service itself is not public.

---

Last checked: 2026-11-20 (translated from the Japanese version last checked 2026-11-12)
