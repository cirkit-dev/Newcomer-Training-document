# GitのリポジトリをGitHubにあげよう

1. [GitHubでリポジトリを作成しよう](#GitHubでリポジトリを作成しよう)

1. [GitのリポジトリをGitHubにあげよう](#gitのリポジトリをgithubにあげよう)

<br>

## GitHubでリポジトリを作成しよう

* New repositoryをクリック
![NewRepositori](../images/GitHub_NewRepositori.PNG)

* Repository name(リポジトリの名前)とDescription(リポジトリの説明)を記入しよう<br>
* リポジトリの公開設定を決める<br>
  * Publicなら誰でも自由に閲覧＆Pull Requestを立てれる<br>
  * Privateなら自分以外は許可した人しか閲覧＆Pull Requestを立てられない<br>
(Pull Requestとは、「編集リクエスト」のような機能で、こういう修正をしてみたけど、もし良ければ反映して下さい、というものです。)<br>
* その他の設定
  * Add a README file<br>
  READMEファイルを作成するかどうか<br>
  (READMEファイルとは、主に「システムの概要」「ツールの使い方」「インストール方法」などの、リポジトリに格納されたソースコードを利用したり、参照する前に読んでほしい内容を記載するファイル。)<br>
  * Add .gitignore<br>
  .gitignoreファイルを作成するかどうか<br>
  (.gitignoreはGitの管理対象から外すためのルールを記述するファイル)<br>
  * Choose a license<br>
  リポジトリにライセンスを付与するかどうか<br>
  ([詳しくはこちら](https://docs.github.com/ja/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository))
![GitHub_Repository_Setting](../images/GitHub_RepositorySettings.PNG)

<br>

## GitのリポジトリをGitHubにあげよう

GitHubでリポジトリを作成できたら、GitのリポジトリとGitHubのリポジトリを連携させます。
```
git remote add origin https://github.com/ユーザーネーム/リポジトリネーム.git

```

GitのリポジトリをGitHubのリポジトリにプッシュしよう
```
git push -u origin master
```
(git pushのオプション -u とは、ローカルリポジトリの現在のブランチの上流をorigin master に規定することを意味している。<b>すなわち、次からは git push だけで上記のコマンドと同じことを実施できる。さらに、git pull だけでも git pull origin master と同じ意味になる。<b>)
