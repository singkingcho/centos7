> 环境准备好之后，我们终于可以学习啦。
>
> -----



linux当中很多内容都很重要，但是讲解顺序我这样安排，先讲解命令，然后讲解文件系统，再讲解用户组全新啊等等。



# 一、 命令

学习Linux，很大一部分的内容就是学习相关的命令，我们没有安装Linux桌面，一开始会不习惯，坚持坚持就好了。

这里我会采用mobaxterm作为终端进行命令的编写与研究



## 1. 文件、路径、目录



### 1）pwd

查看当前目录



### 2）cd

change directory 切换目录

==**要搞清楚，绝对路径与相对路径**==

/开头为绝对路径，以根目录走起，注意好这里没有C盘，D盘的概念，就一个根。

不以斜杠开头则代表从当前目录出发。

```bash
cd /usr/local
```

上面的含义就是从根目录出发到user目录下的local目录之下。

使用相对路径从/usr/local下到bin下使用两种方式进入

```bash
cd /usr/local/bin #使用绝对路径
cd bin #使用相对路径
```

回到上级

```bash
cd ..
```



### 3）mkdir

创建文件夹

```bash
mkdir hello

```

一次创建多个文件夹（这是就在当前目录下）

```bash
mkdir d1 d2 d3
```



创建多层次目录

```bash
mkdir -p d4/d5/d6
```



当然结合上面的一次创建多个文件夹 分开标识也可以

```bash
mkdir -p d11/d22/d33 d55/d77
```



### 4）rmdir

remove direcotry 移除文件夹

移除空目录

```bash
rmdir d1
```



移除连续空目录

```bash
rmdir d1/d2
```

注意此时的d1之下不能有别的文件，否则无法删除



### 5）rm

万能删除命令注意，rm d1

尝试直接删除一个目录是无法删除的

```bash
rm -d d1
```

删除空目录，系统会询问是否删除，回答yes即可删除。



**强制删除所有（谨慎使用）**

Linux没有回收站一说。

```bash
rm -rf path
```

### 6）touch 

摸一下，摸出了一个文件

```bash
touch hello
```



```bash
touch hello.txt love.txt
```



## 2. vi

在命令模式下，输入的每个字符都是对正在编辑的文本文件执行某些操作的命令; 在命令模式下键入的字符甚至可能导致

vi

编辑器进入插入模式。在插入模式下，每个输入的字符都被添加到文件中的文本中; 按下

<Esc>

 键将关闭插入模式。

虽然有很多`vi`命令，但其中少数就已经够我们用了。



vi模式，编辑器根据用户的键入处于不同模式之下

- 命令模式
- 编辑模式
- 底端模式



命令模式此时无法直接在文件当中键入内容，用于翻阅，删除等等。

```bash

```





```bash

```





```bash

```





```bash

```











