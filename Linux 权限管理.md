# 跟权限有关的三个文件
1. /etc/passwd    user account
2. /etc/group     group info
3. /etc/shadow    password
# rwx对于文件和目录的效果区别
| 属性| 文件          | 目录  |
| --- |:-------------:| -----:|
| r   | 允许打开并读取文件内容 | 允许列出目录中的内容，前提是设置了x属性|
| w   | 允许写入文件内容或截断文件，不允许重命名和删除      |  允许新建、删除、重命名文件，前提是设置了x属性 |
| x   | 允许将文件作为程序来执行，使用脚本语言编写的程序必须设置为可读才能被执行      |    允许进入目录 |
# id
# chmod
# umask
# su
# sudo
# chown
# chgrp
# passwd
