# Awesome-AI-Engineer

Who should be called AI engineer, the creater, or the user?

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

It need copilot subscription and sign up the waitlist, can use Codex-CLI blow instead

## VS Code

Packed below extensions in [AI Pack](https://marketplace.visualstudio.com/items?itemName=mefengl.vscode-ai-pack)

### GitHub Copilot

https://marketplace.visualstudio.com/items?itemName=GitHub.copilot

### GitHub Copilot Chat

https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat

### I Don't Care About Commit Message

https://marketplace.visualstudio.com/items?itemName=mefengl.vscode-i-dont-care-about-commit-message

repo: https://github.com/mefengl/vscode-i-dont-care-about-commit-message

### Copy Folder Content

https://marketplace.visualstudio.com/items?itemName=mefengl.copy-folder-content

repo: https://github.com/mefengl/vscode-copy-folder-content

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

#### Scripts

https://greasyfork.org/scripts/462713-chat-octopus , one prompt, three ai models answer for you

### Extension

https://github.com/anaclumos/bing-chat-for-all-browsers , to use Bing Chat in other browsers

## Usage

https://github.com/f/awesome-chatgpt-prompts

https://github.com/wuchangming/chatgpt-query-engineer-handbook

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

### Mac

#### Cursor

https://www.cursor.so/

#### Notion

https://www.notion.so/product/ai

#### Raycast AI

https://www.raycast.com/ai

AaaH! AI as a Hotkey

### CLI

#### Codex-CLI

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

#### opencommit

https://github.com/di-sukharev/opencommit
