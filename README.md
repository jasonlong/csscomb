This is a customized version of csscomb. I'm using the deprecated [PHP version](https://github.com/csscomb/csscomb) because the JS version [doesn't yet handle SCSS indentation](https://github.com/csscomb/csscomb.js/issues/163) properly. I've also hardcoded the default sort order with what we use at GitHub (which, in turn, was pulled from Bootstrap).

I use this to sort my CSS rules in Vim with this keybinding:

````
nnoremap <leader>c :silent !php ~/dev/csscomb/csscomb.php -i %<CR>
````
