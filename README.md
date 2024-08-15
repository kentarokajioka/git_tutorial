# Gitの勉強
- Gitの仕組み
    - 記録の仕方：スナップショットで記録している。
    - できること：バージョン管理ができる。
    - リポジトリとは：コードの履歴を管理している場所。

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
    [git diff]()

- コマンド一覧
    - git init : gitにアップするフォルダに.gitファイルを作成する。
    - git clone ${githubのURL} : リモートリポジトリからコピーを作成する。
    - git add ${ファイル名} : ステージアップするファイルだけ。
    - git commit -v : 変更内容を確認してから、コミットメッセージを打てる。
    - git status : リポジトリとステージの差分、ステージとワークツリーの差分を確認できる。
    - git diff : ワークツリーとステージの変更差分を確認することができる。「--staged」を追記することでステージとリポジトリの差分を確認できる。 