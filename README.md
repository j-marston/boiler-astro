[![Astro](https://img.shields.io/badge/Astro-BC52EE?logo=astro&logoColor=fff)](https://astro.build/)

# About

Astro 構築で使用するボイラーテンプレート

## Tech Stack

| stack | version |
| --- | --- |
| Astro | 7.3.4 |
| eslint | 10.11.0 |
| eslint-plugin-astro | 3.2.1 |
| eslint-plugin-jsx-a11y | 6.10.2 |
| prettier | 3.9.8 |
| prettier-plugin-astro | 1.0.1 |
| stylelint | 2.0.0 |

## Getting Started

ローカル開発：

```sh
pnpm dev
```

URL: [http://localhost:4321](http://localhost:4321)

## Project Structure

```text
/
├── public/
│   └── 加工なしでそのまま配信される静的ファイル (robots.txt, favicon etc.)
├── src/
│   ├── assets/       ※慣例名。importするとビルドで最適化・ハッシュ付与される (image etc.)
│   ├── components/   ※慣例名。再利用するUIコンポーネント (.astro / React etc.)
│   ├── layouts/      ※慣例名。<slot /> でページを包むレイアウトコンポーネント
│   ├── pages/        ※必須。ファイルがそのままURLになる (file-based routing)
│   └── styles/       ※慣例名。グローバルCSSなど
├── astro.config.mjs  Astro設定ファイル
├── tsconfig.json     TypeScript設定ファイル
└── package.json      パッケージ情報・スクリプト定義
```
* /src/content/: Markdown, MDX などファイルを格納する場所として実装する場合もあり

[our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## Commands

| Command | Action |
| :--- | :--- |
| `pnpm dev`| 開発サーバー起動 |
| `pnpm build`| ビルド |
| `pnpm preview`| プレビュー |
| `pnpm astro ...`| Astro CLI コマンド実行 |
| `pnpm astro -- --help`| Astro CLI ヘルプ |
| `pnpm lint` | リンターを実行 |
| `pnpm lint:fix` | リンターを実行して修正を適用 |
| `pnpm fmt` | フォーマッターを実行 |

## Learn More

[our documentation](https://docs.astro.build)
[Discord server](https://astro.build/chat).
