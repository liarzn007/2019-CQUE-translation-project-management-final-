# 步骤二：添加一个新文件到仓库

接下来，使用你喜欢的任何文本编辑器或运行<font color="#6495ED">**touch**</font>命令将新文件添加到项目中。

在包含git仓库的文件夹中添加或修改文件后，git会注意到该仓库内部已进行了更改。 但是，除非你明确告知git，否则git不会正式跟踪该文件（即，执行提交命令，接下来我们将详细讨论提交）。

```htlm
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

 [gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com) 

```htlm
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

 [gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com) 

创建新文件后，可以使用<font color="#6495ED">**git status**</font>命令查看git知道存在的文件。

```htlm
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mnelson.txt

nothing added to commit but untracked files present (use "git add" to track)
```

 [gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com/) 

这基本上是说，“嘿，我们注意到你创建了一个名为 mnelson.txt 的文件。但除非你执行'git添加'命令，否则我们将不会对其进行任何处理。”



#### 一个小插曲:暂存环境、提交和操作者

初学git时最容易混淆的部分之一是暂存环境的概念及其与提交的关系。

<font color="#6495ED">**提交**</font>是自上次提交以来你更改了哪些文件的记录。 本质上，您可以对仓库进行更改（例如，添加文件或修改文件），然后告诉git对这些文件执行提交命令中。

提交构成了项目的本质，并允许您随时回到项目状态。

那么，如何告诉git提交哪些文件呢？ 这就是<font color="#6495ED">**暂存环境**</font>或<font color="#6495ED">**索引**</font>的引入。如步骤2所示，当您对仓库进行更改时，git会注意到文件已更改，但不会对其进行任何操作（例如在提交中添加文件）。

要将文件添加到提交中，首先需要将其添加到暂存环境中。 为此，您可以使用<font color="#6495ED">**git add** </font><filename>命令（请参见下面的步骤3）。

使用git add命令将所需的所有文件添加到暂存环境后，您可以使用<font color="#6495ED">**git commit** </font>命令告诉git将它们打包到提交中。

注意：暂存环境，也称为“暂存”，是新的首选术语，但你也可以将其称为“索引”。