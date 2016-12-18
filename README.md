# NERD Commenter

## Installation

For initial instructions, check out the original script at
[https://github.com/scrooloose/nerdcommenter](https://github.com/scrooloose/nerdcommenter)

## Configuration

Suggested mappings to be put in the vimrc:

  :map  <expr> <Leader>cc  nerdcommenter#Plug('Comment')|ounmap <Leader>cc|sunmap <Leader>cc
  :map  <expr> <Leader>c<Space>  nerdcommenter#Plug('Toggle')|ounmap <Leader>c<Space>|sunmap <Leader>c<Space>
  :map  <expr> <Leader>cm  nerdcommenter#Plug('Minimal')|ounmap <Leader>cm|sunmap <Leader>cm
  :map  <expr> <Leader>cn  nerdcommenter#Plug('Nested')|ounmap <Leader>cn|sunmap <Leader>cn
  :nmap <expr> <Leader>c$  nerdcommenter#Plug('ToEOL')
  :map  <expr> <Leader>ci  nerdcommenter#Plug('Invert')|ounmap <Leader>ci|sunmap <Leader>ci
  :map  <expr> <Leader>cs  nerdcommenter#Plug('Sexy')|ounmap <Leader>cs|sunmap <Leader>cs
  :map  <expr> <Leader>cy  nerdcommenter#Plug('Yank')|ounmap <Leader>cy|sunmap <Leader>cy
  :nmap <expr> <Leader>cA  nerdcommenter#Plug('Append')
  :map  <expr> <Leader>cl  nerdcommenter#Plug('AlignLeft')|ounmap <Leader>cl|sunmap <Leader>cl
  :map  <expr> <Leader>cb  nerdcommenter#Plug('AlignBoth')|ounmap <Leader>cb|sunmap <Leader>cb
  :map  <expr> <Leader>cu  nerdcommenter#Plug('Uncomment')|ounmap <Leader>cu|sunmap <Leader>cu
  :nmap <expr> <Leader>ca  nerdcommenter#Plug('AltDelims')

