# git command Project for github testing

# create github repository

touch README.md 

git init 

git add README.md 

git commit -m “first commit” 

git remote add origin https://github.com/HairanWu/gitcommand.git

git push -u origin master

# create tag
git branch

git tag

git tag -a v0.1 -m "version 0.1 released"

git show v0.1

git push origin v1.0

git push origin --tags

git tag -d v0.1

# create branch

git checkout -b dev

git branch dev

git checkout dev

# Command 
git branch <new-branch>        # 创建新分支

git push <remote_name> <local_branch>:<remote_branch>  # 将新建分支push到远端

git pull <remote_name> <remote_branch>:<local_branch> # 将远程指定分支拉取到本地指定分支上

git checkout <branbch_name>         # 切换到指定分支

git checkout -b <branbch_name>  # 创建并切换到新分支

git merge <branch_name> 　　         # 将指定分支合并到当前分支

git branch -d <branch_name>    # 删除指定分支

git checkout -b [branch] [remote_name]/[branch]   #  设置跟踪分支

git branch -vv    // 查看本地分支跟踪的远程分支

git branch [-u]/[--set-upstream-to] [remote_name]/[branch] # 修改正在跟踪的上游分支


git branch --track [branch] [remote-branch]  # 新建一个分支，与指定的远程分支建立追踪关系

git push [remote_name] --delete  [branch_name]     # 删除指定远程分支

#Git如何拉取指定远程分支
(1) 直接拉取
git clone -b dev 代码仓库地址 （dev是分支名称）

(2) 分支拉取
git init 进行初始化

*与远程代码仓库建立连接：git remote add origin 代码仓库地址）

*将远程分支拉到本地：git fetch origin <remote_branch>

*创建本地分支：git checkout -b <local_branch> <remote_name/remote_branch> 

git pull origin <remote_branch>

（3）子模块
git submodule init
git submodule update