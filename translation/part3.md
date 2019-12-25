### 步骤4：创建提交

您是时候创建第一次提交了！

运行命令`git commit -m“``关于提交的消息``”`

```
mnelson:myproject mnelson$ git commit -m "This is my first commit!"
```

```
[master (root-commit) b345d9a] This is my first commit!
```

```
 1 file changed, 1 insertion(+)
```

```
 create mode 100644 mnelson.txt
```

[**view raw**](https://gist.github.com/cubeton/1068d965d147b4039e4d/raw/5c3262c3f6e3c28328ba57ea33c512dbab149fcf/commit.md)[**commit.md**](https://gist.github.com/cubeton/1068d965d147b4039e4d#file-commit-md) hosted with ❤ by [**GitHub**](https://github.com)

```
mnelson:myproject mnelson$ git commit -m "This is my first commit!"
```

```
[master (root-commit) b345d9a] This is my first commit!
```

```
 1 file changed, 1 insertion(+)
```

```
 create mode 100644 mnelson.txt
```

[**view raw**](https://gist.github.com/cubeton/1068d965d147b4039e4d/raw/5c3262c3f6e3c28328ba57ea33c512dbab149fcf/commit.md)[**commit.md**](https://gist.github.com/cubeton/1068d965d147b4039e4d#file-commit-md) hosted with ❤ by [**GitHub**](https://github.com/)

提交末尾的消息应该与提交所包含的内容有关-可能是一项新功能，可能是一个错误修复，也许只是在修复输入错误。不要放置“ asdfadsf”或“ foobar”之类的消息。这使看到您的承诺的其他人感到悲伤。非常非常伤心。



### 步骤5：创建新分支

现在您进行了新的提交，让我们尝试一些更高级的东西。

假设您要制作新功能，但担心在开发功能时对主项目进行更改。这是 **git分支** 出现的地方 

分支允许您在项目的“状态”之间来回移动。例如，如果您想在网站上添加新页面，则可以仅为该页面创建一个新分支，而不会影响项目的主要部分。完成页面后，您可以将更改从分支[合并](http://git-scm.com/docs/git-merge) 到master分支。当您创建一个新分支时，Git会跟踪分支提交的分支，因此它知道所有文件的历史记录。 

假设您在master分支上，并且想要创建一个新分支来开发您的网页。以下是你需要做的：运行 **git checkout -b <我的分支名称>**.该命令将自动创建一个新分支，然后在其上“签出”，这意味着git会将您移至该分支，脱离master分支。

在运行上述命令之后，您可以使用[git 分支](http://git-scm.com/docs/git-branch) 命令来确定您的分支已创建：

```
mnelson:myproject mnelson$ git branch
```

```
  master* my-new-branch
```

[view raw](https://gist.github.com/cubeton/fa25a25f322a2cd5f405/raw/81033788d288adeffe260bd724ab2699b29e3e35/gitbranch.md)[gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com)

```
mnelson:myproject mnelson$ git branch
```

```
  master* my-new-branch
```

[view raw](https://gist.github.com/cubeton/fa25a25f322a2cd5f405/raw/81033788d288adeffe260bd724ab2699b29e3e35/gitbranch.md)[gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com/)

分支名称旁边带有星号表示在给定时间指向的分支。 

现在，如果您切换回master分支并进行更多提交，则在您将这些更改[合并](http://git-scm.com/docs/git-merge) 到新分支之前，新分支将看不到任何更改。