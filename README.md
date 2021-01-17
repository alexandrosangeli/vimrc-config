# Introduction
This is my .vimrc configuration. I recently started devoting time to familiarise myself with it as it came to my understanding that investing a few days or weeks learning vim will save me a huge amount of time later on.

The configuration is nothing fancy but it does make vim extremely more useful than how it is out of the box. See below for an explanation of what does each line do.

# Walkthrough
- `syntax on` highlights syntax (works for most languages).
- `set noerrorbells` disables sound effects (e.g. when you you press `backspace` in an empty file).
- `set tabstop=4 softtabstop=4` defines tab as four characters long and when `tab` is pressed in insert mode it's 4 spaces long.
- `set shiftwidth=4` characters are shifted by 4 characters.
- `set expandtab` converts tabs to spaces.
- `set smartindent` will (try to) automatically indent.
- `set nu` adds **l**ine n**u**mbers.
- `set wrap` when the line goes off the screen, it goes to the next line (it does **not** create a new line though).
- `set smartcase` makes case-sensitive searching when a capital letter is entered.
- `set noswapfile` doesn't create swap files.
- `set nobackup` doesn't allow backup.
- `set undodir <directory>` sets in which directory an undo file will be created in (see next line).
- `set undofile` creates a file that preserves changes (preserves a history even after a file is closed).
- `set incsearch` makes incremental search (searches as you type).
- `set clipboard=unamedplus` it does copy/pasting to/from the system clipbaord.
- `set colorcolumn=80` indicator is set at the position of the 80th character (see below for personalisation).
- `highlight ColorColumn ctermbg=0 guibg=lightgrey`

### Note
- The configuration is inspired from ThePrimeagen's.
- In order for vim to support copying and pasting to/from the system clipbaord, your vim version needs to support this functionality. To check, enter `$ vim --version` and check for `+clipbaord`. If there's a `-` instead of `+`, then it doesn't. ([solution](https://stackoverflow.com/questions/3961859/how-to-copy-to-clipboard-in-vim/65742440#65742440)).
