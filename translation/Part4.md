### 步骤6：建立新仓库

如果您只想在本地保存密码足迹，那么就不必使用Github但如果您想团队合作，那么您可以用Github合作修改项目密码

 

如果您想在Github创立新仓库，请先登录Github点击首页您将看到一个绿色的“+新仓库”按钮 

![Git_101_Screenshot1-2.png](file:///C:\Users\ASUS\AppData\Local\Temp\msohtmlclip1\01\clip_image001.gif)

 

 

 

 

 

点击该按钮，Github将会让您命名新仓库并给您提供一个简介

![Git_101_Screenshot_2-1.png](file:///C:\Users\ASUS\AppData\Local\Temp\msohtmlclip1\01\clip_image002.gif)

 

 

 

 

 

 

 

 

 

 

 

 

当您完成信息填写后，请点击“创立仓库”按钮，创立新仓库

Github将询问您是否想重新创建一个新仓库，还是想添加一个本地创立的仓库在本例中，由于我们已经在本地创建了一个新的回购，因此我们希望将其推送到Gihub上，以便遵循**.或从命令行部分推送**现有存储库： 

```
mnelson:myproject mnelson$ git remote add origin https://github.com/cubeton/mynewrepository.git
mnelson:myproject mnelson$ git push -u origin master
Counting objects:3, done.
Writing objects:100% (3/3), 263 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
```

[**view raw**](https://gist.github.com/cubeton/3a2616c44e35ca68a6b0/raw/41e5758cfdbd7db8a1659c1adaba9346680097f9/addgithub.md)[**addgithub.md**](https://gist.github.com/cubeton/3a2616c44e35ca68a6b0#file-addgithub-md) hosted with ❤ by [**GitHub**](https://github.com)

```
mnelson:myproject mnelson$ git remote add origin https://github.com/cubeton/mynewrepository.git
mnelson:myproject mnelson$ git push -u origin master
Counting objects:3, done.
Writing objects:100% (3/3), 263 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
```

[**view raw**](https://gist.github.com/cubeton/3a2616c44e35ca68a6b0/raw/41e5758cfdbd7db8a1659c1adaba9346680097f9/addgithub.md)[**addgithub.md**](https://gist.github.com/cubeton/3a2616c44e35ca68a6b0#file-addgithub-md) hosted with ❤ by [**GitHub**](https://github.com/)

 (您需要将第一个命令行中的URL更改为本节中GitHub列出的URL，因为您的GitHub用户名和repo名称不同。)

 

### 步骤7:将分支推送到GitHub

现在，我们将把您分支中的提交到您的新GitHub回购 **推送** 到您的新GitHub回购 这样，其他人就可以看到您所做的更改如果它们得到存储库所有者的批准，则可以将更改合并到主分支中

要将更改推送到GitHub上的新分支，您需要运行**[\**git push\**](http://git-scm.com/docs/git-push)** **origin yourbranchname**`**.**`` `GitHub会自动在远程存储库上为您创建分支： 

```
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects:3, done.
Delta compression using up to 8 threads.
Counting objects:100%(2/2), done.
Writing objects:100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
```

[**view raw**](https://gist.github.com/cubeton/bf8274609c344b6d0e70/raw/4764e740cac9a48eefad341d9e34ceb09f89b73f/addnewbranchgithub.md)[**addgithub.md**](https://gist.github.com/cubeton/bf8274609c344b6d0e70#file-addnewbranchgithub-md) hosted with ❤ by [**GitHub**](https://github.com)

```
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects:3, done.
Delta compression using up to 8 threads.
Counting objects:100%(2/2), done.
Writing objects:100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
```

[**view raw**](https://gist.github.com/cubeton/bf8274609c344b6d0e70/raw/4764e740cac9a48eefad341d9e34ceb09f89b73f/addnewbranchgithub.md)[**addgithub.md**](https://gist.github.com/cubeton/bf8274609c344b6d0e70#file-addnewbranchgithub-md) hosted with ❤ by [**GitHub**](https://github.com/)

 您可能想知道上面命令中的“起源”这个词是什么意思发生的情况是，当您将远程存储库克隆到本地计算机时，Git会创建一个 **别名**为您在几乎所有情况下，此别名都称为"[原点](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)."它本质上是远程存储库的URL的简写**因此，要将更改推送到远程存储库，您可以使用以下命令****:** `git push git@github.com:git/git.git yourbranchname` 或者`git push origin yourbranchname`

(如果这是您第一次在本地使用GitHub，可能会提示您使用GitHub用户名和密码登录。)

如果您刷新GitHub页面，您将看到一条注释，上面写着使用您的名字的分支刚刚被推入存储库中您也可以单击“分支机构”链接，查看那里列出的分支机构

[![Git_101_Screenshot2.png](file:///C:\Users\ASUS\AppData\Local\Temp\msohtmlclip1\01\clip_image003.gif)](https://cloud.githubusercontent.com/assets/5241432/9189475/da30eb86-3fb6-11e5-934f-ca596a2cac69.png)

现在单击上面屏幕截图中的绿色按钮我们要提出！ **撤退请求**！

 

