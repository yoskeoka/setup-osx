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
fisher install omf/theme-bobthefish
```
