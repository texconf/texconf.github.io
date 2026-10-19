# texconf.github.io

TeXConfの恒常の入口です。公開URLは <https://texconf.github.io> です。

開催告知、プログラム、参加登録、発表資料は、西暦名の別リポジトリ（例: [`2026`](https://github.com/texconf/2026)）に置きます。このリポジトリ内に`2026/`のような西暦フォルダを作らないでください。GitHub Pagesでは、同じパスに組織サイトのフォルダと年次リポジトリのプロジェクトサイトが重なります。

## GitHub Pagesの公開元

入口ページの`index.html`はCIが生成し、`gh-pages`ブランチへ書き出します（2026年サイトと同じ方式）。`main`には生成物を置きません。

[Settings → Pages](https://github.com/texconf/texconf.github.io/settings/pages) の Build and deployment で次を選びます。

- **Source**: Deploy from a branch
- **Branch**: `gh-pages`、フォルダ `/`（root）

「GitHub Actions」を選ぶ画面に、こちらで使うワークフロー名（Deploy Pages）を指定する項目はありません。ビルドの再実行は、リポジトリの **Actions** タブ → 左の **Deploy Pages** → **Run workflow** です。

公開元が `main` のままだと、`index.html` が無い状態が配信され <https://texconf.github.io/> が404になります。
