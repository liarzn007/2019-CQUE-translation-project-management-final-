### 步骤10：将GitHub上的更改回馈到您的计算机

目前，GitHub上的资料库看起来与您本地计算机上的略有不同。例如，您在分支中做出并合并到主要分支中的提交在本地计算机上的主分支中不存在。

为了获得您或其他人在giHub上合并的最新更改，请使用**git Pull Origin Master****和**命令(在主分支上工作时)。

```
mnelson：myproject mnelson$git Pull Origin Master        
远程：对对象进行计数：1，完成。
远程：总计1(增量0)、重用0(增量0)、包重用0
解包对象：100%(1/1)，完成。
来自https://github.com/cubeton/mynewrepository
 *分支 主管 ->快点，快点。
   b345d9a..5381b7c主机->原点/母版
合并由递归的 / 循环的 策略。
 minelsons.txt | 1 +
 1个文件已更改，1个插入(+)
```

[视图原始](https://gist.github.com/cubeton/48b5c726b496d50c3975/raw/fe2c68e0988c467fd218587e2397552076355b52/pulloriginmaster.md)[pulloriginmaster.md](https://gist.github.com/cubeton/48b5c726b496d50c3975#file-pulloriginmaster-md) 由❤托管 [GitHub](https://github.com)

```
mnelson：myproject mnelson$git Pull Origin Master
远程：对对象进行计数：1，完成。
远程：总计1(增量0)、重用0(增量0)、包重用0
解包对象：100%(1/1)，完成。
来自https://github.com/cubeton/mynewrepository
 *分支 主管 ->快点，快点。
   b345d9a..5381b7c主机->原点/母版
合并由递归的 / 循环的 策略。
 minelsons.txt | 1 +
 1个文件已更改，1个插入(+)
```

[原始视图](https://gist.github.com/cubeton/48b5c726b496d50c3975/raw/fe2c68e0988c467fd218587e2397552076355b52/pulloriginmaster.md)[pulloriginmaster.md](https://gist.github.com/cubeton/48b5c726b496d50c3975#file-pulloriginmaster-md) 由❤托管 [GitHub](https://github.com/)

这将显示所有已更改的文件以及它们是如何更改的。

现在我们可以使用 [git log](http://git-scm.com/docs/git-log) 命令再次查看所有新提交。

(您可能需要将分支切换回主分支。您可以使用来执行此操作。) **git** **签出主机**` `命令)

```
mnelson:myproject mnelson$ git log
commit3e270876db0e5ffd3e9bfc5edede89b64b83812c
合并：4f1cb175381b7c
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep1117:48:112015-0400
 
    出现分支'主管' of https://github.com/cubeton/mynewrepository
 
commit4f1cb1798b6e6890da797f98383e6337df577c2a
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep 11 17:48:00 2015 -0400
 
    添加新文件夹
 
commit5381b7c53212ca92151c743b4ed7dde07d9be3ce
合并：:b345d9a1e8dc08
作者Meghan Nelson <meghan@meghan.net>
日期：   Fri Sep 11 17:43:22 2015 -0400
 
    Merge 拉取请求 #2 from cubeton/my-newbranch
    
    为文件夹添加更多文本
 
commit1e8dc0830b4db8c93efd80479ea886264768520c
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep 11 17:06:05 2015 -0400
 
    为文件夹添加更多文本
 
commit b345d9a25353037afdeaa9fcaf9f330effd157f1
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Thu Sep 10 17:42:15 2015 -0400
 
    这是我第一次提交!
```

[原始视图](https://gist.github.com/cubeton/48f55c5a237cd8e1a238/raw/3e31113a073b9bdec16800407d718b631dd0f587/gitlogaftermerge.md)[pulloriginmaster.md](https://gist.github.com/cubeton/48f55c5a237cd8e1a238#file-gitlogaftermerge-md) 由❤托管 [GitHub](https://github.com)

```
mnelson:myproject mnelson$ git log
commit3e270876db0e5ffd3e9bfc5edede89b64b83812c
合并：4f1cb175381b7c
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep1117:48:112015-0400
 
    出现分支'主管' of https://github.com/cubeton/mynewrepository
 
commit4f1cb1798b6e6890da797f98383e6337df577c2a
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep 11 17:48:00 2015 -0400
 
    添加新文件夹
 
commit5381b7c53212ca92151c743b4ed7dde07d9be3ce
合并：:b345d9a1e8dc08
作者Meghan Nelson <meghan@meghan.net>
日期：   Fri Sep 11 17:43:22 2015 -0400
 
    Merge 拉取请求 #2 from cubeton/my-newbranch
    
    为文件夹添加更多文本
 
commit1e8dc0830b4db8c93efd80479ea886264768520c
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Fri Sep 11 17:06:05 2015 -0400
 
    为文件夹添加更多文本
 
commit b345d9a25353037afdeaa9fcaf9f330effd157f1
作者Meghan Nelson <mnelson@hubspot.com>
日期：   Thu Sep 10 17:42:15 2015 -0400
 
    这是我第一次提交!
```

[view raw](https://gist.github.com/cubeton/48f55c5a237cd8e1a238/raw/3e31113a073b9bdec16800407d718b631dd0f587/gitlogaftermerge.md)[gitlogaftermerge.md](https://gist.github.com/cubeton/48f55c5a237cd8e1a238#file-gitlogaftermerge-md) hosted with ❤ by [GitHub](https://github.com/)

### 步骤11：徜徉在你的git中  

您已经成功地进行了公关，并将代码合并到主分支。恭喜！如果你想更深入了解，请点击 [这个Git101 文件夹](https://github.com/cubeton/git101/tree/master/TurtorialInfo) 更多使用方法 git and GitHub. 

我还建议找出一些时间与您的团队一起模拟一个较小的团队项目，就像我们在这里所做的那样。让您的团队使用您的团队名称创建一个新文件夹，并向其中添加一些带文本的文件。然后，尝试将这些更改推送到此远程回购。这样，您的团队就可以开始对他们最初没有创建的文件进行更改，并练习使用公关功能。而且，使用GitHub上的git指责和git历史工具来熟悉跟踪文件中进行了哪些更改以及是谁进行了这些更改。 

你用的GIT越多，你就会越熟练.。 别管它了。(我无法抗拒。)

![说明: IMG_265](file:///C:\Users\ADMINI~1\AppData\Local\Temp\msohtmlclip1\01\clip_image001.gif)

### 创作由[Meghan Nelson](https://product.hubspot.com/blog/author/meghan-nelson)