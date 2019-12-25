# 步骤七：将分支推送到GitHub

现在，我们将分支中的提交**推送到**新的GitHub存储库。 这使其他人可以看到您所做的更改。 如果它们是由存储库所有者批准的，则可以将更改合并到主（master）分支中。

要将更改推送到GitHub上的新分支，您需要运行<font color="#6495ED">**git push origin**</font>**您的分支名称**。 GitHub将在远程存储库上自动为您创建分支：

```html
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
```

[addnewbranchgithub.md](https://gist.github.com/cubeton/bf8274609c344b6d0e70#file-addnewbranchgithub-md) hosted with ❤ by [GitHub](https://github.com) 

```
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
```

[addnewbranchgithub.md](https://gist.github.com/cubeton/bf8274609c344b6d0e70#file-addnewbranchgithub-md) hosted with ❤ by [GitHub](https://github.com/) 

您可能想知道上面命令中“起源”一词的含义。 当您将远程存储库克隆到本地计算机时，git为您创建了一个**别名**。 在几乎所有情况下，此别名都称为<font color="#6495ED">**“来源”**</font>。它实质上是远程存储库URL的简写。 因此，要将更改推送到远程存储库，可以使用以下命令：**git push git@github.com：git / git.git yourbranchname或git push origin yourbranchname**

（如果这是您第一次在本地使用GitHub，可能会提示您使用GitHub用户名和密码登录。）

刷新GitHub页面后，您会看到注释，说您的名字的分支刚刚被推送到存储库中。 您也可以单击“分支”链接以查看此处列出的分支。

![Git_101_Screenshot1-2](assets/Git_101_Screenshot1-2.webp)

现在，单击上方屏幕快照中的绿色按钮。 我们将提出合并请求！