### For [vimtex](https://github.com/lervag/vimtex) user

[vimtex](https://github.com/lervag/vimtex) started using its own conceal feature from v2.
Those changes break this plugin for now.
So you should choose vimtex v2 or the latest version v1.6 that tex-conceal works.

```vim
Plug 'lervag/vimtex', {'tag': 'v1.6'}
```

## Options

### Super/sub-scrips

    
To avoid having inscrutable 费解的  utf-8 glyphs appear,
set `g:tex_superscripts` and `g:tex_subscripts`:
```vim
    let g:tex_superscripts= "[0-9a-zA-W.,:;+-<>/()=]"
    let g:tex_subscripts= "[0-9aehijklmnoprstuvx,+-/().]"
```

See `:h tex-conceal` in more detail.

### Fraction

To conceal fraction (½⅓⅔¼⅕⅖⅗⅘⅙⅚⅛⅜⅝⅞)
    let g:tex_conceal_frac =1

## Recommended settings


```vim
set conceallevel=2
let g:tex_conceal="abdgm"
```
```
