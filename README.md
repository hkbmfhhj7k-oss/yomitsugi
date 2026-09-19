# Yomitsugi v0.7 — Shortcut Intake

pixivアプリの共有シートから、iPhoneショートカット経由でYomitsugiへ作品を投げる版です。

## Yomitsugi側
ショートカットから次の形式で開くと自動登録します。

`https://hkbmfhhj7k-oss.github.io/yomitsugi/?intake=共有テキスト`

pixivの共有テキストに含まれるタイトル・作者・URLを既存パーサーで取得します。
pixiv novel IDを使った重複判定も維持します。登録済みなら重複作成せず既存作品を表示します。

## iPhoneショートカット
名前例: `Yomitsugiに追加`

1. 「共有シートに表示」をON
2. 共有入力は「テキスト」と「URL」を許可
3. 「URL」アクションを追加
4. URL欄に以下を作る:
   `https://hkbmfhhj7k-oss.github.io/yomitsugi/?intake=` + URLエンコードした「ショートカットの入力」
5. 「URLを開く」を追加

iOSの表示名はバージョンにより少し異なる場合があります。
共有入力をURLへ安全に埋め込むため、入力は必ずURLエンコードしてください。

## 保存
localStorageキーは従来どおり `yomitsugi.v1` です。
