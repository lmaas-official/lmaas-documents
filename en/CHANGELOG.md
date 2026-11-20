# Changelog

This records changes to the documents in this repository. Changes to the pricing or features of the service itself are also recorded here. The Japanese [CHANGELOG](../CHANGELOG.md) is the original.

## 2026-11-20

- Added English versions of all documents under `en/` (README, docs, specs, examples, schemas, references). The Japanese documents in the repository root remain the original.

## 2026-11-18

- Added the new "Training Data Creation" feature (creating training data from Word, Excel, PowerPoint and PDF) (features, faq, specs/ai-features, specs/supported-channels)
- Added the choice and side-by-side comparison of extraction methods (Direct extraction / MarkItDown) (features, specs/ai-features)

## 2026-11-14

- Added "How additional training (LoRA) relates to the AI execution engine for each model" to the AI feature specifications (specs/ai-features.md)
  - Training and replying are separate mechanisms / how LoRA is applied in Ollama and vLLM / which models can and cannot be trained / continuing training from a previous version
- Added this repository's URL (sameAs) to the structured data (schemas/service.json)
- Added "Related terms" and "How to cite" to the README, and added llms.txt (a summary for AI) to the repository root

## 2026-11-12

- Added US dollar pricing for customers outside Japan (pricing, plan-matrix, service.json)
- Added bank transfer as a payment method (customers in Japan only)
- Unified the names of training strength to "Low / Standard / High", matching the screens
- Added the terms of use (free to read, summarize and quote) to the README
- Added the US dollar price for one additional training run ($5, customers outside Japan) (pricing, plan-matrix)
- Added the public repository URL (lmaas-official/lmaas-documents) to the official links
- First public release
  - Service overview, features, pricing (amounts as revised on 2026-11-06), security, FAQ, use cases, comparisons and integrations
  - Plan comparison table, two examples, structured data (schemas/service.json) and official links
