# GitHub を使って開発を進めることができる

## 1. リモートリポジトリ

- [x] GitHub 上に新規リポジトリを作成してください。
ac_questを作成

## 2. プッシュ

- [x] ローカルの PC 上に GitHub 上で作成したリポジトリの同じ名前のディレクトリを作成し、そのディレクトリ内に README.md　ファイルを作成してください。
`touch README.md`
- [x] 次に、ローカルリポジトリを新規作成し、変更をステージに追加、コミットしてください。
`git init`
`git add .`
`git commit -m "README.mdを作成"`
- [x] リモートリポジトリを登録してください。そして GitHub に変更をプッシュしてください。
`git remote add origin git@github.com:nkjm4my/ac_quest.git`
`git branch -M main`
`git push -u origin main`
## 3. 追加の変更をプッシュ

- [x] README.md に変更を追加してください。そしてその変更を GitHub にプッシュしてください。
`vi README.md`
`git add .`
`git commit -m "はじめましてを追記"`
`git push`

## 4. クローン

- [x] GitHub 上にある他者が作成したリポジトリを自分の PC 上にクローンしてください。クローン対象は何でも良いです。
フォークしてから`git clone git@github.com:nkjm4my/apprentice-challenge.git`しました

