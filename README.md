Android Developer Common Commands
===========================
Android开发常用命令

****

```
netstat -pnlt | grep ':portno'           // how to use netstat on a specific port in Linux
```

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