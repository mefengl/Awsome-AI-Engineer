# Awesome-AI-Engineer

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

### GitHub Copilot CLI

https://www.npmjs.com/package/@githubnext/github-copilot-cli

it need copilot subscription and sign up the waitlist, can use Codex-CLI blow instead

### Codex-CLI

https://github.com/microsoft/Codex-CLI/blob/main/Installation.md#zsh-instructions

-o can be find in https://beta.openai.com/account/org-settings

-k can be find in https://beta.openai.com/account/api-keys

-e can be find in https://beta.openai.com/docs/models/codex

```bash
git clone https://github.com/microsoft/Codex-CLI.git
cd Codex-CLI
# install the requirements
python -m pip install -r requirements.txt

# setup in zsh
./scripts/zsh_setup.sh -o <org-xxxxxxxxxx> -k <sk-xxxxxxxxxx> -e <code-xxxx-0xx>
```

## VS Code

### GitHub Copilot Nightly

https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-nightly

### ChatGPT

https://marketplace.visualstudio.com/items?itemName=gencay.vscode-chatgpt

config:

https://github.com/gencay/vscode-chatgpt#gpt3

`Cmd + Shift + P` and type `Open User Settings (JSON)`,

```json
"chatgpt.method": "GPT3 OpenAI API Key",
// can be created in https://beta.openai.com/account/api-keys
"chatgpt.gpt3.apiKey": "xx-xxxxxxxxxx",
```

## Neovim

### vim-plug

https://github.com/junegunn/vim-plug#neovim

or auto install vim-plug if not exists

```lua
-- [[ ~/.config/nvim/init.lua ]]
vim.cmd([[
let data_dir = has('nvim') ? stdpath('data') . '/site' : '~/.vim'
if empty(glob(data_dir . '/autoload/plug.vim'))
  silent execute '!curl -fLo '.data_dir.'/autoload/plug.vim --create-dirs  https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
  autocmd VimEnter * PlugInstall --sync | source $MYVIMRC
endif
]])
```

### Github Copilot

https://github.com/github/copilot.vim

```lua
-- [[ ~/.config/nvim/init.lua ]]
vim.cmd([[
call plug#begin()
Plug 'github/copilot.vim'
call plug#end()
]])
```

## Browser

### ChatGPT

a tab or tabs of https://chat.openai.com/chat

## Usage

https://github.com/f/awesome-chatgpt-prompts

https://github.com/wuchangming/chatgpt-query-engineer-handbook

## Mac

### Notion

https://www.notion.so/product/ai

### Raycast AI

AI as hotkey

### Bob

https://github.com/yetone/bob-plugin-openai-translator

https://github.com/yetone/bob-plugin-openai-polisher

## Maybe Useful

### VSCode

#### ChatGPT

https://marketplace.visualstudio.com/items?itemName=gencay.vscode-chatgpt

config:

https://github.com/gencay/vscode-chatgpt#gpt3

`Cmd + Shift + P` and type `Open User Settings (JSON)`,

```json
"chatgpt.method": "GPT3 OpenAI API Key",
// can be created in https://beta.openai.com/account/api-keys
"chatgpt.gpt3.apiKey": "xx-xxxxxxxxxx",
```

#### GitHub Copilot Labs

https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-labs

```json
"github.copilot-labs.showBrushesLenses": true,
"github.copilot-labs.showTestGenerationLenses": true,
```
