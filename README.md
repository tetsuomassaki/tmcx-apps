# tmcx-apps

TMCX アプリサポートサイト
https://tetsuomassaki.github.io/tmcx-apps/

## URL設計

```
/                          ← トップ（全アプリ一覧）
/privacy-policy/           ← 共通プライバシーポリシー（全アプリ共有・変更不要）
/<app-name>/               ← アプリ紹介ページ
/<app-name>/support/       ← アプリサポート（FAQ・お問い合わせ）
/<app-name>/appstore.html  ← App Store へ誘導（公開後にリダイレクト）
/<app-name>/playstore.html ← Google Play へ誘導（公開後にリダイレクト）
```

## 申請時に使うURL

| 申請項目 | URL |
|---------|-----|
| プライバシーポリシー | `https://tetsuomassaki.github.io/tmcx-apps/privacy-policy/` |
| サポート (per app) | `https://tetsuomassaki.github.io/tmcx-apps/<app-name>/support/` |

## 新しいアプリを追加する手順

1. `shashinsend/` をコピーして `<new-app>/` にリネーム
2. 各HTMLの内容をアプリに合わせて編集
3. `icon.png` を差し替え
4. `index.html`（トップ）にカードを追加
5. ストア公開後に `appstore.html` / `playstore.html` のリダイレクトURLを有効化

## 現在のアプリ

- **ShashinSend** - WebDAV写真送信アプリ (`/shashinsend/`)
