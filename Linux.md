Android Developer Common Commands
===========================
Linux��������

****

Linux�鿴�ļ��д�Сdu -sh �鿴��ǰ�ļ��д�С
```Bash
du -sh * | sort -n #ͳ�Ƶ�ǰ�ļ���(Ŀ¼)��С�������ļ���С����
```

Notepad++����������ʽƥ������
ͨ��������ʽƥ�����Ŀ�������Unicode���ص㣬ʹ��[\u4e00-\u9fa5]ƥ�䡣����Notepad++�в�������ʹ�á�
��������ǣ����Ƚ�����ת����Unicode���˵�->��ʽ->ת��ΪUTF-8�������ת������ƥ�������Ȼ��ʹ��[\x{4e00}-\x{9fa5}]�Ϳ���ʵ��ƥ�������ˡ�
```
android.(text|hint).*[\x{4e00}-\x{9fa5}]+.*
```

```
date +"%Y-%m-%d %T"

file -sL /dev/sd*     //  How do I tell what sort of data (what data format) is in a file?
UUID=3c05a2da-4e6b-4ba7-855e-62914e67c99f /home/war/aosp  ext3    defaults rw 0 0    // sudo vi /etc/fstab

find /path -name '*.cpp' |xargs wc -l   //ͳ��һ����Ŀ�Ĵ�������
grep --color='auto' -P -n "[\x80-\xFF]" file.xml   //grep for non-ASCII characters in UNIX :
```

VIM ����ת����
```
:write ++enc=utf-8 russian.txt
```