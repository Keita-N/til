# BSD 系のコマンドを GNU 系に置き換える

```
brew install coreutils
```

~/.bash_profile
```
# use GNU commands
export PATH="$(brew --prefix coreutils)/libexec/gnubin:$PATH"
export MANPATH="$(brew --prefix coreutils)/libexec/gnuman:${MANPATH}"

# add color to ls
alias ll="ls -l --color=auto"
alias ls="ls --color=auto"
```

### 参考
- https://www.topbug.net/blog/2013/04/14/install-and-use-gnu-command-line-tools-in-mac-os-x/
