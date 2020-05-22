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

