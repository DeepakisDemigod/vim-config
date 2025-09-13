
## My Vim Configuration

![vim with copilot demo](https://raw.githubusercontent.com/DeepakisDemigod/vim-config/refs/heads/master/Screenshot_2025-09-13-17-29-05-85_84d3000e3f4017145260f7618db1d683.jpg)

> By deepakisdemigod

A minimalist, modern, and productive Vim setup focused on web development with features like:

- Language Server Protocol (via CoC)
- Git integration
- File tree explorer
- Code formatting and linting
- GitHub Copilot integration
- Productivity-oriented keybindings

> **Designed for Vim (not Neovim), but mostly compatible with Neovim as well.**

---

## 📁 Installation

1. **Install Vim Plug (Plugin Manager)**

   Run the following command to install [vim-plug](https://github.com/junegunn/vim-plug):

   ```bash
   curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
     https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
   ```

2. **Clone this config**

   Replace your `~/.vimrc` or `~/.config/nvim/init.vim` (if using Neovim) with the provided `init.vim`:

   ```bash
   mkdir -p ~/.config/nvim
   cp init.vim ~/.config/nvim/init.vim
   ```

3. **Install Plugins**

   Launch Vim and run:

   ```
   :PlugInstall
   ```

---

## 📦 Plugins Overview

| Plugin                                    | Purpose                                  |
| ----------------------------------------- | ---------------------------------------- |
| `neoclide/coc.nvim`                       | Language server + autocomplete engine    |
| `scrooloose/nerdtree`                     | File tree explorer                       |
| `Xuyuanp/nerdtree-git-plugin`             | Git integration for NERDTree             |
| `tiagofumo/vim-nerdtree-syntax-highlight` | Adds syntax highlight to NERDTree        |
| `ryanoasis/vim-devicons`                  | Adds file/folder icons                   |
| `airblade/vim-gitgutter`                  | Git diff signs in gutter                 |
| `ctrlpvim/ctrlp.vim`                      | Fuzzy file finder                        |
| `scrooloose/nerdcommenter`                | Easy toggling of comments                |
| `christoomey/vim-tmux-navigator`          | Navigate seamlessly between tmux and Vim |
| `projekt0n/github-nvim-theme`             | GitHub-styled theme                      |
| `github/copilot.vim`                      | GitHub Copilot inline suggestions        |

---

## 🎨 UI & Theme

* Theme: `github_dark_default`
* Statusline integrates CoC status info
* Relative and absolute line numbers enabled

---

## 🛠️ Key Mappings

| Mode          | Mapping           | Action                             |
| ------------- | ----------------- | ---------------------------------- |
| Insert        | `jk`              | Exit to Normal mode                |
| Normal        | `<C-n>`           | Toggle NERDTree                    |
| Visual/Normal | `++`              | Toggle comment using NERDCommenter |
| Normal        | `<A-j>` / `<A-k>` | Move lines down/up                 |
| Insert        | `<A-j>` / `<A-k>` | Move lines down/up (in-place)      |

---

## 🧠 CoC.nvim Configuration

### Installed Extensions

* `coc-snippets`
* `coc-pairs`
* `coc-tsserver`
* `coc-eslint`
* `coc-prettier`
* `coc-json`

### Keybindings

| Mode          | Mapping                  | Action                                         |
| ------------- | ------------------------ | ---------------------------------------------- |
| Insert        | `<Tab>` / `<S-Tab>`      | Navigate autocomplete                          |
| Insert        | `<C-Space>`              | Trigger autocomplete                           |
| Normal        | `gd` / `gi` / `gr`       | Go to definition/implementation/references     |
| Normal        | `[g` / `]g`              | Prev/Next diagnostics                          |
| Normal        | `<F2>`                   | Rename symbol                                  |
| Visual/Normal | `<leader>f`              | Format selected code                           |
| Normal        | `<space>a` to `<space>p` | Open CoC Lists (diagnostics, extensions, etc.) |

### Useful Commands

```vim
:Format         " Format file
:Fold           " Fold code
:OR             " Organize imports
```

---

## 🌳 NERDTree Behavior

* Auto-syncs with open buffer
* Git status and icons enabled
* Ignores `node_modules/` folders
* Toggle with `<C-n>`

---

## 🤖 GitHub Copilot Keybindings

| Mode   | Mapping           | Action                     |
| ------ | ----------------- | -------------------------- |
| Insert | `<C-l>`           | Accept Copilot suggestion  |
| Insert | `<C-]>` / `<C-p>` | Next / Previous suggestion |
| Insert | `<C-o>`           | Dismiss suggestion         |

---

## ✨ Editor Behavior

* Auto-indentation, smart tabs
* Spaces instead of tabs (2 spaces)
* Line numbers + wrapped line navigation with `j`/`k`
* CoC status in the status line
* Autocommands for signature help, formatting, outline sync, and highlights

---

## 🔁 Tmux Navigation

Move between Vim and Tmux panes with standard direction keys:

* `<C-h>` / `<C-j>` / `<C-k>` / `<C-l>`

---

## 🧼 Recommended Tools

To make the most of this config, install:

* `node` (for CoC extensions)
* `eslint`, `prettier`, etc. (via npm)
* `ripgrep` (for faster file search with CtrlP)

---

## 📌 Final Notes

* This config is lightweight and ideal for JavaScript/TypeScript developers.
* Git integration, LSP, and formatting all work out of the box.
* Built with extensibility and ease-of-use in mind.

---

## 🧾 License

This configuration is shared under the [MIT License](https://opensource.org/licenses/MIT). Feel free to modify and use it!

```

---

Let me know if you want to include screenshots, add language-specific tools (e.g., Python or Go), or turn it into a GitHub repository template.
```
