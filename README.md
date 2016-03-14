# .zprezto-omz
Some oh-my-zsh plugins ported to zprezto

To start using oh-my-zsh plugins with zprezto, add this dirty hack to your `.zshrc`:
```
# Source Prezto.
if [[ -s "${ZDOTDIR:-$HOME}/.zprezto/init.zsh" ]]; then
  zstyle ":prezto:module:rails-omz" loaded 'yes'
  zstyle ":prezto:module:git-omz" loaded 'yes'

  source "${ZDOTDIR:-$HOME}/.zprezto/init.zsh"

  source "${ZDOTDIR:-$HOME}/.zprezto-omz/modules/rails-omz/init.zsh"
  source "${ZDOTDIR:-$HOME}/.zprezto-omz/modules/git-omz/init.zsh"
fi
```
