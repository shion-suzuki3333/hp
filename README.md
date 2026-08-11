# 鈴木 志音 — 個人ページ

埼玉大学大学院の個人ホームページです。研究・参加歴・連絡先を1ページにまとめています。

**公開 URL:** https://shion-suzuki3333.github.io/hp/

## 開発

Node.js 22.12 以上が必要です。

```bash
npm install
npm run dev
```

ローカル確認は通常 `http://localhost:4321` です。GitHub Pages と同じパス（`/hp`）で見る場合は `http://localhost:4321/hp/` を開いてください。

```bash
npm run build   # dist/ に静的ファイルを出力
npm run preview # ビルド結果の確認
```

## 公開

`main` への push で GitHub Actions がビルドし、GitHub Pages に自動デプロイします。

## コンテンツの編集

文言はすべて [`src/content.ts`](src/content.ts) にあります。

| キー | 内容 |
|------|------|
| `profile` | 氏名・所属・メール（`emails`: `{ label, address }`） |
| `research` | 研究テーマと説明 |
| `activities.items` | 参加歴（日付と一文） |
| `contact` | 連絡先セクションの見出し・導入文 |

見た目は [`src/pages/index.astro`](src/pages/index.astro) と [`src/styles/global.css`](src/styles/global.css) です。
