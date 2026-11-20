# Features

Last checked: 2026-11-18 (Japanese original) / Source: https://lmaas.io ("What you can do with lmaas.io" and other features)

## Use AI

| Feature | Details |
|---|---|
| AI chat | Users can use AI in their daily work (writing, summarizing, organizing ideas, research and more) |
| Chatbots and API, ready to use | Prepare chatbots and the APIs used for system integration with a few clicks on the screen |
| Switching inference engines | Switch the mechanism that runs the AI (inference engine) to suit the model you want to use (available on dedicated-GPU plans; see [plan-matrix](../specs/plan-matrix.md) for each plan) |

## Choose AI models

| Feature | Details |
|---|---|
| Over 1,000 models | Use models selected from the AI model hub "Hugging Face" just by choosing them |
| Open models from well-known companies | Google "Gemma", OpenAI "gpt-oss", Meta "Llama", Alibaba "Qwen" and more (open models published by each company) |
| Filter by task and industry | Search by tasks such as "inquiry handling" and "document summarization", or industries such as "healthcare" and "insurance" |
| Usage conditions shown | Each model shows whether "commercial use", "additional training" and "redistribution" are allowed |
| Consent records | Consent to each model's license is recorded together with who consented and when |

## Use internal data (RAG)

| Feature | Details |
|---|---|
| Reference internal documents | Register internal documents such as PDFs, and the AI searches and refers to them when answering. Included in every plan |
| Versioning of reference data | The reference data the AI uses (RAG) is managed by version |
| RAG-only updates | You can also update only the RAG reference data, without additional training |

## Grow your AI (additional training / LoRA)

| Feature | Details |
|---|---|
| Additional training | Train only a small "add-on" (LoRA) without changing the AI model itself. The AI learns to follow the way your registered Q&A and texts answer and are written |
| Training Data Creation | Create training data from Word, Excel, PowerPoint and PDF documents. Choose between "Direct extraction" and "MarkItDown" as the extraction method and compare the results. Check the contents first and use only what you select for training or RAG. Documents are read only inside the service and are never sent to external AI services. It does not use any training runs |
| Simple settings | Just register training data and choose the training strength from "Low", "Standard" and "High". Training runs automatically and you can follow its progress on the screen |
| Versioning of training results | Each version of the AI you have grown is saved. If the results are not what you wanted, you can switch back to a previous version |
| Back to the base model | Stop using the trained version and go back to the base model alone |
| Training history | View the history of training in a list |
| Training while chatting | Training can proceed while the AI is being used in chat. When it finishes, you can use the latest version |
| Training-only mode | On dedicated-GPU plans (Starter Plus, Business Plus), you can switch the server used for chat to training-only mode and train without a limit on the number of runs (it cannot be used for chat or other inference during that time) |

## Connect

| Feature | Details |
|---|---|
| API integration | Call lmaas.io's AI from your own web services and business systems ([integrations](integrations.md)) |
| MCP integration | Let the AI connect to external services and internal systems to gather and summarize the information it needs ([integrations](integrations.md)) |

## Manage

| Feature | Details |
|---|---|
| An environment for each customer | AI environments are separated per customer; the basic design is that they are not mixed with other customers' environments |
| Separation of roles | Only administrators can change settings; users can only use the AI and connections assigned to them |
| Per-user access control | Access from the AI, and the MCP connections to external systems, can be configured for each user |
| External connections by permission | Only administrators register connections to external services, and administrators decide which users can use them |
| Reviewing chat history | On Business and Business Plus, administrators can review all users' conversations (including those via API) for preventing misuse and for audits |
| AI generation records | Each time the AI creates an answer, a signed generation record is created ([security](security.md)) |

## Getting started

- After the service is activated, you can start using your dedicated AI in as little as 10 minutes (a rough guide).
