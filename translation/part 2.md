### 步骤2：在仓库里创建一个新文件夹

使用您喜欢的任何文本编辑器或运行`命令将新文件添加到项目中。`

在包含git repo的文件夹中添加或修改文件后，git会注意到该repo内部已进行更改。但是，除非您明确告诉它，否则git不会正式跟踪该文件（即将其放入提交中-接下来我们将进一步讨论提交）。

```
mnelson:myproject mnelson$ touch mnelson.txt
```

```
mnelson:myproject mnelson$ ls
```

```
mnelson.txt
```

[**view raw**](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[**addfile.md**](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [**GitHub**](https://github.com)

```
mnelson:myproject mnelson$ touch mnelson.txt
```

```
mnelson:myproject mnelson$ ls
```

```
mnelson.txt
```

[**view raw**](https://gist.github.com/cubeton/2d8f224bede4c2dde86b/raw/b865e27cc4715b3a3a4a5839e77ab232ff1b31f9/addfile.md)[**addfile.md**](https://gist.github.com/cubeton/2d8f224bede4c2dde86b#file-addfile-md) hosted with ❤ by [**GitHub**](https://github.com/)

 

创建新文件后，您可以使用"status'"命令查看git知道存在哪些文件。

```
mnelson:myproject mnelson$ git status
```

```
在分支机构主管
```

```
 
```

```
初次提交
```

```
 
```

```
未跟踪的文件：
```

```
  （使用“ git add <文件> ...”包括in将要提交的内容）
```

```
 
```

```
               mnelson.txt
```

```
 
```

```
没有添加任何内容提交但存在未跟踪的文件（使用“ git add”进行跟踪）
```

[**view raw**](https://gist.github.com/cubeton/02e849bbffcbea1e9a61/raw/71c93139666a8a4e06795f53c9aec5db95e6019a/gitstatus.md)[**gitstatus.md**](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [**GitHub**](https://github.com)

```
mnelson:myproject mnelson$ git status
```

```
在分支机构主管
```

```
 
```

```
初次提交
```

```
 
```

```
未跟踪的文件：
```

```
  （使用“ git add <文件> ...”包括in将要提交的内容）
```

```
 
```

```
               mnelson.txt
```

```
 
```

```
没有添加任何内容提交但存在未跟踪的文件（使用“ git add”进行跟踪）
```

[**view raw**](https://gist.github.com/cubeton/02e849bbffcbea1e9a61/raw/71c93139666a8a4e06795f53c9aec5db95e6019a/gitstatus.md)[**gitstatus.md**](https://gist.github.com/cubeton/02e849bbffcbea1e9a61#file-gitstatus-md) hosted with ❤ by [**GitHub**](https://github.com/)

这基本上是说：“嘿，我们注意到您创建了一个名为mnelson.txt的新文件，但是除非您使用'`gitadd'``命令，否则我们将不会对其进行任何处理。``”`

### 插曲：登台环境，提交和您

**初学git时最容易混淆的部分之一是暂存环境的概念及其与提交的关系。**

“提交”记录了自上次提交以来您更改了哪些文件。本质上，您可以对存储库进行更改（例如，添加文件或修改文件），然后告诉git将这些文件放入提交中。

提交构成了项目的本质，并允许您随时回到项目状态。

那么，如何告诉git提交哪些文件呢？**这是**[**“****临时环境”****或“****索引”**](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) **进入的地方。**如步骤2所示，当您对存储库进行更改时，git会注意到文件已更改，但不会对其进行任何操作（例如将其添加到提交中）。

**要将文件添加到提交中，首先需要将其添加到登台环境中。**为此，您可以使用[gitadd](http://git-scm.com/docs/git-add)**<****文件名****>** 命令（请参阅下面的步骤3）。

一旦使用了git add命令将所需的所有文件添加到暂存环境中，就可以使用gitcommit命令告诉git将它们打包为一个提交。 

注意：**暂存环境（也称为``暂存''）是此的新的首选术语，但您也可以将其称为”索引"。**

**初学git时最容易混淆的部分之一是暂存环境的概念及其与提交的关系。**

“提交”记录了自上次提交以来您更改了哪些文件。本质上，您可以对存储库进行更改（例如，添加文件或修改文件），然后告诉git将这些文件放入提交中。

提交构成了项目的本质，并允许您随时回到项目状态。

那么，如何告诉git提交哪些文件呢？**这是**[**“****临时环境”****或“****索引”**](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) **进入的地方。**如步骤2所示，当您对存储库进行更改时，git会注意到文件已更改，但不会对其进行任何操作（例如将其添加到提交中）。

**要将文件添加到提交中，首先需要将其添加到登台环境中。**为此，您可以使用[gitadd](http://git-scm.com/docs/git-add)**<****文件名****>** 命令（请参阅下面的步骤3）。

一旦使用了git add命令将所需的所有文件添加到暂存环境中，就可以使用gitcommit命令告诉git将它们打包为一个提交。 

注意：**暂存环境（也称为``暂存''）是此的新的首选术语，但您也可以将其称为”索引"。**

### 第三步:将文件添加到暂存环境

使用**gitadd**命令将文件添加到暂存环境。 

如果重新运行git status命令，则会看到git已将文件添加到登台环境中（请注意“要提交的更改“行）。  

```
mnelson:myproject mnelson$ git status
```

```
在分支机构主管
```

```
 
```

```
初次提交
```

```
 
```

```
所做更改：
```

```
  （使用“ git rm --cached <file> ...”取消登台）
```

```
 
```

```
               新文件：mnelson.txt
```

[查看由GitHub托管于❤的raw](https://gist.github.com/cubeton/28f7bea3b232f67e031c/raw/875157cd78d75c23f3f0e29bf0c97989e3d52937/addtostaging.md)[addtostaging.md](https://gist.github.com/cubeton/28f7bea3b232f67e031c#file-addtostaging-md)

```
mnelson:myproject mnelson$ git status
```

```
在分支机构主管
```

```
 
```

```
初次提交
```

```
 
```

```
所做更改：
```

```
  （使用“ git rm --cached <file> ...”取消登台）
```

```
 
```

```
               新文件：mnelson.txt
```

[查看由GitHub托管于❤的raw](https://gist.github.com/cubeton/28f7bea3b232f67e031c/raw/875157cd78d75c23f3f0e29bf0c97989e3d52937/addtostaging.md)[addtostaging.md](https://gist.github.com/cubeton/28f7bea3b232f67e031c#file-addtostaging-md)

 重申一下，该文件**尚未**添加到提交中，但是已经添加了。