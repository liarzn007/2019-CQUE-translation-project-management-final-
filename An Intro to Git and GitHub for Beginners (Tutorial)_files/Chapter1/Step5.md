# Step5：创建一个新分支

现在，您已经进行了新的提交，让我们尝试一些更高级的东西。

假设您要制作一个新功能，但担心在开发功能时对主项目进行更改。这是git分支进入的地方。

分支允许您在项目的“状态”之间来回移动。例如，如果要向网站添加新页面，则可以仅为该页面创建一个新分支，而不会影响项目的主要部分。完成页面后，您可以将分支中的更改合并到master分支中。创建新分支时，Git会跟踪分支“分支”的提交，因此它知道所有文件的历史记录。

假设您在master分支上，并且想要创建一个新分支来开发您的网页。您将执行以下操作：运行git checkout -b <我的分支名称>。该命令将自动创建一个新分支，然后在其上“签出”，这意味着git会将您移至该分支，脱离master分支。

运行上述命令后，可以使用git branch命令来确认您的分支已创建：

```html
mnelson:myproject mnelson$ git branch
  master
* my-new-branch
```

[view raw](https://gist.github.com/cubeton/fa25a25f322a2cd5f405/raw/81033788d288adeffe260bd724ab2699b29e3e35/gitbranch.md)[gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com)

```html
mnelson:myproject mnelson$ git branch
  master
* my-new-branch
```

[view raw](https://gist.github.com/cubeton/fa25a25f322a2cd5f405/raw/81033788d288adeffe260bd724ab2699b29e3e35/gitbranch.md)[gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com/)

分支名称旁边带有星号表示在给定时间指向的分支。

现在，如果您切换回master分支并进行更多提交，则在将这些更改合并到新分支之前，您的新分支将看不到任何更改。