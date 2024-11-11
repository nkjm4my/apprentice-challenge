# GitHub フローに従って開発を進めることができる

GitHub にプッシュをしたことのあるローカルリポジトリ（自分の PC 上のディレクトリ）に移動してください。

## 1. プルリクエストとは

- [x] プルリクエストは何か、何のためにあるかをプログラミング初心者にわかるように説明してください。  

##### プルリクエストとは  
- GitHubなどのGitのホスティングサービスが提供する機能  
- 自分がローカルリポジトリで作業した内容をリモートリポジトリのメインのブランチにマージできるように、他の開発者にレビューを依頼すること

##### 目的  
- 他者の目線でチェックを行うことでミスを防ぐ  
- チーム内での情報の共有 など

## 2. プルリクエストの作成

以下のことを行い、プルリクエストを作成してください。

- [x] 1. ローカル（自分の PC ）で pullrequest ブランチを新規作成し、切り替えてください  
`git checkout -b pullrequest`
- [x] 2. 任意のファイルに変更を行ってください  
`echo "プルリク練習" >> README.md`
- [x] 3. 変更をコミットしてください  
`git add README.md`  
`git commit -m "README.mdにプルリク練習を追記"`
- [x] 4. GitHub に pullrequest というブランチ名で変更をプッシュしてください  
`git push -u origin pullrequest`
- [x] 5. GitHub を開き、pullrequest ブランチから main ブランチへのプルリクエストを作成してください  
- [x] 6. 変更内容を確認し、問題なければ GitHub 上で変更をマージしてください  
- [x] 7. GitHub 上の pullrequest ブランチを削除してください  
## ３. ローカルへのリポートリポジトリの変更内容の取り込み

- [x] ローカルリポジトリのブランチを main ブランチに切り替えてください。  
`git checkout main`

- [x] 次に、リモートリポジトリ（GitHub）の main ブランチの内容をローカルリポジトリの main ブランチに取り込んでください。  
`git fetch origin`  
`git merge origin/main`

- [x] それができたらローカルリポジトリの pullrequest ブランチを削除してください。  
`git branch -d pullrequest`

※開発を行う際はここから1に戻り、この1~2のステップを繰り返します

## 4. GitHub フロー

- [x] [GitHub フロー](https://docs.github.com/ja/get-started/quickstart/github-flow) の公式リファレンスを一読してください。

その上で、今後の開発は GitHub フローに基づいて行ってください。多くの組織における基本的な開発フローは GitHub フローもしくは GitHub フローをベースにしたものになります。今から GitHub フローに慣れていきましょう。
