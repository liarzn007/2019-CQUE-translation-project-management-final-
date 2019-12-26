# 步骤三:将文件添加到暂存环境

使用git add命令将文件添加到暂存环境。

如果重新运行git status命令，则会看到git已将文件添加到暂存环境（请注意“要提交的更改”行）。

```htlm
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   mnelson.txt
```

[addtostaging.md](https://gist.github.com/cubeton/28f7bea3b232f67e031c#file-addtostaging-md) hosted with ❤ by [GitHub](https://github.com)

```htlm
mnelson:myproject mnelson$ git status
On branch master

Initial commit

Changes to be :
  (use "git rm --cached <file>..." to unstage)

	new file:   mnelson.txt
```

[addtostaging.md](https://gist.github.com/cubeton/28f7bea3b232f67e031c#file-addtostaging-md) hosted with ❤ by [GitHub](https://github.com/)

重申一下，该文件尚**未**添加到提交中，但即将添加到提交中。