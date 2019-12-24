# 步骤二  添加一个新文件到repo

使用您喜欢的任何文本编辑器或运行触摸命令，继续向项目添加新文件。

在包含git repo的文件夹中添加或修改文件之后，git将注意到在repo中进行了更改。但是，除非您明确地要求git跟踪文件(也就是说，将其放入提交—我们接下来将更多地讨论提交)，否则git不会正式跟踪文件。

```
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

[view raw](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[addfile.md](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [GitHub](https://github.com)

```
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

[view raw](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[addfile.md](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [GitHub](https://github.com/)

 创建新文件之后，可以使用git status命令查看git知道哪些文件存在。

```
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mnelson.txt

nothing added to commit but untracked files present (use "git add" to track)
```

[view raw](https://gist.github.com/cubeton/02e849bbffcbea1e9a61/raw/71c93139666a8a4e06795f53c9aec5db95e6019a/gitstatus.md)[gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com)

这基本上是说，“嘿，我们注意到您创建了一个名为mnelson的新文件。txt，但除非你使用'git添加'命令，否则我们不会对它做任何事情。”

#### 一个小插曲:暂存环境、提交和操作者

当您第一次学习git时，最容易混淆的部分之一是暂存环境的概念以及它与提交的关系。

提交是您自上次提交以来更改的文件的记录。本质上，您可以修改您的repo(例如，添加一个文件或修改一个文件)，然后告诉git将这些文件放入提交。

提交构成了项目的本质，允许您在任何时候返回到项目的状态。

那么，如何告诉git将哪些文件放入提交呢?这就是暂存环境或索引的用武之地。正如在步骤2中所看到的，当您对repo进行更改时，git会注意到文件已经更改，但是不会对其进行任何操作(比如在提交中添加它)。

要将文件添加到提交，首先需要将其添加到暂存环境。为此，可以使用git add <filename>命令(参见下面的步骤3)。</filename>

使用git add命令将所有需要的文件添加到暂存环境之后，可以使用git commit命令告诉git将它们打包到一个提交中。

注意:暂存环境(也称为“staging”)是对此的新首选术语，但您也可以将其称为“索引”。

