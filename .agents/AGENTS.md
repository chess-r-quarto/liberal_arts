## 軽量SPA＆Quartoドキュメント・アーキテクチャ (Liberal Arts)

このリポジトリ（`liberal_arts`）でのアプリ開発およびドキュメント作成においては、以下のルールを厳守すること：

1. **完全ビルド不要のフロントエンド (No Build Step)**
   - アプリケーションは `.html` ファイル単体で完結させること。
   - React 18, Babel (Standalone), Tailwind CSS はすべてCDN経由で読み込むこと。
   - `package.json`, `Node.js`, `Webpack`, `Vite` などのビルドツールやパッケージ管理ツールは、ユーザーの明示的な指示がない限り**絶対に導入しない**こと。

2. **ドキュメントのQuarto化と美装 (Quarto Ecosystem)**
   - 公式マニュアルや技術仕様書は、すべて Quarto Markdown (`.qmd`) で記述し、HTMLにレンダリングすること。
   - YAMLフロントマターには `theme: cosmo` および `toc: true` を設定すること。
   - カスタムCSSを用いて、「上質紙に万年筆で書いたような」美装（背景: Solarized Light `#fdf6e3`、文字色: ブルーブラック `#1a2a40`、フォント: `Palatino` 等のセリフ体）を適用すること。

3. **ドキュメントデプロイの自動化**
   - マニュアル（`.qmd`）を作成・更新した後は、ターミナルで `quarto render` を実行し、生成されたHTMLをGitコミットおよびPushするまでのフローをAIが自律的に提案・実行すること（要ユーザー承認）。
