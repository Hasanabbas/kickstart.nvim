# Neovim Plugins Reference

Based on your Kickstart.nvim configuration.

## Plugin Overview

| Plugin | Purpose | Key Bindings | Enabled |
|--------|---------|--------------|---------|
| **lazy.nvim** | Plugin manager | `:Lazy` | ✅ |
| **telescope.nvim** | Fuzzy finder | `<leader>sf` files, `<leader>sg` grep, `<leader>sh` help, `<leader>sk` keymaps | ✅ |
| **nvim-lspconfig** | LSP support | `grn` rename, `gra` code action, `grd` definition, `grr` references | ✅ |
| **mason.nvim** | LSP installer | `:Mason` | ✅ |
| **blink.cmp** | Autocompletion | Tab/Enter to accept, Ctrl+Space for docs | ✅ |
| **conform.nvim** | Autoformatting | `<leader>f` | ✅ |
| **nvim-treesitter** | Syntax highlighting | Automatic | ✅ |
| **tokyonight.nvim** | Color scheme | Tokyo Night | ✅ |
| **which-key.nvim** | Keybind helper | Space + wait | ✅ |
| **mini.nvim** | Surround, ai, statusline | `saiw)` add surround, `sd'` delete | ✅ |
| **gitsigns.nvim** | Git signs | `]c`/`[c` hunk nav | ✅ |
| **fidget.nvim** | LSP loading indicator | Automatic | ✅ |
| **guess-indent.nvim** | Auto-detect indentation | Automatic | ✅ |
| **LuaSnip** | Snippets | Tab to expand | ✅ |
| **neo-tree.nvim** | File explorer | `<leader>e` | ❌ |
| **autopairs.nvim** | Auto-close brackets | Automatic | ❌ |
| **indent-blankline.nvim** | Show indentation | Automatic | ❌ |
| **todo-comments.nvim** | Highlight TODOs | `:TodoTelescope` | ❌ |

## Key Bindings Reference

### General
- `<leader>` = Space
- `<Esc>` in normal mode = Clear search highlights
- `<C-h/j/k/l>` = Navigate between windows
- `<leader>q` = Open diagnostic quickfix list

### Telescope (Fuzzy Finder)
- `<leader>sh` - Search help tags
- `<leader>sk` - Search keymaps
- `<leader>sf` - Search files
- `<leader>ss` - Search Telescope select
- `<leader>sw` - Search current word
- `<leader>sg` - Live grep
- `<leader>sd` - Search diagnostics
- `<leader>sr` - Resume last search
- `<leader>s.` - Search recent files
- `<leader>sc` - Search commands
- `<leader><leader>` - Find existing buffers
- `<leader>/` - Fuzzily search in current buffer
- `<leader>s/` - Grep in open files
- `<leader>sn` - Search Neovim config files

### LSP
- `grn` - Rename symbol
- `gra` - Code action
- `grD` - Go to declaration
- `grd` - Go to definition
- `grr` - Find references
- `gri` - Go to implementation
- `grt` - Go to type definition
- `gO` - Document symbols
- `gW` - Workspace symbols
- `<leader>th` - Toggle inlay hints

### Formatting
- `<leader>f` - Format buffer

### Mini.nvim
- `va)` - Visually select around paren
- `ci'` - Change inside quotes
- `saiw)` - Add surround around word
- `sd'` - Delete surround quotes
- `sr)'` - Replace ) with '

### Git (Gitsigns)
- `]c` / `[c` - Next/previous hunk
- `<leader>gh` - Stage hunk (visual)
- `<leader>gu` - Undo stage hunk

## Disabled Plugins

To enable a plugin, uncomment the corresponding line in `init.lua`:

```lua
require 'kickstart.plugins.neo-tree',  -- File explorer
require 'kickstart.plugins.autopairs', -- Auto-close brackets
require 'kickstart.plugins.indent_line', -- Show indentation
require 'kickstart.plugins.gitsigns', -- Git integration
require 'kickstart.plugins.debug', -- Debugging
require 'kickstart.plugins.lint', -- Linting
```

## Tips

- Run `:Tutor` to learn Neovim basics
- Press `?` in Telescope for help
- Run `:checkhealth` if something breaks
- Run `:Lazy` to manage plugins
- Run `:Mason` to install language servers
