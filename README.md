# brew
list of tools that brew install

## tools

### start here

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install --cask iterm2
```

### aws
```bash
brew install awscli
brew install aws-iam-authenticator
```

### docker
```bash
brew install --cask docker
brew install bash-completion
brew install docker-completion
brew install docker-compose-completion
brew install docker-machine-completion
```

### k8s
```bash

brew install kubectl # don't forget to install other stuff https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/#install-with-homebrew-on-macos

brew install helm
brew install helmfile
brew install kustomize

brew install kind
brew install tilt-dev/tap/tilt
brew install derailed/k9s/k9s

# kubeval
brew tap instrumenta/instrumenta
brew install kubeval

```

### python

TODO there is more setup needed here ... like setting up veritual env
```bash
brew install python
brew install pyenv
brew install pyenv-virtualenv
```

### other

```bash
brew install jq
brew install htop
brew install tree
brew install starship
brew install insomnia
brew install --cask dropbox
# screen saver
brew install --cask aerial
# windows snap
brew install --cask rectangle
brew install --cask brave-browser
brew install --cask slack 
brew install pwsafe
```

### all done
```bash
brew cleanup
```
