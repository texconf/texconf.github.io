# texconf.github.io

TeXConfの恒常の入口です。公開URLは <https://texconf.github.io> です。

開催告知、プログラム、参加登録、発表資料は、西暦名の別リポジトリ（例: [`2026`](https://github.com/texconf/2026)）に置きます。このリポジトリ内に`2026/`のような西暦フォルダを作らないでください。GitHub Pagesでは、同じパスに組織サイトのフォルダと年次リポジトリのプロジェクトサイトが重なります。

## GitHub Pagesの公開元

入口ページの`index.html`はCIが生成します。リポジトリに生成物を含めない運用のため、Pagesの公開元は **GitHub Actions**（ワークフロー `Deploy Pages`）にしてください。

[Settings → Pages](https://github.com/texconf/texconf.github.io/settings/pages) の Build and deployment で Source を GitHub Actions に切り替えたあと、`Deploy Pages` を再実行します。公開元が `main` ブランチのままだと、pushのたびにブランチ上のファイルだけが配信され、`index.html` が無いため <https://texconf.github.io/> が404になります（Actionsのビルド自体は成功している場合があります）。
