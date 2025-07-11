[Git](https://zh.wikipedia.org/wiki/Git)：https://git-scm.com/

macOS上使用[Xcode Command Line Tools](https://www.freecodecamp.org/news/install-xcode-command-line-tools/)，即`xcode-select --install`安装Apple供应的版本

若已安装Homebrew，则可以使用`brew`替换上面的版本，即：

```shell
# 安装前
% git --version
git version 2.39.5 (Apple Git-154)
% brew install git
# 安装并重启终端后
% git --version
git version 2.50.1
```

# Git常用命令

配置用户名：`git config --global user.name xhxjwz`

配置邮箱：`git config --global user.email xhxjwz@outlook.com`

配置初始分支名：`git config --global init.defaultBranch`

添加远程仓库：`git remote add origin https://github.com/OWNER/REPOSITORY.git`

检查远程仓库：`git remote -v`

更改远程仓库：`git remote set-url https://github.com/OWNER/REPOSITORY.git`

[重新初始化](https://blog.axiaoxin.com/post/reset-git-history/)（一种方式）：

```shell
% git checkout --orphan new_branch
% git add -A
% git commit -m "Messages"
% git branch -D old_branch
# rename new_branch to main
% git branch -m main
# override remote repository
% git push --force origin main
```

# GitHub

## 注册

> [!WARNING]
>
> 在填写完信息进入人机验证时，不要选择Visual Puzzling，建议选择Audio Puzzling。如果刷新出来简单的验证能较快结束验证，而前者必须实打实完成十个，对眼睛非常不友好。

打开<https://github.com/>，根据网站上的信息完成注册。

## 入门

[官方帮助文档](https://docs.github.com/zh)

