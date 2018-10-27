# setup-osx

macOS のセットアップ手順

## ブラウザ

* Google Chrome
* FireFox

## パッケージマネージャ

### brew

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## エディタ

### Visual Studio Code

<https://code.visualstudio.com/Download>

ダウンロードして、zip解凍し `Visual Studio Code.app` をアプリケーションに追加

CMD+SHIFT+P でコマンドパレットを開く

`Shell Command: Install 'code' command in PATH`

## フォント

### source-han-code-jp

```sh
curl -L https://github.com/adobe-fonts/source-han-code-jp/archive/2.000R.tar.gz | tar zx
mv source-han-code-jp-2.000R/OTC/SourceHanCodeJP.ttc ~/library/fonts
rm -r source-han-code-jp-2.000R
```
