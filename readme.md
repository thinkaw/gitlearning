学习路径记录：
- 目前，我先是在本机新建了一个目录gittest
- 然后

mkdir gittest
cd gittest
git init

vim readme.txt

git add readme.txt

git commit -m "xxxxx"

log in github
create a new repo

设置本地和远程仓库的SSH连接

> 第1步：创建SSH Key。在用户主目录下，看看有没有.ssh目录，如果有，再看看这个目录下有没有id_rsa和id_rsa.pub这两个文件，如果已经有了，可直接跳到下一步。如果没有，打开Shell（Windows下打开Git Bash），创建SSH Key：

> $ ssh-keygen -t rsa -C "youremail@example.com"
> 你需要把邮件地址换成你自己的邮件地址，然后一路回车，使用默认值即可，由于这个Key也不是用于军事目的，所以也无需设置密码。

> 如果一切顺利的话，可以在用户主目录里找到.ssh目录，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露出去，id_rsa.pub是公钥，可以放心地告诉任何人。

> 第2步：登陆GitHub，打开“Account settings”，“SSH Keys”页面：然后，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容：



git remote add origin git@github.com:username/newrepo.git

//git remote add origin https://github.com/thinkaw/test.git

//这个需要网页登录，上面那个不用

git push -u origin master

git push origin master

git remote -v

git remote rm origin


--删除远程仓库

--无需修改本地和远程的关联

git push origin master

> D:\Code\gittest>git remote -v
> origin  git@github.com:thinkaw/test.git (fetch)
> origin  git@github.com:thinkaw/test.git (push)

https://github.com/thinkaw/gitlearning

