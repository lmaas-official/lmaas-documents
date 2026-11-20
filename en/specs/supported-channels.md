# Available Channels and Supported Data

Last checked: 2026-11-18 (Japanese original)

## Ways to use the AI

| Channel | Used by | Details |
|---|---|---|
| Web chat screen | Users | Talk with the AI in a browser. The screen always shows that you are talking with an AI |
| API | Customer systems | Call the AI from your own systems ([integrations](../docs/integrations.md)) |
| MCP (AI tools) | The AI | The AI connects to external services and internal systems permitted by an administrator |

## Ways to manage

| Channel | Used by | Details |
|---|---|---|
| Admin screens (web) | Administrators | Registering users, choosing AI models, reserving training, permitting external connections, issuing API keys and more |

## Data that can be used for training and reference

| Purpose | What can be used | Notes |
|---|---|---|
| Internal document reference (RAG) | Documents such as PDFs | The AI searches and refers to registered documents |
| Additional training (LoRA) | Text Q&A and passages | Each document is read up to about 2,000 tokens; anything longer is cut off |
| Training Data Creation | Word, Excel, PowerPoint, PDF | Create training data from documents, review it, then use it for additional training and RAG ([ai-features](ai-features.md)) |

Details of supported file formats are provided on the screens available after you sign up.

## Display languages

- The official site, applications and inquiries are available in Japanese and English (English is the default; Japanese is at https://lmaas.io/ja ).
- If the English and Japanese versions of the terms differ, the Japanese version takes precedence.
