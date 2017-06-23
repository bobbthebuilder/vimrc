""" --- Minimal vim configuration file for C/C++ development --- """

""" enable ruler
set ruler

""" ignore case
set ic

""" prevent the cursor from changing the current column when jumping to other lines
set nostartofline

""" show a status line even when only one window is shown
set laststatus=2

""" adjust command promt window size
set cmdheight=1

""" highlight all search hits
set hlsearch

""" disable vi compatibility (emulation of old bugs)
set nocompatible

""" use indentation of previous line
set autoindent

""" use intelligent indentation for C
set smartindent

""" tab width is 4 spaces
set tabstop=4

""" indent also with 4 spaces
set shiftwidth=4

""" sets the number of columns for a TAB
set softtabstop=4

""" expand tabs to spaces
set expandtab

""" wrap lines at 180 characters
set textwidth=180

""" turn syntax highlighting on
syntax on

""" turn line numbers on
set number

""" highlight matching braces
set showmatch

""" intelligent comments
set comments=sl:/*,mb:\ *,elx:\ */

""" disable .swp backup file
set noswapfile

"""
"augroup project
"    autocmd!
"    autocmd BufRead,BufNewFile *.h,*.c set filetype=c.doxygen
"augroup

""" comma-separated list of directories in which vim searches for include files
" let &path.="src/include,/usr/include/AL,"
"

""" to not expand tabs to spaces in makefiles
autocmd! FileType make setlocal noexpandtab

""" highlight all trailing whitespaces in c,cpp,sh files
autocmd! FileType c,cpp,sh :match ErrorMsg '\s\+$'

""" delete all trailing whitespaces by hotkey
nnoremap <silent> <F3> :let _s=@/<Bar>:%s/\s\+$//e<Bar>:let @/=_s<Bar>:nohl<CR>

""" switch between header/source files by hotkey
map <F4> :e %:p:s,.h$,.X123X,:s,.cpp$,.h,:s,.X123X$,.cpp,<CR>
