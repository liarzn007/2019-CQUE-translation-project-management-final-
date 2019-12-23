# Step2 将新文件添加到仓库

1. 继续，使用您喜欢的任何文本编辑器或运行touch命令将新文件添加到项目中。

2. 在包含git repo的文件夹中添加或修改文件后，git会注意到该repo内部已进行了更改。 但是，除非您明确告知git，否则git不会正式跟踪该文件（即，将其放入提交中-接下来我们将详细讨论提交）。

```html
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

[view raw](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[addfile.md](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [GitHub](https://github.com)

```html
mnelson:myproject mnelson$ touch mnelson.txt
mnelson:myproject mnelson$ ls
mnelson.txt
```

[view raw](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[addfile.md](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [GitHub](https://github.com/)

3. 创建新文件后，可以使用git status命令查看git知道存在的文件。

```html
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mnelson.txt

nothing added to commit but untracked files present (use "git add" to track)
view rawgitstatus.md hosted with ❤ by GitHub

```

[view raw](https://gist.github.com/cubeton/02e849bbffcbea1e9a61/raw/71c93139666a8a4e06795f53c9aec5db95e6019a/gitstatus.md)[gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com)

```html
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mnelson.txt

nothing added to commit but untracked files present (use "git add" to track)
view rawgitstatus.md hosted with ❤ by GitHub
```

[view raw](https://gist.github.com/cubeton/02e849bbffcbea1e9a61/raw/71c93139666a8a4e06795f53c9aec5db95e6019a/gitstatus.md)[gitstatus.md](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [GitHub](https://github.com/)

4. 这基本上是说：“嘿，我们注意到您创建了一个名为mnelson.txt的新文件，但是除非您使用'git add'命令，否则我们将不会对其进行任何处理。”

5. 插曲：

   过渡环境，提交和您初学git时最容易混淆的部分之一是暂存环境的概念及其与提交的关系。

   提交是自上次提交以来您更改了哪些文件的记录。本质上，您可以对存储库进行更改（例如，添加文件或修改文件），然后告诉git将这些文件放入提交中。

   提交构成了项目的本质，并允许您随时回到项目状态。

   那么，如何告诉git提交哪些文件呢？这就是暂存环境或索引的引入。如步骤2所示，当您对存储库进行更改时，git会注意到文件已更改，但不会对其进行任何操作（例如在提交中添加文件）。

   要将文件添加到提交中，首先需要将其添加到登台环境中。为此，您可以使用git add <filename>命令（请参见下面的步骤3）。

   使用git add命令将所需的所有文件添加到暂存环境后，您可以使用git commit命令告诉git将它们打包到提交中。

   注意：暂存环境，也称为“暂存”，是此的新的首选术语，但您也可以将其称为“索引”。