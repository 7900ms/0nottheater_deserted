
进入 [vi-mode](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/vi-mode)

(目标：用少量的 基本操作，完成大量的工作)

ctrl+[

一般思路：移动到对的位置，然后输入或删除

光标的位置、光标的动作

= = = 移动光标 = = =

to the Beginning of a word:

b

to the End of a word:

e
3e

= = = 移动光标 = = =

去最开头
^

去最末尾
$

= = = 撤销键盘操作 = = =

撤销
u

重做
ctrl+r

= = = 键盘操作 = = =

删除
X

自删除
x

= = = 光标操作 = = =

删除,光标动
X

(
一个经典动作：从某位置开始，一个一个字的向前删除字母
去最末尾        $
光标任意位置    3b
删除,光标动     X
(撤销 u)
光标任意位置    3w
自删除(清理最后一个字符) x
)

= = = 高级 - (组合快捷键)行操作 = = =

删除整行
dd

= = = 高级 - (组合快捷键)词块操作: 删除 + 去一个单词/一行的首尾位置 = = =

光标放在空格处，删除一个单词
de
db

全删掉
d$
d^

= = = 高级 - 复制粘贴 = = =

复制
y

粘贴
p

复制整行
yy

-

emacs:
去最开头 ctrl+a
去最末尾 ctrl+e

-

/supplementary/一般思路
移动到对的位置，然后输入或删除

/supplementary/移动光标不用
w,3w
/supplementary/删除单词不用
dw

/supplementary/傲游
让光标起始位置在空格处，再删除。用 de 不用 dw 
http://arhat.blog.51cto.com/101503/114148
https://www.ibm.com/developerworks/cn/linux/l-cn-tip-vim/
G vi 常用命令 db

http://www.thegeekstuff.com/2009/03/8-essential-vim-editor-navigation-fundamentals/

-

