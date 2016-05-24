# Installation  

The NERD Commenter requires Vim 7 or higher is comprised of 2 files:  

    plugin/NERD_commenter.vim  
    doc/NERD_commenter.txt 

## Via Plugin Manager (Recommended)

#### Pathogen Install

###### Unix

```sh
git clone https://github.com/scrooloose/nerdcommenter.git ~/.vim/bundle
```

###### Neovim

```sh
git clone https://github.com/scrooloose/nerdcommenter.git ~/.config/nvim/bundle
```

#### Vim-Plug Install
1. Add `Plug 'Plug scrooloose/nerdcommenter'` to your .vimrc file.
2. Reload .vimrc (`:so %` from vimrc, or just restart vim)
3. Run `:PlugInstall`

#### Vundle Install
1. Add `Plugin 'scrooloose/nerdcommenter'` to your .vimrc file.
2. Run `:BundleInstall`

#### NeoBundle Install
1. Add `NeoBundle 'scrooloose/nerdcommenter'` to your .vimrc file.
2. Run `:NeoUpdate``

#### Post Install  
After the **'Classic'** or **'Pathogen'** install, make sure that you have filetype plugins enabled, as the script makes use of 
**|'commentstring'|** where possible (which is usually set in a filetype plugin). 
See **|filetype-plugin-on|** for details, but basically, stick this in your vimrc:

    filetype plugin on

## Install Manually

#### Vim

###### Unix

```sh
git clone https://github.com/scrooloose/nerdcommenter.git ~/.vim/plugin
```

###### Windows (PowerShell)

```powershell
md ~\vimfiles\plugin
$uri = 'https://raw.githubusercontent.com/scrooloose/nerdcommenter/master/plugin/NERD_commenter.vim'
(New-Object Net.WebClient).DownloadFile($uri, $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath("~\vimfiles\autoload\NERD_commenter.vim"))
```

#### Neovim

```sh
git clone https://github.com/scrooloose/nerdcommenter.git ~/.config/nvim/plugin
```


# Usage  

The following key mappings are provided by default (there is also a menu 
provided that contains menu items corresponding to all the below mappings): 

Most of the following mappings are for normal/visual mode only. The |NERDComInsertComment| mapping is for insert mode only. 

**[count]\<leader\>cc |NERDComComment|**  
Comment out the current line or text selected in visual mode. 


**[count]\<leader\>cn |NERDComNestedComment|**  
Same as \<leader\>cc but forces nesting. 


**[count]\<leader\>c\<space\> |NERDComToggleComment|**  
Toggles the comment state of the selected line(s). If the topmost selected 
line is commented, all selected lines are uncommented and vice versa. 


**[count]\<leader\>cm |NERDComMinimalComment|**  
Comments the given lines using only one set of multipart delimiters. 


**[count]\<leader\>ci |NERDComInvertComment|**  
Toggles the comment state of the selected line(s) individually. 


**[count]\<leader\>cs |NERDComSexyComment|**  
Comments out the selected lines ``sexily'' 


**[count]\<leader\>cy |NERDComYankComment|**  
Same as \<leader\>cc except that the commented line(s) are yanked first. 


**\<leader\>c$ |NERDComEOLComment|**  
Comments the current line from the cursor to the end of line. 


**\<leader\>cA |NERDComAppendComment|**  
Adds comment delimiters to the end of line and goes into insert mode between 
them. 


**|NERDComInsertComment|**  
Adds comment delimiters at the current cursor position and inserts between. 
Disabled by default. 


**\<leader\>ca |NERDComAltDelim|**  
Switches to the alternative set of delimiters. 


**[count]\<leader\>cl**  
**[count]\<leader\>cb    |NERDComAlignedComment|**  
Same as |NERDComComment| except that the delimiters are aligned down the 
left side (\<leader\>cl) or both sides (\<leader\>cb). 


**[count]\<leader\>cu |NERDComUncommentLine|**  
Uncomments the selected line(s). 
