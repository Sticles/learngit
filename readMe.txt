git add file 新增文件到暂缓区
git commit -m "版本描述"
git diff 比较本地开发代码和暂缓区代码的区别
git diff --cached 比较暂缓区代码和版本库代码的区别
git diff HEAD -- readMe.txt 比较本地开发代码和版本库代码的readMe.txt内容的区别
git checkout -- file 代码没有提交到暂缓区域时，如何放弃工作区代码的修改
git reset + 版本号 回退版本
git reset HEAD file 将暂缓区代码的修改撤销掉
git log --pretty=oneline 比较简洁的显示提交日志
git reflog 查看回退版本的操作日志

Git SSH Key 生成步骤:
一 、

设置Git的user name和email：

git config --global user.name "xuhaiyan"
git config --global user.email "haiyan.xu.vip@gmail.com"

二、生成SSH密钥过程：
1.查看是否已经有了ssh密钥：cd ~/.ssh
如果没有密钥则不会有此文件夹，有则备份删除
2.生存密钥：
$ ssh-keygen -t rsa -C “haiyan.xu.vip@gmail.com”
按3个回车，密码为空。


Your identification has been saved in /home/tekkub/.ssh/id_rsa.
Your public key has been saved in /home/tekkub/.ssh/id_rsa.pub.
The key fingerprint is:
………………


最后得到了两个文件：id_rsa和id_rsa.pub
3.添加密钥到ssh：ssh-add 文件名
需要之前输入密码。
4.在github上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥。

打开https://github.com/ ，登陆Sticles，然后添加ssh。
