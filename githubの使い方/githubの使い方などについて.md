# githubの使い方などについて
## 1. 概要〜githubとは〜
GitHubとは、Gitの仕組みを利用して、世界中の人々が自分の作品(プログラムコードやデザインデータなど)を保存、公開できるようにしたウェブサービスの名称。<br>
その名の通り、「Git」の「ハブ：拠点・中心・集まり」という意味である。GitHubは、GitHub社によって運営されており、個人・企業問わず無料で利用が可能。<br>
GitHubに作成されたリポジトリ（保存庫のようなもの）は、基本的にすべて公開されるが、指定したユーザーからしかアクセスができないプライベートなレポジトリを作ったりできる。<br>
また、各プロジェクトにwiki（メモ書き）やタスク管理ツールなど、コラボレーションのための機能も充実しているのが特徴。<br>
※詳細については、[GitHubとは何か](https://www.sejuku.net/blog/7901)参照。<br>
余談として、GitHubには個人向けの他に組織（チーム）でリポジトリ管理するための **「organization」** が存在する。<br>
ここで活用しているサービスは「organization」である。<br>
※詳細については、[Organizationとは](https://tonari-it.com/github-organization/)参照。
## 2. 使い方
### 2-1. 事前準備
  * gitインストール<br>
  →[公式サイト](https://git-scm.com/)よりダウンロード及びインストール
  * エディタのインストール<br>
  →vs codeなど
### 2-2. リポジトリの作成〜削除
2-2-1-1. リポジトリの作成<br>
下記いずれかより実施<br>
  * Overviewより「New」をクリック<br>
  ![Overviewからリポジトリ作成](image/2-2-1-1.create_repository①.jpg)
  * Repositoriesより「New repository」をクリック<br>
  ![Repositoriesよりリポジトリ作成](image/2-2-1-1.create_repository②.jpg)<br>
2-2-1-2. リポジトリ名などの設定<br>
  * Owner: リポジトリ所有者を選択<br>
  1. Repository name: リポジトリの名称<br>
  →あとから変更可能（2-2-1-4）参照
  2. Description: リポジトリの概要(任意)<br>
  3. Public/Private: リポジトリの公開/非公開設定<br>
  4. Initialize this repository with: 予めGitHubがテンプレファイルを用意してくれる(任意)
  ![リポジトリ名などの設定](image/2-2-1-2.create_repository.jpg)
2-2-1-3. セットアップ<br>
※2-2-1-2でREADMEやLICENCEの選択などを行った場合は不要<br>
![セットアップ](image/2-2-1-3.setup.jpg)
2-2-1-4. リポジトリ名変更及び削除<br>
2-2-1-4-1. リポジトリ名変更<br>
![リポジトリ名変更](image/2-2-1-4-1.rename.jpg)<br>
2-2-1-4-2. リポジトリの公開/非公開設定<br>
![リポジトリの公開/非公開設定](image/2-2-1-4-2.cahge_visibility.jpg)<br>
2-2-1-4-3. リポジトリの削除<br>
![リポジトリの削除](image/2-2-1-4-3.delete_repository.jpg)<br>
### 2-3. リポジトリのソース取得〜更新
### 2-4. gitコマンド
