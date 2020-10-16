# setup-osx

macOS のセットアップ手順

## ブラウザ

* Google Chrome
* FireFox

## XCode

App Store から XCodeを入手する。

macOSをバージョンアップした場合、
XCode Command Line Tools の再インストールが必要となるので、以下でインストールする。
(Catalinaからはインストール失敗して、Macのソフトウェア・アップデートからインストールすることになる？）

```sh
xcode-select --install
```



## パッケージマネージャ

### brew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## python

```sh
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py --user
```

## ruby

```sh
brew install rbenv
```

## go

```sh
brew install go dep
mkdir ~/src ~/bin
```

## node

[Node セットアップ手順](./SETUP_NODE.md)

## フォント

### source-han-code-jp

```sh
curl -L https://github.com/adobe-fonts/source-han-code-jp/archive/2.000R.tar.gz | tar zx
mv source-han-code-jp-2.000R/OTC/SourceHanCodeJP.ttc ~/library/fonts
rm -r source-han-code-jp-2.000R
```

```sh
brew tap homebrew/cask-fonts
brew cask install font-source-han-code-jp
```

### powerline

```sh
git clone https://github.com/powerline/fonts.git
cd fonts
./install.sh
```

## fish shell

[fish shellセットアップ手順](./SETUP_FISH_SHELL.md)

## terminal

### iTerm2

<https://www.iterm2.com/downloads.html>

```sh
mkdir ~/.iterm2/
```

![preference](./images/iterm2preference.png)

`com.googlecode.iterm2.plist` ファイルを置き換える。

### colorrc

`.colorrc` の内容を `~/.colorrc` ファイルに保存。

## git user

```sh
git config --global user.name yoskeoka
git config --global user.email y.okamoto@gemcook.com
```

## エディタ

### Visual Studio Code

<https://code.visualstudio.com/Download>

ダウンロードして、zip解凍し `Visual Studio Code.app` をアプリケーションに追加

⌘+SHIFT+P でコマンドパレットを開く

`Shell Command: Install 'code' command in PATH`

設定をjson編集モードで開き、 `vscode-settings.json` の内容を貼り付ける。

`install-vscode-extentions.sh` を実行して拡張をまとめてインストール。

## command line tools

```sh
brew install jid jo jq colordiff ghq coreutils
```

```sh
git config --global ghq.root '~/src'
```

```sh
pip install awscli --user
```

## Docker & Kubernetes

[Docker for mac](https://docs.docker.com/docker-for-mac/install/)

```sh
brew install kubectx
gofish install helm
```

## GUI tools

```sh
brew cask install copyq
```

## mac setting

⌘+SHIFT+3 or ⌘+SHIFT+3 のスクリーンショットの保存先変更。

```sh
defaults write com.apple.screencapture location ~/Pictures/
killall SystemUIServer
```
