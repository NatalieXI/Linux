# Linux
学习笔记
# linux 命令行的规则

command -options -args
ls      -a       /usr 为例

1. short option -a -l -h
2. long option -all -list
3. short option combine -alh

# file命令
file filename
# less 命令
less filename
1. j.k.d.u.space
2. q退出

# 通配符
1. 星号  0,1,more char 
2. ?  1 char
3. [character] one character in set
4. [!character] no one character in set
5. [[:class:]] one char in class
## 有以下几种类
1. [:digit:] number
2. [:lower:] lower char 
3. [:upper:] upper char 
4. [:alnum:] num + alpha
5. [:alpha:] lower + upper

# mkdir命令
mkdir directory....

# cp命令（copy）
1. cp item1 item2（当前目录当中复制一个文件）
2. cp items... directory
3. -a(archive) -i(interactive) -r(recursive递归的) -u(update) -v(verbose)

# ln命令
ln file link  //创建硬链接
ln -s item link //创建软链接
## 硬链接
编辑一个其中文件，所有的文件都会变化，且删除任何一个文件不会影响其他文件
## 软链接
相当于windows的快捷方式，编辑一个其中文件，所有的文件都会变化，删除源文件，链接中断
