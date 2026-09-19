# Yomitsugi v0.4 — Rich Records

入口は軽いまま、作品レコードの内部情報を充実させた版です。

## 主な変更
- CORS確認用のpixivテストUIを撤去
- 編集画面を折りたたみ式に拡張
- 「前回まで」「今回起きたこと」「伏線・気になること」
- 登場人物メモ、関係の変化、重要イベント
- お気に入り度、お気に入り箇所、Biblio候補
- 取得履歴 `captures`
- 読書履歴 `readingHistory`
- タグ変更履歴 `tagSnapshots`
- pixiv作品ID等の内部情報を確認可能
- v0.3系までのデータを `yomitsugi.v1` から自動移行

既存の3ファイルをGitHubリポジトリのルートへ上書きしてください。
