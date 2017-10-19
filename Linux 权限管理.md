# 跟权限有关的三个文件
1. /etc/passwd    user account
2. /etc/group     group info
3. /etc/shadow    password
# rwx对于文件和目录的效果区别
| 属性| 文件          | 目录  |
| --- |:----------:| :-----:|
| r   | 允许打开并读取文件内容 | 允许列出目录中的内容，前提是设置了x属性|
| w   | 允许写入文件内容或截断文件，不允许重命名和删除      |  允许新建、删除、重命名文件，前提是设置了x属性 |
| x   | 允许将文件作为程序来执行，使用脚本语言编写的程序必须设置为可读才能被执行      |    允许进入目录 |
# id
查看当前用户的uid ,gid等等
# chmod
1. 二进制表示法 chmod 600 filename
2. 符号表示法(u,g,o)(+,-,=)(r,w,x) chmod o+r filename
# umask去掉不需要的默认权限
1. umask 0066 第一个 为特殊权限
# su
# sudo
# chown
chown [owner][:group] filename
# chgrp(用的不多，因为chown可以完成这个操作)

# passwd
passwd [user]
