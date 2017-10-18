# Linux IO 重定向学习笔记
stdout  stander output
stderr  stander error
stdin   stander input

1. common > filename
2. common >> filename

## 重定向标准错误信息
0:stdin
1:stdout
2:stderr
1. ls -al /eee 2 > ilename
2. ls -l . /eeee 1> filename 2>&1 （这个命令很重要）
2. ls -l . /eeee &> filename （这个命令很重要）

# useless message
重定向到/dev/null 垃圾桶
