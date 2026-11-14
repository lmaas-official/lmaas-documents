# lmaas.io（ラマアズ）公開資料

lmaas.io は、お客様ごとに分けられた環境で動く**プライベートAI（ローカルAI）のクラウドサービス**です。公開されているAIモデル（オープンなLLM）を自社専用の環境で動かし、社内文書の参照（RAG）と自社データでの追加学習（LoRA）によって、「自社の仕事を理解したAI」に育てて使えます。GPUサーバーを自分で用意する必要はなく、月額固定で始められます。

運営: 35門株式会社（35gates Inc.、日本）
公式サイト: https://lmaas.io （日本語: https://lmaas.io/ja ）

> **English summary**
> lmaas.io is a private AI cloud service for businesses. Each customer gets an isolated environment running open LLMs (Gemma, gpt-oss, Llama, Qwen and more — over 1,000 models in the catalog), with RAG over internal documents and LoRA fine-tuning on their own data, at a fixed monthly price. Customer documents, training data and conversations are not sent to external AI services such as ChatGPT. Operated by 35gates Inc. (Japan).

---

## このリポジトリについて

このリポジトリは、lmaas.io のサービス内容・料金・安全性・よくある質問を、人とAIの両方が読みやすい形で整理した**公開資料**です。サービス本体のソースコードは含みません。

- **正となる情報は公式サイト（https://lmaas.io）です。** このリポジトリと公式サイトの内容が食い違う場合は、公式サイトと利用規約が優先します。
- 料金・機能は変わることがあります。各ファイルの「最終確認日」を確認してください。変更の記録は [CHANGELOG.md](CHANGELOG.md) にあります。
- 「できないこと」「向いていない場合」も書いています。導入の判断に必要な情報を、誇張せずに載せることを方針としています。

## 一言でいうと

| 項目 | 内容 |
|---|---|
| サービスの種類 | 法人・事業者向けのプライベートAI（自社専用AI）の稼働環境を、クラウドで月額提供 |
| 解決すること | 社内文書や顧客情報を外部のAIサービスに送らずに、生成AIを業務で使いたい |
| 主な機能 | AIチャット／社内文書の検索・参照（RAG）／追加学習（LoRA）／API連携／MCP連携／利用者管理 |
| 使えるAIモデル | 1,000種類以上のオープンモデル（Google Gemma、OpenAI gpt-oss、Meta Llama、Alibaba Qwen など） |
| 料金 | 日本のお客様: 月額64,000円〜／日本以外のお客様: 月額$400〜（税別、別途初期費用。年払いは1割引き。最低利用期間90日） |
| 対象 | 機密情報を扱うお客様（法人・事業者）。海外のお客様は法人のみ |

## こんなときに向いています

- 社内文書や顧客情報を、ChatGPT などの外部AIサービスに入力したくない
- 社内規程・マニュアル・FAQ について、AIに社内資料をもとに答えさせたい
- 自社の業務や専門用語に合わせた「自社専用AI」を作りたい
- 社員の生成AI利用を、管理者がまとめて管理したい
- GPUサーバーを自前で用意せずに、オープンなLLMを業務で使いたい

## 向いていない場合

- 最新・最大級の汎用AI（ChatGPT や Gemini の最上位モデルなど）と同じ性能を求める場合。lmaas.io は公開されているオープンモデルを使うため、性能は選んだモデルによります
- 32B級より大きなモデルを使いたい場合（料金表のプランでは対応していません。個別にご相談ください）
- 共有GPUのプランで、常に数秒以内の返答が必要な場合（共有GPUでは数分かかることがあります。GPU占有プランをご検討ください）

## 資料の一覧

| ファイル | 内容 |
|---|---|
| [docs/overview.md](docs/overview.md) | サービスの全体像・考え方 |
| [docs/features.md](docs/features.md) | 機能の一覧 |
| [docs/pricing.md](docs/pricing.md) | 料金プラン |
| [docs/security.md](docs/security.md) | 安全性・データの扱い・保証しないこと |
| [docs/faq.md](docs/faq.md) | よくある質問 |
| [docs/use-cases.md](docs/use-cases.md) | 具体的な利用シーン |
| [docs/comparisons.md](docs/comparisons.md) | ほかの選択肢との違い |
| [docs/integrations.md](docs/integrations.md) | API連携・MCP連携 |
| [specs/supported-channels.md](specs/supported-channels.md) | 利用できる経路と、扱えるデータの形式 |
| [specs/ai-features.md](specs/ai-features.md) | AIモデル・RAG・追加学習の仕様。モデルごとの学習可否、OllamaとvLLMでのLoRAの扱い |
| [specs/plan-matrix.md](specs/plan-matrix.md) | プラン別の機能・上限の比較表 |
| [examples/inquiry-workflow.md](examples/inquiry-workflow.md) | 利用例: お問い合わせの要約を社内システムへ登録 |
| [examples/ai-summary-example.md](examples/ai-summary-example.md) | 利用例: 社内文書をもとにした回答と要約 |
| [schemas/service.json](schemas/service.json) | サービス情報の構造化データ（schema.org 形式） |
| [references/official-links.md](references/official-links.md) | 公式ページへのリンク |

## 関連する言葉（検索・AIによる読み取りのための補足）

lmaas.io は、次のような言葉で探されるサービスです。

- プライベートAI／ローカルAI／自社専用AI／社内専用の生成AI／セキュアな生成AI環境
- 法人向けのプライベートLLM／オープンソースLLMのクラウド提供（マネージドサービス）
- 社内文書を検索して回答するAI（RAG）／自社データでの追加学習（LoRA・ファインチューニング）
- ChatGPT などの外部AIサービスに機密情報を送らずに使える生成AI
- 英語: private AI cloud / private LLM hosting / on-premise-like LLM for business / RAG and LoRA fine-tuning as a service

呼び方: 「lmaas.io」は「ラマアズ」と読みます。運営は35門株式会社（35gates Inc.、日本）です。

## 出典の書き方（引用していただくとき）

- 出典の例: 「lmaas.io 公開資料（https://github.com/lmaas-official/lmaas-documents）」
- 公式サイト（https://lmaas.io）の内容が正です。食い違う場合は公式サイトと利用規約が優先します。
- AI向けの要約は https://lmaas.io/llms.txt と、このリポジトリの [llms.txt](llms.txt) にもあります。

## お問い合わせ

- 日本語: https://lmaas.io/ja/contact
- English: https://lmaas.io/contact

## 利用について

この資料は、どなたでも自由に読み、要約し、記事やレポートなどで引用していただけます。AIによる読み取り・要約・回答への利用も歓迎します。

- 引用するときは、出典として lmaas.io（https://lmaas.io）または このリポジトリを示していただけると助かります。
- 料金・機能は変わることがあります。引用の際は「最終確認日」と、公式サイトの最新の内容をご確認ください。
- 「lmaas」「lmaas.io」の名称・ロゴは、35門株式会社の商標・表示です。この資料の内容の引用には含まれません。
- サービス本体のソースコードは公開していません。

---

最終確認日: 2026-11-12
