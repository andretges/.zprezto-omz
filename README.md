# .zprezto-omz
Some oh-my-zsh plugins ported to zprezto

Symlink modules to your .zprezto modules directory:
```zsh
setopt EXTENDED_GLOB
for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto-omz/modules/*; do \
  ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.zprezto/modules/${rcfile:t}"
done
```

And then use them in `.zpreztorc` as usual:
```zsh
zstyle ':prezto:load' pmodule \
  'git-omz' \
  'rails-omz' \
```
