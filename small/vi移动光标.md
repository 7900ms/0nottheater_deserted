
进入 [vi-mode](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/vi-mode)

(提高使用效率的原则：用少量的,明白易懂的 最基本操作，完成大量的工作)

ctrl+[

一般思路：移动到对的位置，然后输入或删除

光标的位置、光标的动作

/supplementary/vi-mode的问题
vi-mode的问题是，在一个 terminal emulator 里(比如xterm,iTerm,urxvt)，当vi-mode生效时 zsh-shell的命令历史会失效：不能再 自动联想 cd 过的命令、nano 过的文件名

= = = 操作单位 = = =

矩形光标：前面的边 等于 竖线光标

操作单位

字符（h、l）→ 单词 (w、W、b、B、e) → 行 (j、k、0、^、$、:n)

先定单位,再定量 (单位是矢量的，它包含了方向)

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

矩形光标：前面的边 等于 竖线光标

正常删除 (删掉光标左边的字符)
X

自删除 (删掉光标后边的字符)
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
[vi里的操作单位](https://www.ibm.com/developerworks/cn/linux/l-cn-tip-vim/)
G vi 常用命令 db

http://www.thegeekstuff.com/2009/03/8-essential-vim-editor-navigation-fundamentals/

-

