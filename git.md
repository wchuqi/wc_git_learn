# 1 简介
集中式版本控制系统：CVS、SVN
Git：分布式版本控制系统

常用概念
- 工作区
- 缓存区
- 版本区
![git不同区示意图](vx_images/53333017235943.png =368x)

# 2 常用命令
```shell
查看git帮助
# git help git
# git help <command>
# git <command> --help

生成公钥私钥
~/.ssh
# ssh-keygen -t rsa -C "email"
~/.ssh/id_rsa
~/.ssh/id_rsa.pub
```

```shell
仓库初始化
# git init

添加仓库
# git remote -v
# git remote -vv
# git remote add <name> <remote-url>
# git remote remove <name>
```

```shell
文件处理
# git add .
# git add dir1/dir2/file1
# git add dir1/dir2/*

提交
# git commit -m "commit log"

拉取
# git pull [name]
# git fetch <name>
# git fetch --all


推送
# git push -u origin master

移除文件
# git rm <file>
```

```shell
撤消操作
# git commit --amend
# git reset HEAD <file>
# git checkout -- <file>

查看状态
# git status

比较操作
# git diff --cached
```
[撤消操作](https://git-scm.com/book/zh/v2/Git-基础-撤消操作)

```shell
commit点操作
# git checkout 
```

```shell
版本回退
# git reset --hard head^
# git reset --hard head^^^
# git reset --hard <commitid>
```

```shell
log查看
# git log
# git log <--revert> -1
# git log --pretty=oneline

所有操作
# git reflog
```

# 参考文档
- [最好看官方文档](https://git-scm.com/book/zh/v2)


# 常见的坑
- 带有.git目录的都被git识别为仓库
- 