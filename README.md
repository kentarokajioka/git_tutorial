# Gitの勉強
- Gitの仕組み
    - 記録の仕方：スナップショットで記録している。
    - できること：バージョン管理ができる。
    - リポジトリとは：コードの履歴を管理している場所。

- pushする前にすること
    - 認証用のトークンを準備
        - github > setting > developper setting > Personal access tokes > 全選択で発行
        - トークンパスはsecret.jsonに保存した
    - リポジトリの作成
        - Repository > New > public
    - pushする際
        - パスワードはトークンを記載すればよい

- Udemy
    [Gitの流れ](./_img/udemy1.jpg)
    [Gitのエリア](./_img/udemy2.jpg)
    [コミットまでの流れ](./_img/udemy3.jpg)
    [新しいファイルを追加した時](./_img/udemy4.jpg)
    [ファイルを変更した時](./_img/udemy5.jpg)
    [gitクローン](./_img/udemy6.jpg)
    [git add](./_img/udemy7.jpg)
    [git commit](./_img/udemy8.jpg)
    [git status](./_img/udemy9.jpg)

- コマンド一覧
    - git init : gitにアップするフォルダに.gitファイルを作成する。
    - git clone <githubのURL> : リモートリポジトリからコピーを作成する。
    - git add <ファイル名> : ステージアップするファイルだけ。
    - git commit -v : 変更内容を確認してから、コミットメッセージを打てる。
    - git status : リポジトリとステージの差分、ステージとワークツリーの差分を確認できる。
    - git diff : ワークツリーとステージの変更差分を確認することができる。「--staged」を追記することでステージとリポジトリの差分を確認できる。 
    - git log : 変更履歴の確認。「--oneline」で一行で表示、「-p ファイル名」で指定ファイルの差分確認、「-n <コミット数>」で最近のコミット分だけ確認
    - git rm <ファイル名> : ファイルの削除を記録。「-r <フォルダ名>」、「--cached <ファイル名>」はファイルは残すけどgitからは削除
    - git mv <旧ファイル><新ファイル> : ファイルの移動、ファイル名の変更を記録する。
    - git remote add origin <github URL>: リモートリポジトリを新規追加、pushする前に登録しておく。
    - git push origin master : リモートリポジトリへ送信する。「-u」push -u originとすることで次回以降git pushのみでよくなる。 

- エイリアス（ショートカット）をつける
    - git config --global alias.ci commit
    - git config --global alias.st status
    - git config --global alias.br branch
    - git config --global alias.co checkout