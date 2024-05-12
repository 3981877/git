# git配置公钥和常用命令

git官网：https://git-scm.com/

github 生成key
在GitHub上生成SSH key的步骤如下：

打开终端（在Windows上可以使用Git Bash）。

输入以下命令生成新的SSH key：

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
将"your_email@example.com"替换为你的GitHub注册邮箱。

系统会提示你输入文件保存路径和文件名，如果你想直接按回车接受默认路径和文件名，则直接回车即可。

系统会让你输入密码，这个密码可以用于确保SSH key的安全，但如果你不想设置密码，直接按回车即可。

生成的SSH key保存在~/.ssh/id_rsa.pub（默认路径和文件名）。

使用以下命令查看SSH key：

cat ~/.ssh/id_rsa.pub
复制显示的SSH key内容。

登录GitHub网站，进入Settings -> SSH and GPG keys -> New SSH key，将复制的SSH key粘贴到Key文本框中，然后点击“Add SSH key”按钮保存。

完成以上步骤后，你就可以在本地使用SSH方式克隆GitHub上的仓库，以及无密码地推送和拉取代码。


# 说说常见的Git命令

1. git init： 初始化一个新的 Git 仓库
2. git clone：从远程仓库克隆代码到本地
3. git add： 将文件添加到 Git 的暂存区
4. git commit： 将暂存区的文件提交到本地仓库
5. git push： 将本地仓库的代码推送到远程仓库
6. git pull：从远程仓库拉取最新代码到本地
7. git branch：查看本地分支列表
8. git checkout： 切换分支
9. git merge： 将指定分支合并到当前分支
10. git status： 查看当前仓库状态
11. git log：查看提交历史记录
12. git reset： 撤销提交
13. git stash：将当前工作区的修改暂存起来
14. git tag：打标签，用于版本控制
15. git remote：管理远程仓库并到本地分支
16. git fetch：从远程仓库获取最新代码，但不合
17. git diff： 查看文件差异 
18. git revert：撤销指定提交
19. git rm： 从 Git 中删除文件
20. git config： 配置 Git 环境。
