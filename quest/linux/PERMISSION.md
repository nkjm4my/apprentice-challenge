# パーミッションを操作できる

## 1. ファイルのオーナーとグループ

- [x] ホームディレクトリの直下に、README.md という名前の空ファイルを作成してください。  
`touch ~/README.md`

- [x] その上で、README.md ファイルのオーナーとグループを確認してください。  
`ls -l ~/README.md`

## 2. ファイルのパーミッション

- [x] README.md ファイルのパーミッションを確認し、誰に何の権限が付与されているかを説明してください。 
```shell
$ ls -l ~/README.md  
-rw-rw-r-- 1 ec2-user ec2-user 37 11月 13 15:55 /home/ec2-user/README.md
```
#### 与えられている権限
オーナー：読み取り、書き込み  
グループ：読み取り、書き込み  
その他のユーザー：読み取り


## 3. ファイルのパーミッションの設定

README.md ファイルのオーナーに対して、読み取り、書き込み、実行の全ての権限を付与してください。  
`chmod u+rwx ~/README.md`  
（すでにwrは付与されているので`chmod u+x ~/README.md`でも可）

## 4. ディレクトリのパーミッションの設定

ホームディレクトリの直下に、permission という名前の空ディレクトリを作成してください。  
`mkdir ~/permission`

permission ディレクトリのグループに対して、書き込み権限を付与してください。  
`chmod g+w ~/permission`

## 5. スーパーユーザー

スーパーユーザーとして、ホームディレクトリの直下に superuser という名前の空ディレクトリを作成してください。  
`sudo mkdir ~/superuser`

作成後、superuser ディレクトリのオーナーが誰かを確認してください。  
`ls -ld ~/superuser`
（オーナーが`root`になってた）