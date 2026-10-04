# 週間スケジュール（オオサカポテト）

社内用。月曜の週間ミーティングと、生産部・流通部・営業の週間予定を共有する画面。

- 画面：この `index.html`（GitHub Pages で配信）
- データ：Google スプレッドシート「週間スケジュールDB」（Apps Script の API 経由）
- 受発注管理DB は「読むだけ」（受注・シフト・設定）。書き込みはしない
- ログイン：名前＋合言葉（合言葉は Apps Script のスクリプトプロパティで管理。この中には入っていない）

## 更新手順
1. `index.html` を差し替える
2. `git add -A && git commit -m "更新" && git push`
3. 1〜2分で GitHub Pages に反映

API 側（Apps Script）は `~/gas-projects/週間スケジュール` で `clasp push` → 新バージョンをデプロイ。
