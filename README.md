# Gitに慣れよう！

## Gitのインストール
1. まずはこのサイトへ
<br><a href="URL" target="_blank" rel="https://git-scm.com/download/win">https://git-scm.com/download/win</a>

1. お使いのWindows環境に合ったインストーラーをダウンロードする<br>（ほとんどの場合 Standalone Installer の 64-bit Git for Windows Setup）
2. インストーラーの指示に従ってインストールする。インストールの詳細は以下のページを参考にしてください（あまり気にしなくてもOK押しまくってれば大丈夫だと思います）
<br><a href="URL" target="_blank" rel="https://sukkiri.jp/technologies/devtools/git/git_win.html">https://sukkiri.jp/technologies/devtools/git/git_win.html</a>
1. 適当なターミナルを立ち上げて、以下のコマンドを叩いてバージョン情報が出ればインストール成功！<br>
`git --version`

## Gitの初期設定
以下のサイトを参考にGitにユーザー名・メールアドレスを登録してください。Global でも Local でもお好きな方で大丈夫です（Localの場合は先に目的のディレクトリで`git init`を行っておく必要があります）。これは記事でも言及されていますが、コミットの情報に必要になってきます。
<br><a href="URL" target="_blank" rel="https://laboradian.com/set-git-user-and-email/">https://laboradian.com/set-git-user-and-email/</a>

## ローカルリポジトリとリモートリポジトリを接続しよう！
ローカルリポジトリ：あなたのPCでのリポジトリ<br>
リモートリポジトリ：GitHub上のリポジトリ
1. PCの適当な場所にGit-testディレクトリを作成する。ディレクトリはリポジトリの名前と一致させる（混乱を防ぐため）
2. ターミナル上で作成したディレクトリに移動する。
3. `git init`を叩く
4. 隠しフォルダの .git が作成されていれば初期化成功！
<br>これでGit-testディレクトリにローカルリポジトリが作成されました
5. 次にローカルリポジトリとリモートリポジトリを紐づけます。以下のコマンドを叩いてください。<br>`git remote add origin https://github.com/s1300104/Git-test.git`
6. 確認のために更に次も叩いてください。
<br>`git remote -v`
<br>URLやらが表示されていれば紐づけ成功！