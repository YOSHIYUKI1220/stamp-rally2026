# 🎪 学園祭スタンプラリー

学園祭来場者向けのQRコードスタンプラリーWebアプリです。

## 特徴

- 📱 スマホのブラウザだけで動作（インストール不要）
- 🆓 完全無料（GitHub Pages でホスティング）
- 🔒 HTTPS 対応（カメラアクセスに必須）
- 💾 データはブラウザ内に保存（サーバー不要）

## ファイル構成

```
stamp-rally-package/
├── index.html        # アプリの入口
├── stamp-rally.jsx   # アプリ本体（React）
├── manifest.json     # PWA設定（ホーム画面追加）
├── icon-192.png      # アイコン（任意・差し替え可）
├── icon-512.png      # アイコン（任意・差し替え可）
└── README.md         # このファイル
```

## セットアップ手順

1. このリポジトリをGitHubにアップロード
2. Settings → Pages → main ブランチを公開
3. 発行されたURLをQRコード化して入口に掲示

詳細は付属の **導入マニュアル.docx** を参照してください。

## 管理者パスワード

初期パスワード: `admin2024`

変更する場合は `stamp-rally.jsx` の3行目を編集してください。

```js
const ADMIN_PASSWORD = "admin2024"; // ← ここを変更
```

## QRコードフォーマット

各ブースのQRコードには以下の文字列を埋め込みます：

```
STAMP_RALLY:booth_01
STAMP_RALLY:booth_02
...
STAMP_RALLY:booth_10
```

管理者画面のブースタブから「QR表示」ボタンでQRコードを生成・印刷できます。

## ライセンス

学園祭・文化祭での利用に限り自由に使用できます。
