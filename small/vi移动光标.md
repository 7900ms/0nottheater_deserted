
进入 [vi-mode](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/vi-mode)

ctrl+[

一般思路：移动到对的位置，然后输入或删除

光标的位置、光标的动作

= = = 移动光标 = = =

前进

b
3b

后退

w
3w

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

删除整行
dd

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

= = = 高级 - 词块操作 = = =

光标放在空格处，删除一个单词
de
db

全删掉
d$
d^
dd

= = = 高级 - 复制粘贴 = = =

复制

粘贴

复制整行


-

emacs:
去最开头 ctrl+a
去最末尾 ctrl+e

-

/supplementary/傲游
用 de 不用 dw
http://arhat.blog.51cto.com/101503/114148

-

