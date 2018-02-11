# Linux
学习笔记
# linux 命令行的规则

command -options -args
ls      -a       /usr 为例

1. short option -a -l -h
2. long option -all -list
3. short option combine -alh

# file命令
file filename（用于辨识该文件的类型）
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

# 命令的种类 type、which、help、man命令
1. execute binary 可执行二进制文件()
2. buildin bash (内建bash)
3. shell function (内嵌的shell)
4. alias (别名)
# awk命令
分析工具
# nohup命令（no hang up 不挂起执行）
该命令的一般形式为：nohup command &

  &的意思是在后台运行， 什么意思呢？  意思是说， 当你在执行 ./a.out & 的时候， 即使你用ctrl C,  那么a.out照样运行（因为对SIGINT信号免疫）。 但是要注意， 如果你直接关掉shell后， 那么， a.out进程同样消失。 可见， &的后台并不硬（因为对SIGHUP信号不免疫）。
   nohup的意思是忽略SIGHUP信号， 所以当运行nohup ./a.out的时候， 关闭shell, 那么a.out进程还是存在的（对SIGHUP信号免疫）。 但是， 要注意， 如果你直接在shell中用Ctrl C, 那么, a.out进程也是会消失的（因为对SIGINT信号不免疫）
   所以， &和nohup没有半毛钱的关系， 要让进程真正不受shell中Ctrl C和shell关闭的影响， 那该怎么办呢？ 那就用nohua ./a.out &吧， 两全其美。
   如果你懂守护进程， 那么nohup ./a.out &颇有点让a.out成为守护进程的感觉。

