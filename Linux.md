Android Developer Common Commands
===========================
Linux常用命令

****

Linux查看文件夹大小du -sh 查看当前文件夹大小
```Bash
du -sh * | sort -n #统计当前文件夹(目录)大小，并按文件大小排序
```

Notepad++中用正则表达式匹配中文
通常正则表达式匹配中文可以利用Unicode的特点，使用[\u4e00-\u9fa5]匹配。但在Notepad++中不能正常使用。
解决方法是，首先将编码转换成Unicode（菜单->格式->转换为UTF-8，如果不转换可能匹配出错），然后使用[\x{4e00}-\x{9fa5}]就可以实现匹配中文了。
```
android.(text|hint).*[\x{4e00}-\x{9fa5}]+.*
```

```
date +"%Y-%m-%d %T"

file -sL /dev/sd*     //  How do I tell what sort of data (what data format) is in a file?
UUID=3c05a2da-4e6b-4ba7-855e-62914e67c99f /home/war/aosp  ext3    defaults rw 0 0    // sudo vi /etc/fstab

find /path -name '*.cpp' |xargs wc -l   //统计一个项目的代码数：
grep --color='auto' -P -n "[\x80-\xFF]" file.xml   //grep for non-ASCII characters in UNIX :
```

VIM 编码转换：
```
:write ++enc=utf-8 russian.txt
```