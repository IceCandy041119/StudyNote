# TmuxNotes

## 目录   

- [介绍](#介绍)
- [使用](#使用)

## 介绍

Tmux是一个终端复用工具,允许你在一个终端中使用多个Shell.其允许高度可定制的工具,可以使用相关快捷键创建多个标签页并在它们间导航.       

## 使用   

`tmux` 快捷键——都要先按下前缀键默认 `Ctrl+b`     
- **会话**-每个会话都是一个独立的工作区,其中包含一个或多个窗口
	- `tumx` 开始一个新的会话
	- `tumx new -s NAME` 以指定名称开始一个新的会话
	- `tmux ls` 列出当前所有的会话
	- 在会话中输入 `前缀键+d` 与当前会话分离
	- `tmux a` 重新连接最后一个会话,也可以通过 `-t` 指定具体的会话
- **窗口**-相当于编辑器或是浏览器中的标签页,从视觉上将一个会话分割为多个部分
	- `前缀键+c` 创建一个新的窗口
	- `前缀键+N` 跳转到第N个窗口,窗口是有编号的
	- `前缀键+p` 切换到前一个窗口
	- `前缀键+n` 切换到下一个窗口
	- `前缀键+，` 重命名当前窗口
	- `前缀键+w` 列出当前所有窗口
- **面板**-像vim中的分屏一样,面板使我们可以在一个屏幕里显示多个Shell
	- `前缀键+"` 水平分割
	- `前缀键+%` 垂直分割
	- `前缀键+<箭头>` 切换到指定方向的面板
	- `前缀键+z` 切换当期面板的缩放
	- `前缀键+[` 开始往回滚动屏幕,可以按空格键选择,回车复制选中的部分
	- `前缀键+空格` 在不同的面板排布间切换

>一般不要嵌套多个Tmux不然容易混乱,一般默认情况下会阻止你这样做,嵌套情况常见于在Tmux使用 `ssh` 登陆到远端后在远端使用Tmux,这样Tmux阻止不了.如果发生了可以 `前缀键+前缀键` 选中最外层的终端.    

