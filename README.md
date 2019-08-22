# gitskills
##概要
*something about git skills*
**参考文献**：[Git教程](https://www.liaoxuefeng.com/wiki/896043488029600)

##创建版本库
在需要创建版本库的目录下输入：`$ git init`

##把文件添加到版本库
-第一步:将文件添加到暂存区(`stage`)
   `$ git add <file>`
-第二步：将暂存区的所有内容提交到当前分支
   `$ git commit -m "message"`

##查看git当前状态
   `$ git status`

##远程仓库
需要在GitHub上add `SSH keys`

###添加远程库
  -第一步：在`GitHub`上创建仓库（*此时此仓库为空*）
  -第二步：在本地git仓库下运行命令：`$ git remote add origin git@<github link>`
  -第三步：将本地库的内容推送到远程：`$ git push -u origin master`

   Ps:由于远程库是空的，我们第一次推送`master`分支时，加上了`-u`参数，Git不但会把本地的`master`分支内容推送的远程新的`master`分支，还会把本地的`master`分支和远程的`master`分支关联起来，在以后的推送或者拉取时就可以简化命令。

###从远程库克隆
   `$ git clone git@<github link>`