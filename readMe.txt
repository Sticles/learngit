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
git branch 查看分支
git branch dev 创建分支dev
git checkout dev 切换到分支dev
git merge dev 合并分支dev到master
git branch -d dev 删除分支dev
git merge --no-ff -m "merge with no-ff" dev 禁用Fast forword模式下合并dev分支代码到主线，会创建一次commit操作
git log --graph --pretty=oneline --abbrev-commit 查看分支合并图
git stash 储藏工作环境修改代码
git stash list 查看现场存储列表
git stash apply  stash@{0}  恢复到存储工作状态
git stash drop stash@{0} 删除现场存储状态stash@{0}
git stash pop 等同于git stash apply + git stash drop
git clone git@github.com:michaelliao/gitskills.git 克隆远程库内容到本地 
要从远程库克隆内容到本地首先要配置ssh-key
