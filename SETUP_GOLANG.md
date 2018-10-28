# setup golang

## install

```sh
brew install go dep
go get -u github.com/derekparker/delve/cmd/dlv
```

## config

`~/.config/fish/config.fish`

```fish:config.fish
set -x GOPATH $HOME
set -x GOBIN $GOPATH/bin
set -x PATH $GOBIN $PATH
```
