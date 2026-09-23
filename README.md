# legal-docs

Shimuworks で公開する各アプリのプライバシーポリシーなど、法務系ドキュメントをまとめて GitHub Pages で公開するためのリポジトリ。

## 構成

アプリごとにフォルダを切り、その中にHTML(公開用)とMD(編集用の原本)を置く。

```
legal-docs/
  <アプリのslug>/
    privacy-policy.html   ← 実際に公開されるページ
    privacy-policy.md     ← 編集用の原本(Markdown)
```

公開URLは次の形式になる。

```
https://shimuworks-apps.github.io/legal-docs/<アプリのslug>/privacy-policy.html
```

## 新しいアプリを追加する手順

1. このリポジトリ直下に、アプリの `slug`(app.json の `expo.slug` と揃える)と同名のフォルダを作る
2. `privacy-policy.md` を書き、内容を `privacy-policy.html` にも反映する(スタイルは既存ファイルをコピーして流用)
3. コミット・push すると、GitHub Pages 経由で数分以内に公開される
4. アプリ側の `PRIVACY_POLICY_URL` を上記URL形式に更新する

## GitHub Pages 設定

このリポジトリの Settings → Pages で、ブランチ `main` の `/ (root)` を公開元として設定している。

## 現在公開しているアプリ

| アプリ | slug | URL |
| --- | --- | --- |
| 経過日数トラッカー | elapsed-tracker | https://shimuworks-apps.github.io/legal-docs/elapsed-tracker/privacy-policy.html |
