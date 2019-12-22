# vim-colors-duochrome

This is a fork of [vim-colors-plain](https://github.com/andreypopp/vim-colors-plain), a minimalistic colorscheme which uses bold to highlight keywords and a
distinguished color for constant literals (string, numbers, tags, etc).

![DuoChrome](/screenshots/duochrome.jpg)

## Purpose

Grey is often used for comments so as to minimize visual noise and allow 
focusing on source code. However, this also tends to obscure comments, 
which is important to well documented programs. 

Choosing a color that 
contrasts well with the background but at the same time allows focus to 
be drawn to either code or comments is the objective of vim-colors-duochrome.

## Deviation

vim-colors-duochrome is a light colorscheme only and differs from 
vim-colors-plain in two distinct but subtle ways:

1. It inherits the light background from [flatwhite-vim](https://github.com/kamwitsta/flatwhite-vim) for a warmer 
   paper tint (versus the blue tint of vim-colors-plain).

2. Comments (and directives) inherit the orange foreground color from 
   [vim-quantum](https://github.com/tyrannicaltoucan/vim-quantum) for a monochromatic contrast to the background.

Hence, duochrome: black monochrome/blue for text and constants, 
and paper/orange for background and comments. 

## Installation & Usage

With [vim-plug](https://github.com/junegunn/vim-plug) you add this to the `.vimrc`:

```
Plug 'sdothum/vim-colors-duochrome'
```

Then:

```
set background=light
colorscheme duochrome
```

## Successor

This colorscheme bundle has been superseded with a significantly tweaked 
(with added dark background) and more fully optimized vim colorscheme 
file for dynamic refreshes (containing optional runtime colorscheme 
parameters).

Why not update this bundle? Well, for the above reasons, as the updated
colorscheme is unconventional in its incorporation of runtime flags 
allowing refreshes to reflect the distraction free mode handling of my 
personal .vimrc configuration. This being said, the updated colorscheme 
should be useable as is, as the colorscheme defaults (flags) are set to 
sane settings, so should behave as expected.

See the associated [.vim 
dotfiles](https://github.com/sdothum/dotfiles/tree/master/vim/.vim), 
notably colors/duochrome.vim, and after/plugin/ui.vim and 
after/plugin/theme.vim for dynamic color rule refreshes and distraction 
free editing.
