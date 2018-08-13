# Linux Basic Operation
It comes from the [EasyHPC](http://www.easyhpc.org/)

## 目录

- [Chapter 1	Linux基础入门](https://github.com/Zhaojiahua/Linux-Basic-Operation#chapter-1linux%E5%9F%BA%E7%A1%80%E5%85%A5%E9%97%A8)
  - [1.1	linux常用快捷键以及帮助手册](https://github.com/Zhaojiahua/Linux-Basic-Operation#11linux%E5%B8%B8%E7%94%A8%E5%BF%AB%E6%8D%B7%E9%94%AE%E4%BB%A5%E5%8F%8A%E5%B8%AE%E5%8A%A9%E6%89%8B%E5%86%8C)
    - [1.1.1 快捷键](https://github.com/Zhaojiahua/Linux-Basic-Operation#111-%E5%BF%AB%E6%8D%B7%E9%94%AE)
    - [1.1.2 帮助手册](https://github.com/Zhaojiahua/Linux-Basic-Operation#112-%E5%B8%AE%E5%8A%A9%E6%89%8B%E5%86%8C)
    	[1.2	软件安装](https://github.com/Zhaojiahua/Linux-Basic-Operation#12%E8%BD%AF%E4%BB%B6%E5%AE%89%E8%A3%85)
    	[1.3	用户权限管理](https://github.com/Zhaojiahua/Linux-Basic-Operation#13%E7%94%A8%E6%88%B7%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86)
    - [1.3.1 查看用户](https://github.com/Zhaojiahua/Linux-Basic-Operation#131-%E6%9F%A5%E7%9C%8B%E7%94%A8%E6%88%B7)
    	[1.4	文件权限管理](https://github.com/Zhaojiahua/Linux-Basic-Operation#14%E6%96%87%E4%BB%B6%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86)
    - [1.4.1 查看文件权限](https://github.com/Zhaojiahua/Linux-Basic-Operation#141-%E6%9F%A5%E7%9C%8B%E6%96%87%E4%BB%B6%E6%9D%83%E9%99%90)
    - [1.4.2 变更文件所有者](https://github.com/Zhaojiahua/Linux-Basic-Operation#142-%E5%8F%98%E6%9B%B4%E6%96%87%E4%BB%B6%E6%89%80%E6%9C%89%E8%80%85)
    - [1.4.3 修改文件权限](https://github.com/Zhaojiahua/Linux-Basic-Operation#143-%E4%BF%AE%E6%94%B9%E6%96%87%E4%BB%B6%E6%9D%83%E9%99%90)
    	[1.5	目录及文件操作](https://github.com/Zhaojiahua/Linux-Basic-Operation#15%E7%9B%AE%E5%BD%95%E5%8F%8A%E6%96%87%E4%BB%B6%E6%93%8D%E4%BD%9C)
    - [1.5.1 基本目录操作](https://github.com/Zhaojiahua/Linux-Basic-Operation#151-%E5%9F%BA%E6%9C%AC%E7%9B%AE%E5%BD%95%E6%93%8D%E4%BD%9C)
    - [1.5.2 基本文件操作](https://github.com/Zhaojiahua/Linux-Basic-Operation#152-%E5%9F%BA%E6%9C%AC%E6%96%87%E4%BB%B6%E6%93%8D%E4%BD%9C)
    	[1.6	搜索文件](https://github.com/Zhaojiahua/Linux-Basic-Operation#16%E6%90%9C%E7%B4%A2%E6%96%87%E4%BB%B6)
    	[1.7	文件解压缩](https://github.com/Zhaojiahua/Linux-Basic-Operation#17%E6%96%87%E4%BB%B6%E8%A7%A3%E5%8E%8B%E7%BC%A9)
    	[1.8	管道与一些文本命令](https://github.com/Zhaojiahua/Linux-Basic-Operation#18%E7%AE%A1%E9%81%93%E4%B8%8E%E4%B8%80%E4%BA%9B%E6%96%87%E6%9C%AC%E5%91%BD%E4%BB%A4)
    	[1.9	文本处理](https://github.com/Zhaojiahua/Linux-Basic-Operation#19%E6%96%87%E6%9C%AC%E5%A4%84%E7%90%86)
  - [1.10  重定向](https://github.com/Zhaojiahua/Linux-Basic-Operation#110--%E9%87%8D%E5%AE%9A%E5%90%91)
  - [1.11  进程的基本操作](https://github.com/Zhaojiahua/Linux-Basic-Operation#111--%E8%BF%9B%E7%A8%8B%E7%9A%84%E5%9F%BA%E6%9C%AC%E6%93%8D%E4%BD%9C)
  - [1.12  进程管理](https://github.com/Zhaojiahua/Linux-Basic-Operation#112--%E8%BF%9B%E7%A8%8B%E7%AE%A1%E7%90%86)
- Chapter 2	Vim基础入门
- Chapter 3	Shell入门教程
- Chapter 4	GDB入门教程



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

### 1.2	软件安装

不同的linux版本会有不同的安装命令，由于我们的开发环境是基于CentOS的，所以我们以此为例学习相关的软件安装。

### 1.3	用户权限管理

Linux 是一个多用户的操作系统，所有用户共享一些主机的资源，但他们也分别有自己的用户空间，用于存放各自的文件。由于 Linux 的**用户管理**和**权限机制**，不同用户不可以轻易地查看、修改彼此的文件。

#### 1.3.1 查看用户

```shell
$ whoami
```

输出：当前伪终端的用户名。

### 1.4	文件权限管理

Linux环境中的文件有它的权限管理。

#### 1.4.1 查看文件权限

`ls` 命令不仅可以列出并显示当前目录的文件，还可以用来查看文件的权限。

```shell
$ ls -l
```

输出：文件类型和权限 链接数 所有者 所属用户组 文件大小 最后修改时间 文件名。

文件类型和权限解释

- 第一位是指文件类型，例如 `“d”` 表示目录， `“-”` 表示普通文件等。
- 后九位可以分为三组，每组三位分别表示 `读权限/写权限/执行权限` ，这三组分别对应的是 `拥有者权限/所属用户组权限/其他用户权限` 。

#### 1.4.2 变更文件所有者

```shell
$ sudo chown new_owner file
```

#### 1.4.3 修改文件权限

有两种方式对文件权限进行修改 

- 二进制数字表示。每个文件的三组权限对应一个 `"rwx"` ，每一位可以用 0 或 1 表示是否有权限，例如只有读和写权限的话就是 `"rw-" - "110"`，所以 `"rwx"` 对应的二进制"111"就是十进制的7。所以将 file 文件权限改为 `"rwx------"` 的命令是：

  ```shell
  $ chmod 700 file
  ```

- 加减赋值表示。假设一开始 file 文件的权限是 `"rwxr--r--"` 完成上述同样的效果，还可以：

  ```shell
  $ chmod go-rr file
  ```

  g、o 还有 u 分别表示 `group`、`others` 和 `user`，+ 和 - 分别表示增加和去掉相应的权限。



### 1.5	目录及文件操作

在linux系统中最常见的行为就是切换目录以及对文件进行操作了。

#### 1.5.1 基本目录操作

在linux中，我们使用 `cd` 命令来切换目录，使用 `.` 表示当前目录，`..` 表示上一级目录, `-` 表示上一次所在目录，`～` 通常表示当前用户的 home 目录。使用 `pwd` 命令可以获取当前所在路径（绝对路径）。

#### 1.5.2 基本文件操作

- 创建

  - 文件：使用 `touch` 命令来创建一个新的空白文件。

    ```shell
    $ touch myfile
    ```

  - 目录：使用 mkdir 命令可以创建一个新的目录。

    ```shell
    $ mkdir mydir
    ```

- 复制

  - 文件：使用 `cp（copy）`命令复制一个文件到指定目录。

    ```shell
    $ cp myfile ../../mydir
    ```

  - 目录：在复制文件的基础上加上 `-r` 参数即可。

    ```shell
    $ cp -r dir mydir
    ```

- 删除

  - 文件：使用 `rm（remove files or directories）`命令删除一个文件。

    ```shell
    $ rm test
    ```

  - 目录：删除目录需要加上 -r 参数。

    ```shell
    $ rm -r mydir
    ```

- 移动及重命名

  移动文件和对文件重命名都使用 `mv` 命令。 

  - mv 源目录文件 目的目录

    ```shell
    $ mv myfile mydir
    ```

    注意，这里`mv`命令是剪切文件。

  - mv 旧的文件名 新的文件名

    ```shell
    $ mv myfile myfile1
    ```

- 编辑文件

  Linux系统存在许多编辑器，例如vim，emacs，nano等等，在这里我们使用vim编辑器来打开文件

  ```shell
  $ vim myfile
  ```



### 1.6	搜索文件

Linux提供了许多与搜索相关的命令给用户使用。

- **which**：`which`只从环境变量指定的路径中去搜索文件，所以我们常常使用`which`来判断是否安装了某个软件。

  ```shell
  $ which nano
  ```

- **whereis**：一个比较简单的搜索命令，它直接从数据库而不是硬盘查询，而且只能搜索特定的文件。所以，它的搜索很快。

- **locate**：在这里要先介绍`" /var/lib/mlocate/mlocate.db "`数据库，因为 `locate` 命令就是通过这个数据库查找的。这个数据库由系统每天定时维护更新，所以有时候需要手动执行 `updatedb` 命令来更新数据库。

  ```shell
  $ locate /usr/a
  ```

  查找 /usr 及其子目录下所有以 a 开头的文件。

- **find**：`find`命令是一个功能非常强大的命令，它可以根据文件的各个属性来搜索，在此只介绍其简单的搜索。

  ```shell
  $ sudo find /usr/ -name myfile
  ```

  在 /usr/ 目录下搜索名字为 myfile 的文件或目录。



### 1.7	文件解压缩

本节介绍linux上常用的解压缩工具，包括zip、rar以及tar。

- **rar**：rar是一种在windows常见的文件压缩格式，但是在linux下必须先安装才能使用。

  - 创建压缩文件

    ```shell
    rar a ehpc.rar ./Desktop/
    ```

  - 使用 `a` 参数添加文件进压缩包

    ```
    rar a ehpc.rar a.o
    ```

  - 使用 `d` 参数删除文件

    ```
    rar d ehpc.rar a.o
    ```

  - 使用 `l` 参数查看文件

    ```
    rar l ehpc.rar
    ```

  - 解压分为两种，一种是 `x` 参数解压，这样会保持压缩文件的目录结构；另一种是 `e` 参数解压，将所有文件解压到当前目录

    ```
    unrar x ehpc.rar
    unrar e ehpc.rar
    ```

- **zip**：zip也是在windows和linux使用率比较高的文件压缩格式。

  - 创建压缩包

    ```
    zip -r -o ehpc.zip ./Desktop
    ```

    其中，`-r` 参数表示递归，所以上面命令是打包ehpc目录进压缩包；`-o` 参数表示输出到ehpc.zip压缩文件。

  - 使用 `-e` 参数进行加密

    ```
    zip -r -e -o ehpc.zip ./Desktop
    ```

    需要注意的是，由于编码问题linux下和windows下的文本文件可能会不同，如果希望在linux压缩的文件在windows下正常解压，可以加上 `-l` 参数。

  - 查看与解压

    ```
    unzip -l ehpc.zip（查看）
    unzip ehpc.zip（解压）
    ```

- **tar**：实际上，在linux中用得更多的是tar工具。tar 原本只是一个打包工具，没有压缩功能，需要配合其他具有压缩功能而没有打包功能的工具进行打包压缩。

  - 创建一个 tar 包

    ```
    tar -cf ehpc.tar ./Desktop
    ```

    其中，`-c` 参数表示创建，`-f` 参数表示指定文件名，必须跟在文件名之前。

  - 查看一个 tar 包

    ```
    tar -tf ehpc.tar
    ```

  - 解包一个 tar 包到指定目录

    ```
    tar -xf ehpc.tar -C ehpcdir
    ```

  上面我们说了tar需要配合其他工具进行压缩，其实一般只需要加一个参数就可以了。这里以gzip为例

  ```
  tar -xzf ehpc.tar.gz（解压缩）
  ```



### 1.8	管道与一些文本命令

管道是一种通信机制，它可以将前一个进程的输出作为下一个进程的输入。所以它常常用来进行进程间（也包括socket进行网络通信）的通信。不过，在这里我们首先介绍一些linux终端执行命令的知识。

- **&& 和 ||**：当我们希望同时输入多条命令时，可能还希望对某几个命令的结果进行判断。例如，如果存在某个文件，就把它删除，如果不存在则什么也不做。而 `&&` 和 `||` 就提供了这种判断的功能。`&&` 表示如果前一个命令返回的状态为0（这些状态码有一套默认的规定），则执行后一个命令，否则不执行。而 `||` 则与之相反。

  例如我们常常使用 which 命令来判断是否安装了某个命令

  ```shell
  which rar>/dev/null && echo "Installed."
  ```

  当然也可以结合使用

  ```shell
  which rar>/dev/null && echo "Installed." || echo "Not installed"
  ```

- **管道**：通常我们在命令行中使用匿名管道，由分隔符 `|` 表示，而命名管道更常出现在源代码中。

  ```shell
  ls -a | grep mysql
  ```

  这个命令就是先执行 `ls -a` 命令，然后将输出结果作为输入执行`grep mysql`命令在其中查找包含mysql的文件。

  - grep：一个很常用的命令。使用者可以通过其与正则表达式配合实现很高效的查找，不过在这里先简单介绍一下

    ```shell
    grep -r "ehpc" ~
    ```

    搜索 ~ 目录下所有包含"ehpc"的文件。

  - wc：统计并输出一个文件中行、字节等数据的数目。其中，`-l` 参数表示行数，`-c` 参数表示字节数。结合管道使用，统计文件的个数

    ```shell
    ls -a | wc -l
    ```

  -  uniq：值得注意的是，uniq只除去连续重复的的行，如果希望全文达到同样的效果我们往往会先使用 `sort` 命令进行排序，即

    ```shell
    cat words | sort | uniq
    ```



### 1.9	文本处理

在上一节中我们学习了一些管道相关的命令，现在我们继续学习一些简单的文本处理命令。

- **sort**：在之前出现过很多次的命令，顾名思义它的功能是排序。当然，它可以根据不同的标准来排序，例如

  ```shell
  ls -a | sort（默认为字典排序）
  ```

  反转排序

  ```shell
  ls -a | sort -r
  ```

- **col**：相信许多程序员在实际中都会遇到类似于将程序代码中的tab转空格的需要，而linux提供了tab和空格相互转换的命令 `col`

  ```shell
  cat myFile | col -x | cat -A
  ```

  在这里，`-x` 参数表示将 tab 转换成空格，而 `-h` 参数则相反。

- **tr**：替换操作（删除操作也可以视为一种替换操作）也是文本处理常用的操作之一。如果是要删除，可以使用 `-d` 参数

  ```shell
  echo "Hello world!" | tr -d "el"
  ```

  这样会删除"Hello world!"中所有的“e”和“l”。

  再例如将小写转换成大写

  ```shell
  echo "Hello world!" | tr '[a-z]' '[A-Z]'
  ```

- **paste**：这个命令可以简单地合并文件。例如将数据以 ';' 为分隔符合并（默认的分隔符为Tab）

  ```shell
  paste -d ';' data1 data2 data3
  ```



### 1.10  重定向

在之前管道的知识点中，学习者很容易有这种想法：命令的输出太复杂或者太多了，希望可以将其保存到文件中查看或者长久保存。而将标准输出、标准错误等信息输出到指定文件中，就是重定向。

- **重定向**：重定向是通过 '>' 和 '>>' 等操作符完成的，（当然也有'<'和'<<'，前者是导向，后者是追加），其实将标准输出看作一个文件的话，将命令输出导向到另一个文件自然也是没问题的。

  ```shell
  echo “Hello world!” > output
  ```

  结合管道

  ```shell
  cat words | sort | uniq >> output
  ```

- **文件描述符**：除了标准输出，我们还经常需要重定向标准错误，在此就必须提到标准输入、标准输出和标准错误的文件描述符。在linux中，它们的文件描述符分别是0、1、2，我们可以通过这几个描述符来完成我们想要的操作。我们可以这样来将标准输出和标准错误重定向到同一个文件

  ```shell
  cat words | sort | uniq > output 2>&1
  ```

  其中，`&`表示后面的是标准输出而不是一个文件名为1的文件，而这里的重定向顺序也是不能改变的。也可以这么做

  ```shell
  cat words | sort | uniq &> output
  ```

- **永久重定向以及“丢弃”输出**：我们很容易想到如果我们想不断将标准输出重定向到某个文件，难道需要在每一个命令后面加上重定向命令？当然是不需要的，linux提供了永久重定向的方法。当然，这里的永久也并不是那么永久

  ```shell
  exec 1> output
  ```

  其中 `exec` 命令的作用是用新的进程去替换旧的进程，或者指定重定向。有时候我们仅仅希望执行命令而不想要其输出，这时候我们可以将输出重定向到空设备 /dev/null

  ```shell
  cat words | sort | uniq 1>/dev/null 2>&1
  ```

  这样输出结果就没有。



### 1.11  进程的基本操作

在日常工作中我们常常需要对进程进行操作，这就要求我们掌握一些基本的进程操作指令。

- **前台/后台切换**：我们在之前的学习中已经知道终止一个在前台运行的进程的快捷键是 `ctrl + c` 。同样，我们在之前也已经知道将我们当前进程停止并转到后台的快捷键是 `ctrl + z`。那么，如何让我们的进程在前台与后台之间切换呢？我们可以通过 `&` 这个符号，让我们的命令在后台中运行

  ```shell
  ls &
  ```

  这样命令就会在后台自己运行了。那么当我们如何查看在后台的工作呢？可以使用

  ```shell
  jobs
  ```

  这时我们可以看到每行是这样的格式

  ```shell
  [1] + suspended ...(command)
  ```

  其中，第一列的数字表示job编号，也就是转到后台的工作的编号，第二列如果是 '+' 表示的是这是最后一个被转入后台的工作， '-' 的话则是倒数第二个，其他的话在这列没有符号。第三列表示状态，而后面则是命令本身。那么我们突然想要把工作从后台拿回前台怎么办呢？可以使用

  ```shell
  fg %jobid
  ```

  如果只是希望其在后台运行的话，可以

  ```shell
  bg %jobid
  ```

- **终止**：终止命令比较简单，但是在参数上我们可以通过选择信号值来决定以何种方式终止程序，信号值可以这样查看

  ```shell
  kill -l
  ```

  所以可以这样终止程序

  ```shell
  kill -signal pid
  ```

  或者

  ```shell
  kill -signal %jobid
  ```



### 1.12  进程管理

在这节我们进一步学习对进程的查看与控制。

- **top**：top 命令是我们常常使用查看工具，它可以实时查看系统的一些关键信息的变化。

  - 第一行：当前程序名称 当前系统时间 机器启动时间 系统用户数量 1分钟内、5分钟内和15分钟内cpu平均负载。

  - 第二行：进程总数 正在运行的进程数 休眠的进程数 停止的进程数 僵尸进程数。

  - 第三行

    - 用户空间占用CPU百分比
    - 内核空间占用CPU百分比
    - 用户空间优先级变化的进程占用CPU百分比
    - 空闲CPU百分比
    - 等待IO的CPU时间百分比
    - 硬中断占用CPU的百分比
    - 软中断占用CPU的百分比
    - 虚拟 CPU 等待物理 CPU 的时间的百分比

  - 第四行

    - 物理内存总量
    - 使用物理内存总量
    - 空闲内存总量
    - 缓存内存总量

  - 第五行

    - 交换区总量
    - 使用交换区总量
    - 空闲交换区总量
    - 缓冲交换区总量

    然后就是许多行进程的信息了，以下按顺序分别对应

    - PID：进程id
    - USER：进程所属用户
    - PR：进程动态优先级值
    - NI：进程静态优先级值
    - VIRT：进程使用虚拟内存总数
    - RES：进程使用物理内存数
    - SHR：进程共享内存大小
    - S：进程状态
    - %CPU：CPU利用率
    - %MEM：内存利用率
    - TIME+：进程活跃总时间
    - COMMAND：进程运行名

  我们甚至可以与这个程序交互，例如输入`k`的话系统会提示进一步输入信号值以及pid号以杀死一个进程，更多的信息可以查看帮助手册。

- **ps**：你一定经常看见 `ps aux` 这个命令将会列出所有的进程信息。我们还往往配合 `grep` 和正则表达式使用。

  ```shell
  ps aux | grep slurm
  ```

  打印出来的信息如下

  - F：进程的标志（process flags），当 flags 值为 1 则表示此子程序只是 fork 但没有执行 exec，为 4 表示此程序使用 root 权限
  - USER：进程拥有者
  - PID：进程ID
  - PPID：父进程的PID
  - SID：session 的ID
  - TPGID：前台进程组的ID
  - %CPU：进程占用的CPU百分比
  - %MEM：占用内存的百分比
  - NI：进程的 NICE 值
  - VSZ：进程使用虚拟内存大小
  - RSS：驻留内存中页的大小
  - TTY：终端ID
  - S or STAT：进程状态
  - WCHAN：正在等待的进程资源
  - START ：启动进程的时间
  - TIME：进程消耗CPU的时间
  - COMMAND：命令的名称和参数

  我们还可以用这样的命令去查看进程树

  ```shell
  pstree
  ```



