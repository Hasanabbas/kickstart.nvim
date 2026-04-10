# Neovim Coding Cheat Sheet

## Navigation

### Basic Movement
| Keys | Action |
|------|--------|
| `h` `j` `k` `l` | Left, Down, Up, Right |
| `w` / `b` | Next/Previous word |
| `e` / `ge` | End of word / Previous word end |
| `0` / `$` | Start/End of line |
| `^` | First non-blank character |
| `{` / `}` | Previous/Next paragraph |
| `gg` / `G` | Start/End of file |
| `Ctrl+o` / `Ctrl+i` | Jump back/forward |
| `Ctrl+u` / `Ctrl+d` | Half page up/down |
| `Ctrl+b` / `Ctrl+f` | Page up/down |

### Go To
| Keys | Action |
|------|--------|
| `gd` | Go to definition (LSP) |
| `gD` | Go to declaration |
| `gr` | Find references |
| `gi` | Go to implementation |
| `gt` | Go to type definition |
| `%` | Jump to matching bracket |
| `gf` | Go to file under cursor |

## Editing

### Basic Editing
| Keys | Action |
|------|--------|
| `i` / `a` | Insert before/after cursor |
| `I` / `A` | Insert at start/end of line |
| `o` / `O` | New line below/above |
| `x` | Delete character |
| `dd` / `cc` | Delete/Change entire line |
| `yy` / `p` | Yank (copy)/Paste |
| `u` / `Ctrl+r` | Undo/Redo |
| `.` | Repeat last command |
| `~` | Toggle case |
| `gUU` / `guu` | Upper/Lowercase line |
| `>>` / `<<` | Indent/Unindent |
| `==` | Auto-indent line |

### Text Objects
| Keys | Action |
|------|--------|
| `viw` | Select inside word |
| `vaw` | Select around word |
| `vi)` / `va)` | Inside/Around parentheses |
| `vi"` / `va"` | Inside/Around quotes |
| `ciw` | Change inner word |
| `ci"` | Change inside quotes |
| `dap` | Delete entire paragraph |
| `yi{` | Yank inside braces |

### Surround (mini.nvim)
| Keys | Action |
|------|--------|
| `saiw)` | Add () around word |
| `saiw"` | Add "" around word |
| `saiw[` | Add [] around word |
| `sd'` | Delete quotes |
| `sr)'` | Replace ' with ) |

## Search & Replace

| Keys | Action |
|------|--------|
| `/` | Search forward |
| `?` | Search backward |
| `n` / `N` | Next/Previous match |
| `*` | Search word under cursor |
| `:%s/old/new/g` | Replace all |
| `:%s/old/new/gc` | Replace with confirm |
| `:s/old/new` | Replace in line |

## Buffers

| Keys | Action |
|------|--------|
| `:e filename` | Open file |
| `:w` | Save |
| `:q` / `:qa` | Close/Close all |
| `:wa` | Save all |
| `<leader><leader>` | Find buffer (Telescope) |
| `:bn` / `:bp` | Next/Previous buffer |
| `:bd` | Delete buffer |

## Windows

| Keys | Action |
|------|--------|
| `:sp` / `:vsp` | Split horizontal/vertical |
| `<C-h/j/k/l>` | Navigate windows |
| `<C-w>w` | Cycle windows |
| `<C-w>r` | Swap windows |
| `<C-w>_` | Maximize height |
| `<C-w>\|` | Maximize width |
| `:close` | Close window |

## Tabs

| Keys | Action |
|------|--------|
| `:tabnew` | New tab |
| `:tabnext` / `:tabprev` | Next/Previous tab |
| `gt` / `gT` | Next/Previous tab |
| `:tabclose` | Close tab |

## Telescope (Fuzzy Finder)

| Keys | Action |
|------|--------|
| `<leader>sf` | Find files |
| `<leader>sg` | Grep (search text) |
| `<leader>sh` | Search help tags |
| `<leader>sk` | Search keymaps |
| `<leader>sw` | Search current word |
| `<leader>sd` | Search diagnostics |
| `<leader>sr` | Resume search |
| `<leader>s.` | Recent files |
| `<leader>sc` | Search commands |
| `<leader>sn` | Search Neovim config |
| `<leader>/` | Search in buffer |
| `?` | Show keybindings (in Telescope) |
| `Ctrl+n/p` | Next/Previous item |
| `Enter` | Open selection |
| `Ctrl+u` | Multi-select (up) |
| `Ctrl+d` | Multi-select (down) |

## LSP

| Keys | Action |
|------|--------|
| `grn` | Rename symbol |
| `gra` | Code action |
| `gd` | Go to definition |
| `gr` | Find references |
| `gi` | Go to implementation |
| `K` | Hover documentation |
| `<leader>th` | Toggle inlay hints |
| `[d` / `]d` | Previous/Next diagnostic |
| `<leader>q` | Open quickfix list |

## Git

### Gitsigns
| Keys | Action |
|------|--------|
| `]c` / `[c` | Next/Previous hunk |
| `<leader>ghs` | Stage hunk |
| `<leader>ghu` | Undo stage hunk |
| `<leader>ghp` | Preview hunk |
| `<leader>ghb` | Blame line |

### General
| Keys | Action |
|------|--------|
| `:G` | Open lazygit (if installed) |
| `<leader>gg` | Open lazygit (Telescope) |

## Code Actions

| Keys | Action |
|------|--------|
| `<leader>f` | Format buffer |
| `<leader>a` | Show available actions |
| `Tab` (in completion) | Accept suggestion |
| `Ctrl+Space` | Show completion menu |
| `Ctrl+e` | Cancel completion |
| `Ctrl+k` | Toggle signature help |

## Fold

| Keys | Action |
|------|--------|
| `zc` / `zC` | Close fold / all |
| `zo` / `zO` | Open fold / all |
| `za` | Toggle fold |
| `zM` / `zR` | Close/Open all folds |
| `zk` / `zj` | Previous/Next fold |

## Visual Mode

| Keys | Action |
|------|--------|
| `v` | Enter visual mode |
| `V` | Visual line mode |
| `Ctrl+v` | Visual block mode |
| `o` | Go to other end |
| `gv` | Reselect last |
| `J` / `K` | Move line down/up |
| `<` / `>` | Indent |
| `y` | Yank |
| `p` | Paste |
| `u` / `U` | Lower/Uppercase |

## Miscellaneous

| Keys | Action |
|------|--------|
| `<Esc>` | Clear search highlight |
| `:` | Command mode |
| `Ctrl+]` | Jump to tag |
| `:make` | Run make |
| `:!cmd` | Run shell command |
| `Ctrl+v` + `i` | Insert mode (from normal) |
| `Ctrl+c` | Exit insert (like Esc) |
| `Ctrl+a` / `Ctrl+x` | Increment/Decrement number |
| `qa` | Record macro `a` |
| `@a` | Play macro `a` |
| `@@` | Repeat macro |

## Tips

- Prepend a count: `3w` = move 3 words, `5dd` = delete 5 lines
- `:` + `Up/Down` = Navigate command history
- `/` + `Up/Down` = Navigate search history
- `:help [topic]` = Get help
- `:checkhealth` = Debug issues
- `<C-r>"` = Paste from register in insert mode
