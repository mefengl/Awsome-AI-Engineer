# Awsome-AI-Engineer
who should be called AI engineer, the creater, or the user?

## Requirements

### Github Copilot Subscription
https://github.com/features/copilot

### OpenAI Acccount 
https://beta.openai.com/

### oh-my-zsh 
https://ohmyz.sh/#install

### Neovim
https://github.com/neovim/neovim/wiki/Installing-Neovim#install-from-package

## CLI

### zsh-autosuggestions 
https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh

### Codex-CLI
https://github.com/microsoft/Codex-CLI/blob/main/Installation.md#zsh-instructions

https://github.com/microsoft/Codex-CLI/blob/main/Installation.md#zsh-instructions

-k can be find in https://beta.openai.com/account/api-keys

-e can be find in https://beta.openai.com/docs/models/codex

-o can be find in https://beta.openai.com/account/org-settings

```bash
git clone https://github.com/microsoft/Codex-CLI.git
cd Codex-CLI
# install the requirements
python -m pip install -r requirements.txt

# setup in zsh
./scripts/zsh_setup.sh -o <org-xxxxxxxxxx> -k <sk-xxxxxxxxxx> -e <code-xxxx-0xx>
```

## VS Code

### Github Copilot
https://marketplace.visualstudio.com/items?itemName=GitHub.copilotvs

### ChatGPT
https://github.com/mpociot/chatgpt-vscode

Not Official, so you need to get the session token by yourself, see https://github.com/mpociot/chatgpt-vscode#obtaining-the-session-token

## Neovim

### Packer
https://github.com/wbthomason/packer.nvim#quickstart

### Github Copilot
https://github.com/github/copilot.vim

```lua
-- add this in Packer
use 'github/copilot.vim'
```
