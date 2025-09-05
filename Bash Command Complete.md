# Bash Command Complete

## About Bash

Bash is an sh-compatible command language interpreter that executes commands read from the standard input or from a file.  Bash also incorporates useful features from the Korn and C shells (ksh and csh).

Bash is intended to be a conformant implementation of the Shell and Utilities portion of the IEEE POSIX specification (IEEE Standard 1003.1).  Bash can be configured to be POSIX-conformant  by  default.

```bash
bash --version
    GNU bash, version 5.0.17(1)-release (x86_64-pc-linux-gnu)
    Copyright (C) 2019 Free Software Foundation, Inc.
    License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>

    This is free software; you are free to change and redistribute it.
    There is NO WARRANTY, to the extent permitted by law.
man bash  #manual of Bash
help  #list all internal shell commands
help cd  #help information of command 'cd'
```

GNU official Bash manual: https://www.gnu.org/software/bash/manual/

Bash guide from The Linux Documentation Project: https://tldp.org/LDP/abs/html/



## File System Management

### `pwd` print work directory 输出当前工作目录

```bash
uesrname@hostname:~$ pwd
/home/uesrname
```

`uesrname@hostname`： 始终会显示，指示了当前设备和用户是什么。

`uesrname@hostname`: always display, indicate what this device is and which user is working.

`~$`：其中`~`指示了当前工作目录是用户的 home 目录；`$`指示了当前用户为普通用户。

`~$`：`~` indicate the current work directory is the home of the user; `$` indicate the user is a normal user.

### `ls` list directory contents 列出工作目录内容

```bash
uesrname@hostname:~$ ls
Applications   Desktop   Documents   Downloads   help   Music   Pictures   Videos
uesrname@hostname:~$ ls -1  # One item per line
Applications
Desktop
Documents
Downloads
...
uesrname@hostname:~$ ls -d Documents  #-d, --directory: list directories themselves, not their contents. This can check if a folder exits
Documents
uesrname@hostname:~$ ls -a /  #Shows all, including hidden ones and . , .. 
.  ..  bin  boot  cdrom  dev  etc  home  lib  lib32  lib64  libx32  ...  #Too long so omitted here
uesrname@hostname:~$ ls -A /  #Shows all, including hidden ones but without . , .. 
bin  boot  cdrom  dev  etc  home  lib  lib32  lib64  libx32  ...  #Too long so omitted here
uesrname@hostname:~$ ls -l ~  #Long format
total 116
#drwxrwxr-x  3 xiongyw xiongyw  4096 2月   6 16:21  Applications
#-rw-r--r--  1 xiongyw xiongyw 12484 2月  20 10:48 'capes for nongraphic characters'
#drwxr-xr-x  2 xiongyw xiongyw  4096 1月   6 17:09  Desktop
#drwxr-xr-x  4 xiongyw xiongyw  4096 2月  19 13:47  Documents
#drwxr-xr-x  2 xiongyw xiongyw  4096 2月  19 12:07  Downloads
#drwxrwxr-x  2 xiongyw xiongyw  4096 1月   8 13:47  help
#drwxr-xr-x  2 xiongyw xiongyw  4096 1月   3 18:18  Music
#drwxr-xr-x  3 xiongyw xiongyw  4096 2月  18 18:04  Pictures
#drwxrwxr-x  2 xiongyw xiongyw  4096 1月   6 10:36 'Sunlogin Files'
#-rw-r--r--  1 xiongyw xiongyw 12484 2月  20 10:48 't directories themselves, not their contents'
#-rw-r--r--  1 xiongyw xiongyw  9919 2月  20 10:48 't information about the FILEs (the current directory by default).  Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.'
#drwxr-xr-x  2 xiongyw xiongyw  4096 1月   3 18:18  Videos
uesrname@hostname:~$ ls -lh ~  #Displays file sizes in human-readable units
#total 116K
#drwxrwxr-x  3 xiongyw xiongyw 4.0K 2月   6 16:21  Applications
#-rw-r--r--  1 xiongyw xiongyw  13K 2月  20 10:48 'capes for nongraphic characters'
#drwxr-xr-x  2 xiongyw xiongyw 4.0K 1月   6 17:09  Desktop
#drwxr-xr-x  4 xiongyw xiongyw 4.0K 2月  19 13:47  Documents
#...  #Too long so omitted here
uesrname@hostname:~$ ls -lt ~  #Sorts by modification time (newest first)
uesrname@hostname:~$ ls -lS ~  #Sorts by size (largest first)
uesrname@hostname:~$ ls -ltr ~  #-r to reverses the default sort order.
uesrname@hostname:~$ ls -lt -r ~  #-r to reverses the default sort order.
uesrname@hostname:~$ ls -F ~  #File types symbols
# Applications/    'capes for nongraphic characters'        Desktop/
# Pictures/        Personnel/                               't directories themselves, not their contents'
# ...
```

```bash
ls -ld .
```



### `cd` change directory 切换目录

切换当前的工作目录为用户指定的目录。

```bash
uesrname@hostname:~$ cd Documents
uesrname@hostname:~/Documents$ 
```

`.`: Current directory;

`..`: Parent directory;

`~`: Home directory;

`/`: Root directory (type all alone);



```bash
find . -name "example.txt"  #Find file example.txt in the current directory and its subdirectory.
```

```bash
sudo chown $USER:$USER .
sudo chown xiongyw:xiongyw .
```

## rename

```bash
rename [选项] 's/原字符串/新字符串/[修饰符]' 文件名匹配模式
# 替换 old 为 new
rename 's/old/new/' *old*
# 添加前缀
rename 's/^/prefix_/' *.jpg
# 添加后缀
rename 's/$/_backup/' *.log
# -n 或 --nothink: 模拟运行（显示将要重命名的文件，但不实际执行）
rename -n 's/pattern/replacement/' *.files
# -f 或 --force: 强制覆盖已存在的文件
rename -f 's/pattern/replacement/' *.files
# 对.png进行rename
rename 's/pattern/replacement/' *.png
# 对任意文件名进行rename
rename 's/pattern/replacement/' *
```



## Others

### Ctrl + C 终止续行模式（左侧出现续行提示符）

## Reference

https://www.linuxcool.com/