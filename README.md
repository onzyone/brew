# brew
list of tools that brew install

## tools

### start here

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install --cask iterm2 
or
brew install --cask wezterm
brew install font-meslo-lg-nerd-font
```

### IDE
```bash
brew install --cask cursor
brew install --cask visual-studio-code
```

### docker
```bash
brew install --cask docker
brew install bash-completion
brew install docker-completion

brew install buildpacks/tap/pack
```

### k8s
```bash

brew install kubectl # don't forget to install other stuff https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/#install-with-homebrew-on-macos

brew install helm
brew install helmfile
brew install chart-testing
brew install kustomize

brew install tilt-dev/tap/tilt
brew install derailed/k9s/k9s
brew install kubectx

# pick your adventure
brew install k3d
brew install kind
brew install minikube

# optional but cool
brew install infra

```

### terraform
```bash
# https://learn.hashicorp.com/tutorials/terraform/install-cli
brew tap hashicorp/tap
brew install hashicorp/tap/terraform
brew install tflint
brew install tfsec
brew install terraform-docs
```

### aws
```bash
brew install awscli
brew install aws-iam-authenticator
brew install eksctl
```

### gcp
```
brew install --cask google-cloud-sdk
```

### Langs
just got with devcontainers.
#### unity
```bash
brew install --cask unity-hub
brew install --cask dotnet-sdk
```

### db tools
```bash
# mongodb
brew install --cask mongodb-compass
```

### support tools
```bash
brew install git
brew install gh
brew install act # github actions local run
brew install jq
brew install yq
brew install htop
brew install tree
brew install --cask sublime-text
brew install wget
brew install watch
brew install coreutils
brew install --cask obsidian
```

### api testing tools
```bash
brew install insomnia
```

### other

```bash
# more stuff for starship https://starship.rs/config/#prompt
brew install starship
brew install starship zsh-syntax-highlighting
brew install --cask dropbox
# screen saver
brew install --cask aerial
# windows snap
brew install --cask rectangle
brew install --cask brave-browser
brew install --cask arc
brew install --cask slack
brew install --cask zoom
brew install direnv
brew install mkcert
# replaces iState
brew install --cask stats
# may not need this one all the time
brew install menumeters
brew install --cask karabiner-elements
```

### crypto
```bash
brew install --cask ipfs
brew install --cask ledger-live
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
