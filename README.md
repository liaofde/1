#create a new repository on the command line

echo "# 1" >> README.md

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/liaofde/1.git
git push -u origin master


#push an existing repository from the command line

git remote add origin https://github.com/liaofde/1.git

git push -u origin master

#本地修改远程仓库地址

git remote set-url origin newAddress  

另外还可以先删除，然后添加地址  

git remote rm origin  

git remote add origin newAddress  

#找回git reset中只 add,未commit的内容  
git reset后，找回git中只add,未commit的内容。 
一般如果commit过，即使reset。也可以通过git log/git reflog查看提交记录，然后git reset --XXX。
但是没有commit就不行了。

找到两种解决办法： 
1.执行 git fsck --lost-found，然后到.git/lost-found目录下找找看有没有你丢失的文件。 


2.如果用phpstorm的话,phpstorm有自己的本地历史记录，可以恢复。其他IDE一般也有这个功能，找下这个功能。 

可以试试，也许有用。 
如果还有其他办法也可以给我留言，学习下。 
假如没有add,怎么找回，我也不知道？你知道也告诉我下。 
