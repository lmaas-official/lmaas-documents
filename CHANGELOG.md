# 変更履歴

このリポジトリの資料の変更を記録します。サービスそのものの料金・機能が変わったときも、ここに記録します。

## 2026-11-20

- すべての資料の英語版を `en/` に追加（README・docs・specs・examples・schemas・references）。日本語版（リポジトリ直下）が原本で、食い違う場合は日本語版が優先
- README と llms.txt に英語版への案内を追加

## 2026-11-18

- 新しい機能「AI学習用データ作成」（Word・Excel・PowerPoint・PDF から学習データを作る）を追記（features・faq・specs/ai-features・specs/supported-channels）
- 読み取り方式（直接読み取り・MarkItDown）の選択と見比べを追記（features・specs/ai-features）

## 2026-11-14

- AI機能の仕様（specs/ai-features.md）に「モデルごとの追加学習（LoRA）とAI実行エンジンの関係」を追記
  - 学習と返事を出す仕組みは別であること／Ollama・vLLMでの組み込み方の違い／学習できるモデル・できないモデル／続きからの学習
- 構造化データ（schemas/service.json）に、このリポジトリのURL（sameAs）を追記
- README に「関連する言葉」「出典の書き方」を追記し、AI向けの要約 llms.txt をリポジトリ直下に追加

## 2026-11-12

- 日本以外のお客様向けの米ドル料金を追加（pricing・plan-matrix・service.json）
- お支払い方法に銀行振込（日本のお客様のみ）を追記
- 学習強度の呼び方を画面に合わせて「低・標準・高」に統一
- 利用条件（自由に読み・要約・引用できること）をREADMEに追記
- 追加学習1回の料金に米ドル（$5、日本以外のお客様）を追記（pricing・plan-matrix）
- 公開リポジトリのURL（lmaas-official/lmaas-documents）を公式リンクに追記
- 初版を公開
  - サービス概要・機能・料金（2026-11-06改定の金額）・安全性・よくある質問・利用シーン・比較・連携の資料
  - プラン比較表、利用例2件、構造化データ（schemas/service.json）、公式リンク
