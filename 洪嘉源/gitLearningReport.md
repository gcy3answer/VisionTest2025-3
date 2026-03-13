## Git 常用指令
### 初始设置
1. git init 初始化仓库
2. git clone <repo_url> 克隆远程仓库
3. git config --global user.name 设置用户名
4. git config --global user.email 设置邮箱地址
### 状态与提交改变
1. git status 查看目录状态
2. git add <file> 组织文件
3. git add . 组织所有文件
4. git commit -m "message" 提交更改
### 分支管理
1. git branch 列出本地分支
2. git branch <name> 创建新的分支
3. git checkout <name> 切换分支
4. git merge <branch> 合并指定分支到当前分支
5. git branch -d <name> 删除分支
## PR 流程
1. fork 目标仓库。
2. 使用git clone 部署到本地
3. 进入本地目录，使用git remote add upstream [url]添加原始仓库
4. 使用git fetch upstream拉取原始仓库的更新
5. 使用git checkout master和git merge upstream/master替换到主分支并合并更新
6. 提交git push origin master
