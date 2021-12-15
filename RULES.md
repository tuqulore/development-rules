# ルール

## CI/CD

.github/workflows 配下で以下の設定を行っています

### ベースブランチへの CI/CD

- 本番環境への配信

### プルリクエストへの CI/CD

- jest のようなテストツールによるコードテスト
- eslint のようなリンティングツールによるコードチェック
- prettier のようなフォーマッターによるコード整形
- ステージングプレビュー環境への配信

## ブランチ保護

プルリクエスト時に以下のルールを適用します

- CI をパスしなければマージができない
- 自分自身でマージせずに、レビュアーからの承認（Approve）を受けて始めてマージができる

## 開発フロー

基本的には[GitHub flow](https://docs.github.com/ja/get-started/quickstart/github-flow)を採用しています

### ブランチ

- main もしくは master ブランチがベースブランチである
- 場合によっては一時的に develop ブランチをベースブランチとすることがある

### 着手表明

1. [カンバン](https://github.com/orgs/tuqulore/projects/2/views/1)の「やる」カラムをチェックする
2. 優先度の高い issue のうち着手可能なものを[自分自身にアサイン](https://docs.github.com/ja/issues/tracking-your-work-with-issues/assigning-issues-and-pull-requests-to-other-github-users)する
3. 着手した issue を「やっている」カラムに移動する

### Pull Request での作業

1. 作業内容を Pull Request として提出して[レビューをリクエスト](https://docs.github.com/ja/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review)する
2. [レビュー](https://docs.github.com/ja/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)を受ける
3. マージの承認を得られたら自分でマージする

### Issue での作業

1. issue に進捗をコメント、完了する
2. 社内ミーティングで確認する

## タスク管理

[カンバン](https://github.com/orgs/tuqulore/projects/2/views/1)を中心として優先度の設定、進捗の管理をおこなっています

## コミットメッセージ

基本的には[Conventional Commits](https://www.conventionalcommits.org/ja/v1.0.0/)を採用しています
