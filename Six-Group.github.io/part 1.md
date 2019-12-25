### part 1

# ***\*Git和GitHub入门指南（教程）\****

2015年10月1日 / 作者[MEGHAN NELSON](https://product.hubspot.com/blog/author/meghan-nelson)

· 

· 分享

· 

8月，我们在HubSpot主持了一次《女性代码见面会》，并开展了针对初学者的使用git和GitHub的研讨会。我首先浏览了有关git的 [基础知识](https://www.slideshare.net/HubSpot/git-101-git-and-github-for-beginners) 和背景的``幻灯片演示''，然后我们分成几个小组来运行我创建的教程来模拟大型协作项目的工作。活动结束后我们得到了反馈，它是一个实用的动手介绍。因此，如果您也是git的新手，请按照以下步骤操作以轻松更改代码库，打开拉取请求（PR）并将代码合并到master分支中。任何重要的git和GitHub术语均以粗体显示，并带有官方git参考资料的链接。 

##  ***\*准备工作：\****安装git并创建一个GitHub帐户 

安装git并创建一个GitHub帐户

请按照 [此处的](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 说明安装git（如果没有安装的话）***\*请注意，对于本教程，我们将仅在命令行上使用git。\****尽管有一些很棒的git GUI（图形用户界面），但我认为先使用git特定的命令学习git，然后在更熟悉该命令后尝试git GUI会更容易。 

完成此操作后, 在此处创建[一个GitHub的账户](https://github.com/join).（公共存储库是免费的，但私人存储库是收费的。）

安装git并创建一个GitHub帐户

请按照 [此处的](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 说明安装git（如果没有安装的话）***\*请注意，对于本教程，我们将仅在命令行上使用git。\****尽管有一些很棒的git GUI（图形用户界面），但我认为先使用git特定的命令学习git，然后在更熟悉该命令后尝试git GUI会更容易。 

完成此操作后, 在此处创建[一个GitHub的账户](https://github.com/join).（公共存储库是免费的，但私人存储库是收费的。）

## 步骤1***\*创建本地git存储库\**** 

***\*使用git在本地计算机上创建新项目时，首先要创建一个新项目\****[***\*的仓库\****](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository) (短时间的, '***\*仓库\****', ). 

要使用git，我们将使用终端。如果您对终端和基本命令没有太多经验，请查看[这份教程](http://mac.appstorm.net/how-to/utilities-how-to/how-to-use-terminal-the-basics/) （尤其是“导航文件系统”和“移动”部分）。

首先，打开一个终端，然后使用￼cd￼（更改目录）命令移动到要在本地计算机上放置项目的位置。例如，如果您的桌面上有一个'项目'文件夹，则可以执行以下操作：

mnelson:Desktop mnelson$ cd ~/Desktop

mnelson:Desktop mnelson$ mkdir myproject

mnelson:Desktop mnelson$ cd myproject/

[***\*view raw\****](https://gist.github.com/cubeton/67a84eb876984f0b5785/raw/d4560016d742865c1fd68d97fcff1feb557d5e19/terminalcd.md)[***\*terminalcd.md\****](#file-terminalcd-md) hosted with ❤ by [***\*GitHub\****](https://github.com)

mnelson:Desktop mnelson$ cd ~/Desktop

mnelson:Desktop mnelson$ mkdir myproject

mnelson:Desktop mnelson$ cd myproject/

[***\*view raw\****](https://gist.github.com/cubeton/67a84eb876984f0b5785/raw/d4560016d742865c1fd68d97fcff1feb557d5e19/terminalcd.md)[***\*terminalcd.md\****](#file-terminalcd-md) hosted with ❤ by [***\*GitHub\****](https://github.com/)

 

***\*要在文件夹的根目录中初始化git存储库，请运行\****[***\*git init\****](http://git-scm.com/docs/git-init) 命令: 

mnelson:myproject mnelson$ git init

Initialized empty Git repository in /Users/mnelson/Desktop/myproject/.git/

[***\*view raw\****](https://gist.github.com/cubeton/89793ba1bc947f64658e/raw/f3dba1dd72fda5eeb98b761338aedfc310d29d54/gitinit.md)[***\*gitinit.md\****](#file-gitinit-md) hosted with ❤ by [***\*GitHub\****](https://github.com)

mnelson:myproject mnelson$ git init

Initialized empty Git repository in /Users/mnelson/Desktop/myproject/.git/

[***\*view raw\****](https://gist.github.com/cubeton/89793ba1bc947f64658e/raw/f3dba1dd72fda5eeb98b761338aedfc310d29d54/gitinit.md)[***\*gitinit.md\****](#file-gitinit-md) hosted with ❤ by [***\*GitHub\****](https://github.com/)
