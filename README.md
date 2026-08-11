# 大学生個人HP（Astro）

名前・大学・研究・参加歴・連絡先を載せた、1ページ構成の個人サイトです。文言は仮データです。

## 必要な環境

- Node.js 22.12 以上

## 使い方

```bash
npm install
npm run dev
```

ブラウザで表示された URL（通常は `http://localhost:4321`）を開きます。

本番用の静的ファイルを出す場合:

```bash
npm run build
npm run preview
```

## 公開 URL（GitHub Pages）

- https://shion-suzuki3333.github.io/hp/

`main` へ push すると GitHub Actions がビルドして自動公開します。

## 文言の直し方

[`src/content.ts`](src/content.ts) を編集してください。

- `profile` … 氏名・大学・研究室・一言・メール（`emails` に `{ label, address }` を並べる）
- `research` … 研究テーマと説明
- `activities.items` … 「〜に参加しました」形式の参加歴
- `contact` … 連絡先セクションの文言

レイアウトや見た目は [`src/pages/index.astro`](src/pages/index.astro) と [`src/styles/global.css`](src/styles/global.css) です。
