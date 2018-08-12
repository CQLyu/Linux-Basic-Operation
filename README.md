# Linux Basic Operation
It comes from the [EasyHPC](http://www.easyhpc.org/)

## Chapter 1	Linux基础入门

### 1.1	linux常用快捷键以及帮助手册 

在我们正式学习linux命令之前，我们应该了解一些基本的快捷键，以及查看帮助手册。

#### 1.1.1 快捷键

- Tab :  命令补全，当你忘记某个命令的全称时可以只输入它的开头的一部分，然后按下 Tab 键 就可以得到提示或者帮助完成。
- Ctrl+c ： 强行终止当前程序。

- Ctrl+d ： 键盘输入结束或退出终端。

- Ctrl+s ： 暂停当前程序，暂停后按下任意键恢复运行。

- Ctrl+z ： 将当前程序放到后台运行，恢复到前台为命令fg。

- Ctrl+a ： 将光标移至输入行头，相当于Home键。

- Ctrl+e ： 将光标移至输入行末，相当于End键。

- Ctrl+k ： 删除从光标所在位置到行末。

- Alt+Backspace ： 向前删除一个单词。

- Shift+PgUp ： 将终端显示向上滚动。

- Shift+PgDn ： 将终端显示向下滚动。

#### 1.1.2 帮助手册

在 Linux 环境中，如果你对某个命令感到疑惑，可以使用man命令来获取帮助，它是Manual pages的缩写。用户可以通过执行man命令调用手册页。

```shell
$ man <command_name>
```

