e# brew
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
brew install chart-testing
brew install kustomize

brew install kind
brew install minikube
brew install tilt-dev/tap/tilt
brew install derailed/k9s/k9s
brew install kubectx

# kubeval
brew tap instrumenta/instrumenta
brew install kubeval

```

### terraform
```bash
# https://learn.hashicorp.com/tutorials/terraform/install-cli
brew tap hashicorp/tap
brew install hashicorp/tap/terraform
brew install tflint
brew install tfsec
```

### eks
```bash
brew install eksctl
```

### python

TODO there is more setup needed here ... like setting up veritual env
```bash
brew install python
brew install pyenv
brew install pyenv-virtualenv
brew install miniforge
```
#### python exports
```bash
# python
if command -v pyenv 1>/dev/null 2>&1; then
  export PYENV_ROOT="$HOME/.pyenv"
  export PATH="${PYENV_ROOT}/bin:${PATH}"
  eval "$(pyenv init --path)"
  eval "$(pyenv init -)"
fi

alias python=/opt/homebrew/bin/python3
alias pip=/opt/homebrew/bin/pip3
```

### lint
```
pip install yamllint
pip install pylint
pip install pre-commit
brew install shellcheck

pre-commit install
```

### go
```bash
brew install go
```

### unity
```bash
brew install --cask unity-hub
brew install --cask dotnet-sdk
```

### support tools
```bash
brew install git
brew install --cask visual-studio-code
brew install jq
brew install htop
brew install tree
brew install --cask sublime-text
brew install wget
brew install watch
brew install coreutils
```

### other

```bash
# more stuff for starship https://starship.rs/config/#prompt
brew install starship
brew install starship zsh-syntax-highlighting
brew install insomnia
brew install --cask dropbox
# screen saver
brew install --cask aerial
# windows snap
brew install --cask rectangle
brew install --cask brave-browser
brew install --cask slack
brew install --cask zoom
brew install direnv
brew install mkcert
# may not need this one all the time
brew install menumeters
brew vault
```

### crypto
```bash
brew install --cask ipfs
brew install --cask ledger-live
```

### haskell
```bash
brew install cabal-install
```

#### ~/.zshrc
```bash
autoload -Uz compinit
compinit

export EDITOR=vim
source /opt/homebrew/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

eval "$(/opt/homebrew/bin/brew shellenv)"
eval "$(starship init zsh)"
eval "$(direnv hook zsh)"

# k8s
source <(kubectl completion zsh)
alias k=kubectl
compdef __start_kubectl k

curl https://v2.wttr.in
```

### all done
```bash
brew cleanup
```
