# fish shell

```sh
brew install fish
```

```sh
sudo vim /etc/shells
# 最終行に以下を追加
# /usr/local/bin/fish
```

```sh
chsh -s /usr/local/bin/fish
curl -Lo ~/.config/fish/functions/fisher.fish --create-dirs git.io/fisher
brew install ghq peco fzf
fisher add yoshiori/fish-peco_select_ghq_repository oh-my-fish/plugin-balias edc/bass oh-my-fish/plugin-peco 0rax/fish-bd
```

install theme.

```sh
fisher add oh-my-fish/theme-bobthefish
```

```sh
vim ~/.config/fish/config.fish
# config.fish の内容を貼り付ける
```

```sh
mkdir ~/.peco
vim ~/.peco/config.json
# 下記のJSONを貼り付ける
```

```json
{
    "InitialFilter": "Fuzzy"
}

```