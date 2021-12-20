# My Development Environment

My current "dev env" list of tools and commands to install on a mac.
I stole a lot from [here](https://betterprogramming.pub/how-to-set-up-your-macbook-for-web-development-in-2021-a7a1f53f6462). Then added stuff to it.

## Package Management

### Homebrew:


/bin/bash -c “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

Useful commands:
```brew doctor```
``````brew cleanup``````

## Command Line Tools

### Iterm2

Terminal app with nice features over and above the standard terminal.

```brew install --cask iterm2```

### Shell integration

You can enable better integration between your shell and iTerm2.
```iTerm2 > Install Shell Integration```
Then, add the following to your .zshrc
```source ~/.iterm2_shell_integration.zsh```

### zsh

(if not already installed)

```brew install zsh```

### Oh my zsh

Oh My Zsh is a community-driven framework for
managing your Zsh configuration. It provides
hundreds of plugins and themes and makes configuring Zsh a breeze.

```sh -c “$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

We can configure Zsh by running ```vim ~/.zshrc``` or (```open ~/.zshrc``` 
if you prefer TextEdit over Vim). You’ll see a lot of configurations added by Oh My Zsh that you can play with. If you ever need to reset your .zshrc, you can find the template [here](https://github.com/ohmyzsh/ohmyzsh/blob/master/templates/zshrc.zsh-template).

### zsh Theme
Powerlevel10k

```brew install romkatv/powerlevel10k/powerlevel10k```

Install text highlighting
https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md


```p10k configure```

plugins:
https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins

### TLDR Man Pages

Just some extra help pages

```brew install tldr```

## Code Management / Version Control / Collaboration

### GIT

```brew install git```

### Lazy GIT

terminal UI for GIT CLI

```brew install jesseduffield/lazygit/lazygit```

```brew install lazygit```

### Delta
 
Diff viewer for git

```brew install git-delta```

## Containers

### Docker

```brew install --cask docker```

## IDE's

### Visual Studio Code

```brew install --cask visual-studio-code```

## Language / Frameworks

### Node

Javascript framework
```brew install node```

### Python

#### pyenv: manages python more easily (thank doing it yourself)

https://www.freecodecamp.org/news/python-version-on-mac-update/

```brew install pyenv```


```pyenv install 3.10.0```

Macs still use python 2.7, therefore install in...
Installed Python-3.10.0 to /Users/aje/.pyenv/versions/3.10.0

echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc


```echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.zshrc```


## Diagraming / Diagrams as Code

### Structurizr

Diagrams as code tool for C4 diagrams (docker image). There is
also a handy linter on vscode market place search for "structurizr"

https://dev.to/simonbrown/getting-started-with-structurizr-lite-27d0

```docker pull structurizr/lite```
```docker run -it --rm -p 8080:8080 -v [your path - see docs in``` ```link]:/usr/local/structurizr structurizr/lite```

## Image Editing etc.

### Gimp

```brew install --cask gimp```

## Cloud front

## PostgresQL

https://gist.github.com/ibraheem4/ce5ccd3e4d7a65589ce84f2a3b7c23a3

```brew install postgres```

