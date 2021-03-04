# Vim Installation & Usage

![screenshot: vim](./screenshots/vim.png)
NeoVim + Tmux with true colors on iTerm2.

## Installation
### Using a plugin manager (recommended)

vim-plug:

```
Plug 'jchassoul/onehalf', { 'rtp': 'vim' }
```

The 'rtp' option is necessary as the vim theme resides in a subdirectory of the git repo.

### Manual Installation
Download the files in [vim/](./) and put them in their respective folders
(`./vim/colors/` and `./vim/autoload/airline/themes/`)

## Usage
Put `colorscheme <scheme>` and `let g:airline_theme='<theme>'`, if using airline
or `let g:lightline = { 'colorscheme': '<theme>' }`, if using lightline, in your `.vimrc`
to set the color scheme and airline (or lightline) theme. Make sure you have
syntax highlighting on, and 256 colors set. Vim version >= 7.4 recommended.

For example:

```
syntax on
set t_Co=256
set cursorline
colorscheme onehalflight
let g:lightline = { 'colorscheme': 'onehalfdark' }
```
