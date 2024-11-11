# ブランチを利用して開発を進めることができる

Git で管理されているディレクトリに移動してください。

## 1. ブランチの新規作成

- [x] feature という名前のブランチを新規作成してください。  
`git branch feature`

## 2. ブランチの切り替え

- [x] ローカルリポジトリのブランチを feature ブランチに切り替えてください。  
`git checkout feature`

## 3. マージ

- [x] feature ブランチでファイルの変更を行い、コミットしてください。そしてローカルリポジトリのブランチを main ブランチに切り替えてください。  
`echo "featureブランチを新規作成" >> README.md`  
`git add README.md`  
`git commit -m "featureブランチを作成した旨をREADME.mdに追記"`  
`git checkout main`

- [x] 次に、feature ブランチの変更を main ブランチに取り込んでください。なお、他のブランチの変更を取り込むことをマージと言います。  
`git merge feature`

## 4. ブランチの名前の変更

- [x] feature ブランチの名前を rename という名前に変更してください。  
`git branch -m feature rename`

## 5. ブランチの削除

- [x] rename ブランチを削除してください。  
`git branch -d rename`  
