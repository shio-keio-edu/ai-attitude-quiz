# AIへの接し方診断

あなたがAIにどう思われているかを、AI本人がインタビュー形式で診断する全8問のWebクイズ. 結果はタイプ判定＋メーター表示で、画像保存・Xシェアに対応しています。

公開URL: https://shio-keio-edu.github.io/ai-attitude-quiz/

## ファイル構成

| ファイル | 説明 |
|---|---|
| `index.html` | 診断ページ本体（HTML/CSS/JS を1ファイルに内包） |
| `ogp.png` | Xシェア用のOGP画像（1200×630） |

## デプロイ手順（GitHub Pages）

1. このリポジトリを Public で用意し、`index.html` と `ogp.png` をリポジトリ直下に配置する
2. **Settings → Pages** を開く
3. **Source** を `Deploy from a branch` にする
4. **Branch** を `main` / `/(root)` に設定して Save
5. 数分待つと公開URLで閲覧できる

## 公開URLを変える場合

ユーザー名・リポジトリ名を変更したときは、`index.html` 内の以下4か所のURLを実際の公開URLに合わせて書き換える（Xシェア時のサムネイル表示に必要）.

- `og:url`（metaタグ）
- `og:image`（metaタグ）
- `twitter:image`（metaタグ）
- `SITE_URL`（`<script>` 内の定数）
