# 步骤五：创建一个新分支

现在，你已经进行了新的提交，让我们尝试一些更高级的东西。

假设你要制作新内容，但担心在制作时会对主项目进行更改。这时候纪要涉及到<font color="#6495ED">**git分支**</font>的内容。

分支允许你在项目的“状态”之间来回切换。 例如，如果要向网站添加新页面，则可以仅为该页面创建一个新分支，而不会影响项目的主要部分。 完成页面后，你可以将分支中的更改<font color="#6495ED">**合并**</font>到master分支中。 创建新分支时，Git会跟踪“分支”的提交情况，因此它知道所有文件的历史记录。

假设您在master分支上，并且想要创建一个新分支来开发你的网页。 您将执行以下操作：运行<font color="#6495ED">**git checkout -b <我的分支名称>**</font>。 该命令将自动创建一个新分支，并可以在该页面查看，这意味着git会将你移至该分支，脱离master分支。

运行上述命令后，可以使用<font color="#6495ED">**git分支**</font>已创建：

```html
mnelson:myproject mnelson$ git branch
  master
* my-new-branch
```

[gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com) 

```html
mnelson:myproject mnelson$ git branch
  master
* my-new-branch
```

 [gitbranch.md](https://gist.github.com/cubeton/fa25a25f322a2cd5f405#file-gitbranch-md) hosted with ❤ by [GitHub](https://github.com) 

分支名称旁边带有星号表示在给定时间指向的分支。

现在，如果您切换回master分支并进行更多提交，则在将这些更改<font color="#6495ED">**合并**</font>到新分支之前，你的新分支将看不到任何更改。