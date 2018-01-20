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
git remote add origin git@github.com:Sticles/learngit.git 将本地git库关联到自己的github项目库上
git push (-u) origin master (首次)将本地库的内容推送到自己的github远程库
