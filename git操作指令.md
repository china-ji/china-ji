# git本地仓库 操作
1. 创建仓库 git init
1. 提交到暂存区 git add 文件夹或文件名称  .代表全部文件
1. 提是把暂存区的所有内容提交到当前分支   git commit -m '提交的描述'
1. 查看提交记录 git log
1. 回退版本 git reset --hard commit_id
1.  丢弃工作区没有提交的代码 git checkout -- gitdemo.html
1. 丢弃暂存区的代码  git reset HEAD 文件名   再  git checkout -- 文件名
1. 查看分支 git branch
1. 创建分支 git branch 分支名
1. 切换分支 git checkout 分支名
1. 创建+切换分支：git checkout -b
1. 合并某分支到当前分支：git merge
1. 删除分支：git branch -d
> 注意 切换dev分支后，不修改master的代码，就不会冲突。 修改master 之后 合并dev分支代码就会发生冲突。 解决冲突，只需要在vscode开发工具中 选择代码合并方式即可。

# git 设置ssh

> ssh-keygen -t rsa -C "173794464@qq.com"

> cat ~/.ssh/id_rsa.pub

> 将生成的密钥 添加到gitee仓库中，就可以使用ssh地址 克隆和提交项目了

# git 远程仓库操作
1. 克隆 git clone 地址
> 注意：项目组给你一个项目链接，你就克隆到本地
1. 查看远程地址 git remote -v 
1. 删除远程链接 git remote remove origin
1. 添加远程地址：git remote add origin 
1. 同步远程 git pull origin master  
1. 第一次推送 master 分支的所有内容 git push -u origin master 




