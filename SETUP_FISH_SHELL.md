# fish shell

```sh
brew install fish
```

```sh
sudo echo '/usr/local/bin/fish' >> /etc/shells
```

```sh
chsh -s /usr/local/bin/fish
curl -Lo ~/.config/fish/functions/fisher.fish --create-dirs git.io/fisher
brew install ghq peco fzf
fisher install ghq yoshiori/fish-peco_select_ghq_repository omf/plugin-balias edc/bass oh-my-fish/plugin-peco 0rax/fish-bd
```

install theme.

```sh
fisher install omf/theme-bobthefish
```
