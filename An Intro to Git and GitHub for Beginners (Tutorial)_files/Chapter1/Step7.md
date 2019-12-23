# Step7将分支推送到GitHub

现在，我们将分支中的提交推送到新的GitHub存储库。 这使其他人可以看到您所做的更改。 如果它们是由存储库所有者批准的，则可以将更改合并到master分支中。

要将更改推送到GitHub上的新分支，您需要运行git push origin您的分支名称。 GitHub将在远程存储库上自动为您创建分支：

```
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
addnewbranchgithub.md hosted with ❤ by GitHub
```

```
mnelson:myproject mnelson$ git push origin my-new-branch
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cubeton/mynewrepository.git
 * [new branch]      my-new-branch -> my-new-branch
view rawaddnewbranchgithub.md hosted with ❤ by GitHub
```

您可能想知道上面命令中“起源”一词的含义。 发生的事情是，当您将远程存储库克隆到本地计算机时，git为您创建了一个别名。 在几乎所有情况下，此别名都称为“来源”。 它实质上是远程存储库URL的简写。 因此，要将更改推送到远程存储库，可以使用以下命令：git push git@github.com：git / git.git yourbranchname或git push origin yourbranchname

（如果这是您第一次在本地使用GitHub，则可能会提示您使用GitHub用户名和密码登录。）

如果刷新GitHub页面，您会看到注释，说您的名字的分支刚刚被推送到存储库中。 您也可以单击“分支”链接以查看此处列出的分支。

![Git_101_Screenshot2](C:\Users\Administrator\Desktop\gitbook summer\2019-CQUE-translation-project-management-final-\附件2 translation project\An Intro to Git and GitHub for Beginners (Tutorial)_files\Git_101_Screenshot2.webp)现在，单击上方屏幕快照中的绿色按钮。 我们将提出拉取请求！