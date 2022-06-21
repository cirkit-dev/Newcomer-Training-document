# Ruby on Railsの環境構築

## 目次

1. [Ubuntuを導入するための準備をしよう(WSLの導入)](#ubuntuを導入するための準備をしようwslの導入)

1. [Ubuntuの導入とアップデート](#ubuntuの導入とアップデート)

1. [Ubuntuに各種ライブラリの導入](#ubuntuに各種ライブラリの導入)

1. [Node.jsの導入](#nodejsの導入)

1. [rbenvの導入とRubyの導入](#rbenvの導入とrubyの導入)

1. [Railsの導入](#railsの導入)

1. [MySQLの導入](#mysqlの導入)

<br>

## Ubuntuを導入するための準備をしよう(WSLの導入)
* WindowsでLinuxSubSystemを有効化しよう

* 開発者モードの有効化をしよう

* Windows Terminalを導入しよう(Windows11にはデフォルトで導入されているらしいので確認してみてなかったら入れてね！)<br>
[Windows Terminalのインストールはここから！](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=ja-jp&gl=JP)

* WSLをアップデートしよう<br>
[Linux カーネル更新プログラム パッケージをダウンロード](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

## Ubuntuの導入とアップデート
* [Ubuntuのインストールはここから](https://apps.microsoft.com/store/detail/ubuntu-on-windows/9NBLGGH4MSV6?hl=ja-jp&gl=JP)

## ここまでのことを1発で行う神コマンド
(注意：前提として、WSL2を使うにはCPUの仮想化支援機能が必要です。PCによっては仮想化支援機能がUEFI/BIOSの初期状態でオフになっていることもあるので、オンになっていることを確認してください。)<br>

1. コマンドプロンプトやPowerShellを管理者権限で起動

1. 以下のコマンドでUbuntu,仮想マシンプラットフォーム,WSL,WSL用Linuxカーネル,GUIアプリサポート,Linuxディストリビューションをインストール
```
wsl --install -d Ubuntu
```


* Ubuntuの初期設定
  * ユーザー名入力（小文字と数字のみ使えます）
  * パスワード入力（見えないのは仕様なので注意）

* データを引っ張ってくるサーバーを変える(通信速度を早くしたい方のみ(任意))
```
sudo sed -i.bak -e "s%http://us.archive.ubuntu.com/ubuntu/%http://ftp.jaist.ac.jp/pub/Linux/ubuntu/%g" /etc/apt/sources.list
```

* ホームディレクトリの設定
  * Ubuntuを起動してpwdと入力する
  * 

## Ubuntuに各種ライブラリの導入

## Node.jsの導入

## rbenvの導入とRubyの導入

## Railsの導入

## MySQLの導入
