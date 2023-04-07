# mac VIM配置文件备份

```bash
"激活VIM 内置插件
set nocompatible
filetype plugin on

"主题"-----------------------------------------
"set nu    
colorscheme default
syntax on
"编码"-----------------------------------------
set fileencodings=utf-8
set fencs=utf-8
set termencoding=utf-8
set encoding=utf-8

"自动判断编码时 依次尝试一下编码
set fileencodings=utf-8,gb18030,gbk,gb2312,ANSI,ucs-bom,cp936,big5,euc-jp,euc-kr

" 设置外观 -------------------------------------
"set number                      "显示行号 
set numberwidth=1               "设置在编辑过程中右下角显示光标的行列信息
set showtabline=0               "隐藏顶部标签栏"
set guioptions-=r               "隐藏右侧滚动条" 
set guioptions-=L               "隐藏左侧滚动条"
set guioptions-=b               "隐藏底部滚动条"
"set cursorline                  突出显示当前行"
"set cursorcolumn                突出显示当前列"
set langmenu=zh_CN.UTF-8        "显示中文菜单
set showcmd                     "在状态栏显示正在输入的命令
set autoindent      			"设置C/C++方式自动对齐
set cindent                     "也是设置C/C++方式自动对齐"


" 变成辅助 -------------------------------------
syntax on                       "开启语法高亮
set nowrap                      "设置代码换行""nowrap 表示不换行"
set fileformat=unix             "设置以unix的格式保存文件"
set cindent                     "设置C样式的缩进格式"
set tabstop=4                   "一个 tab 显示出来是多少个空格，默认 8
set shiftwidth=4                "每一级缩进是多少个空格
set backspace+=indent,eol,start "set backspace&可以对其重置
set showmatch                   "显示匹配的括号"
set scrolloff=5                 "距离顶部和底部5行"
set laststatus=2                "命令行为两行"
" 其他杂项 -------------------------------------
"set mouse=a                     启用鼠标"
set selection=exclusive
set selectmode=mouse,key
set matchtime=5
set ignorecase                  "忽略大小写"
set incsearch
set hlsearch                    "高亮搜索项"
"set expandtab                   "将Tab键自动转换成空格 真正需要Tab键时使用[Ctrl + V + Tab]
%retab!
set whichwrap+=<,>,h,l
set autoread   
set wrap						"自动折行"


"启动时隐去援助提示
set shortmess=atI

"没有保存或文件只读时弹出确认
"set confirm

"文件自动检测外部更改
set autoread

"c文件自动缩进
set cindent


"智能缩进
set smartindent

"显示标尺，就是在右下角显示光标位置
set ruler

"启动显示状态行
set laststatus=2

"浅色显示当前行
"autocmd InsertLeave * se nocul

"用浅色高亮当前行
"autocmd InsertEnter * se cul


"被分割窗口之间显示空白
"set fillchars=vert:/
"set fillchars=stl:/
"set fillchars=stlnc:/

" vundle 环境设置
"filetype off
"set rtp+=~/.vim/bundle/Vundle.vim
"vundle管理的插件列表必须位于 vundle#begin() 和 vundle#end() 之间
"call vundle#begin()
"Plugin 'VundleVim/Vundle.vim'
"Plugin 'altercation/vim-colors-solarized'
"Plugin 'tomasr/molokai'
"Plugin 'vim-scripts/phd'
"Plugin 'Lokaltog/vim-powerline'
"Plugin 'octol/vim-cpp-enhanced-highlight'
"Plugin 'Raimondi/delimitMate'
" 插件列表结束
"call vundle#end()
"filetype plugin indent on


" 配色方案
"set background=dark
"colorscheme torte
"colorscheme molokai
"colorscheme phd

" 禁止显示菜单和工具条
"set guioptions-=m
"set guioptions-=T


"共享剪切板
"set clipboard=unnamed


" 总是显示状态栏
"set laststatus=2




" 基于缩进或语法进行代码折叠
"set foldmethod=indent
"set foldmethod=syntax
" 启动 vim 时关闭折叠代码
"set nofoldenable
```

