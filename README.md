# vim-sidescroll

A Vim plugin that provides a horizontal scrolling mode for easier navigation of wide lines.

## Installation

Use your favorite Vim plugin manager.

### With vim-plug

```vim
Plug 'pirey/vim-sidescroll'
```

Then run `:PlugInstall`.

### With lazy.nvim (for Neovim)

```lua
{
  'pirey/vim-sidescroll',
}
```

### With vim.pack

```lua
vim.pack.add({ 'https://github.com/pirey/vim-sidescroll' })
```

## Usage

Enter horizontal scroll mode by pressing `zl` or `zh` (zh is silent).

In scroll mode:

- `l` / `h`: scroll right/left by one column
- `L` / `H`: scroll right/left by half screen width
- `q` or `<Esc>`: exit scroll mode

## Configuration

You can customize the keybindings by setting global variables in your vimrc:

```vim
let g:sidescroll_right_key = 'l'
let g:sidescroll_left_key = 'h'
let g:sidescroll_right_big_key = 'L'
let g:sidescroll_left_big_key = 'H'
let g:sidescroll_quit_key = 'q'
let g:sidescroll_escape_key = '<Esc>'
```

## License

MIT