Android Developer Common Commands
===========================
Android开发常用命令

****

```
netstat -pnlt | grep ':portno'           // how to use netstat on a specific port in Linux

wget --mirror -p --adjust-extension --no-parent --convert-links -P yii_doc <url>

export http_proxy=debian:123456@proxy.debian.org:8080 
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

#https://help.github.com/articles/creating-project-pages-manually/
git checkout --orphan gh-pages
# Creates our branch, without any parents (it's an orphan!)
git rm -rf .
# Remove all files from the old working tree
git add index.html
git commit -a -m "First pages commit"
git push origin gh-pages


#Push files
git commit -m 'my notes' -- path/to/my/file.ext
```