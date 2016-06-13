Android Developer Common Commands
===========================
Android开发常用命令

****

图片大小转换
```Bash
convert myfigure.png -resize 200×100 myfigure.jpg #Bash

function doConvert
{
    mkdir $1
	convert $2 -resize $1x$1 $1/$2
}
doConvert "64" "test.png" 
```


VIM 编码转换：
```
:write ++enc=utf-8 russian.txt
```

git命令
```Bash
#Clone the repository
git clone https://github.com/username/username.github.io   

#Push it
git add --all   
git commit -m "Initial commit"
git push -u origin master

#Push files
git commit -m 'my notes' -- path/to/my/file.ext
```