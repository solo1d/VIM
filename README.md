# VIM使用笔记

```bash
命令 vimtutor 可以进入vim教程, 就是文档介绍.
系统配置文件 /etc/vim/vimrc    ,用户配置文件 $HOME/.vimrc 

vim 中的快捷按键:

    上下左右   k j h l
    上一页     Ctrl + b
    下一页     Ctrl + f

    快速退出   ZZ  .
    代码排版   gg=G  .
    快速定位   行号加G  .
    
    光标定位   0 (零,到行首) ,  $(行尾) .
    光标快速   gg (文件首部),   G(文件尾部).
    行数跳转   123G (跳转到123行).
    增加行数   222 回车  (跳转到当前行数+222 的那一行).

    删除字符    x (删除光标后面的)  X (删除光标前面的).
    删除单词    dw(删除光标所在单词的后面的部分).
    删除半行    d0(删除光标这一行前面的所有字符) D或d$ (删除后面的).
    删除整行    dd (这个实际是剪切,但是可以用来删除).
    删除多行    20dd (删除当前光标位置向下的20行内容).
    删除所有    dG (在文件开头输出,会全部删除).
    删除任意    先进入v 可视模式. 选择后再按 d 就可以了.

    撤销操作     u
    反撤销       Ctrl + r  (组合键)
    复制一行     yy (在想要复制的行内输入).
    粘贴一行     p / P (一个在光标下面,一个在光标上面粘贴). 
    复制多行     3yy (复制了三行).
    任意复制     先进入v 可视模式. 选择后再按 y 就可以了
    任意粘贴     p / P  (会在光标后面或前面进行粘贴,但是需要 任意复制).

    替换操作     r / R ( r 一个字符,是光标后面的字符, R 替换多个,从光标后的位置向后替换).
    整行替换     :s/需要替换的内容/替换后的内容/g  (把这一行的内容替换掉).
    指定行替换   :12,29s/work/newlink/g  (把12到29行中的 work 替换成 newlink).
    全文替换     :%s/work/newlink/g      (全文的 work 替换成 newlink).
    提示替换     :s/work/gc    (c 关键字会提示用户是否替换,上面都能使用这个选项).

    查找操作     / 或者 ?  在单词上按 # 可以查找这个单词 (n 向下,N 向上).
    man文档      章节号 + K  (在函数上按就会打开一个帮助文档,q退出和vim一样).
                            (函数按3, 系统调用按2, shell和执行程序按1)
    shell命令    ! 后面跟shell 命令就可以执行了.   ! gcc main.c


    分屏操作     :sp 文件名  或者 :vsp 文件名 (一个横向屏,一个竖向屏,在后面添加文件名就能打开两个不同文件).
    屏幕切换     Ctrl + w w  (两个ww 之后就可以在两个窗口之间切换光标了).
    多窗口保存   :wall   (退出是 :qall  , 保存退出:wqall)
    直接分屏     vim -O 文件1 文件2  ; (shell命令, 直接打开两个文件并且分屏显示,竖屏)

```

