# 项目分工安排

## 项目经理

黎莹莹（1610205221）[github账号：Leeyingying0915] 

主要负责fork任务，对任务进行预处理，然后在GitHub中创建小组，并合理的给小组成员分配任务，以便可以高效的完成整个任务。

## 翻译人员及审校人员

黎莹莹1610205221（Leeyingying0915）

张富晏1610202251（zhangfuyan)

曾钰婷1610202251(Yoko-zeng)

舒杰1610602272(SUZY1214)

刘山1610403114(Liushan-unique) 

田兴清1610403118(tianxingqing)

## 项目安排计划表

| 2019年12月22日 | 项目经理在客户处fork需要翻译的文件                           |
| -------------- | ------------------------------------------------------------ |
| 2019年12月22日 | 项目经理整合需要翻译的资料，并在GitHub上面创建小组           |
| 2019年12月22日 | 项目经理分布任务给小组成员                                   |
| 2019年12月23日 | 小组译员开始集中翻译                                         |
| 2019年12月23日 | 小组审校人员对译文进行审校，审校完成和提交到小组内，并在GitHub里创建issue |
| 2019年12月23日 | 项目经理merge译员的翻译，并对译文进行整合                    |
| 2019年12月24日 | 项目经理再次核查翻译                                         |
| 2019年12月25日 | 由项目经理提交给客户                                         |

## 项目实施流程

| 2019.12.22 | 小组成员安装GitHub Desktop登陆账号                           |
| ---------- | ------------------------------------------------------------ |
| 2019.12.22 | 项目经理fork项目并创建翻译小组                               |
| 201912.23  | 项目经理分配任务，每个成员分别建立自己的分支，然后pull request交给项目经理 |
| 2019.12.23 | 审校人员审校翻译人员的翻译作品，并反馈信息，同时可以各自创建issue共同讨论 |
| 2019.12.24 | 翻译人员修改翻译并重新提交给项目经理，项目经理merge翻译      |
| 2019.12.24 | 项目经理整合翻译，并进行再次检查                             |
| 2019.12.25 | 项目经理提交翻译项目给客户                                   |

## 平行文本

| Document                                                     | 文件                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Welcome to the Hexo documentation.                           | 欢迎使用 Hexo，本文档将帮助您快速上手。                      |
| If you encounter any problems when using Hexo, have a look at the[troubleshooting guide](https://hexo.io/docs/troubleshooting), raise an issue on [GitHub](https://github.com/hexojs/hexo/issues) or start a topic on the [Google Group](https://groups.google.com/group/hexo). | 如果您在使用过程中遇到问题，请查看 [问题解答](https://hexo.io/zh-cn/docs/troubleshooting) 中的解答，或者在 [GitHub](https://github.com/hexojs/hexo/issues)、[Google Group](https://groups.google.com/group/hexo) 上提问。 |
| What is Hexo?                                                | 什么是 Hexo？                                                |
| Hexo is a fast, simple and powerful blog framework. You write posts in [Markdown](http://daringfireball.net/projects/markdown/) (or other markup languages) and Hexo generates static files with a beautiful theme in seconds. | Hexo 是一个快速、简洁且高效的博客框架。  Hexo 使用 [Markdown](http://daringfireball.net/projects/markdown/)（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。 |
| Installation                                                 | 安装                                                         |
| It only takes a few minutes to set up Hexo. If you encounter a problem and can’t find the solution here, please [submit a GitHub issue](https://github.com/hexojs/hexo/issues) and we’ll help. | 安装 Hexo 只需几分钟时间，若您在安装过程中遇到问题或无法找到解决方式，请[提交问题](https://github.com/hexojs/hexo/issues)，我们会尽力解决您的问题。 |
| Requirements                                                 | 安装前提                                                     |
| Installing Hexo is quite easy and only requires the following beforehand: | 安装 Hexo 相当简单，只需要先安装下列应用程序即可：           |
| [Node.js](http://nodejs.org/) (Should be at least Node.js 8.10, recommends 10.0 or higher) | (Node.js 版本需不低于 8.10，建议使用 Node.js 10.0 及以上版本) |
| Git                                                          | Git                                                          |
| If your computer already has these, congratulations! You can skip to the [Hexo installation](https://hexo.io/docs/index.html#Install-Hexo) step. | 如果您的电脑中已经安装上述必备程序，那么恭喜您！你可以直接前往 [安装 Hexo](https://hexo.io/zh-cn/docs/index.html#%E5%AE%89%E8%A3%85-Hexo) 步骤。 |
| If not, please follow the following instructions to install all the requirements. | 如果您的电脑中尚未安装所需要的程序，请根据以下安装指示完成安装。 |
| Install Git                                                  | 安装Git                                                      |
| Install Node.js                                              | 安装Node.js                                                  |
| Node.js provides [official installer](https://nodejs.org/en/download/) for most platforms. | Node.js 为大多数平台提供了官方的 [安装程序](https://nodejs.org/en/download/)。 |
| Windows                                                      | Windows 用户                                                 |
| If you use the official installer, make sure **Add to PATH** is checked (it’s checked by default). | 使用 Node.js 官方安装程序时，请确保勾选 **Add to PATH** 选项（默认已勾选） |
| Mac / Linux                                                  | For Mac / Linux 用户                                         |
| If you encounter `EACCES` permission error when trying to install Hexo, please follow [the workaround](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally)provided by npmjs; overriding with root/sudo is highly discouraged. | 如果在尝试安装 Hexo 的过程中出现 `EACCES` 权限错误，请遵循 [由 npmjs 发布的指导](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally) 修复该问题。强烈建议 **不要** 使用 root、sudo 等方法覆盖权限 I |
| Install Hexo                                                 | 安装 Hexo                                                    |
| Once all the requirements are installed, you can install Hexo with npm: | 所有必备的应用程序安装完成后，即可使用 npm 安装 Hexo。       |
| Advanced installation and usage                              | 进阶安装和使用                                               |
| Advanced users may prefer to install and use `hexo` package instead. | 对于熟悉 npm 的进阶用户，可以仅局部安装 `hexo` 包。          |
| Once installed, you can run Hexo in two ways:                | 安装以后，可以使用以下两种方式执行 Hexo：                    |
| `npx hexo <command>`  Linux users can set relative path of `node_modules/` folder: | `npx hexo <command>`  将 Hexo 所在的目录下的 `node_modules` 添加到环境变量之中即可直接使用 `hexo <command>`： |
| Setup                                                        | 建站                                                         |
| Once Hexo is installed, run the following commands to initialize Hexo in the target `<folder>`. | 安装 Hexo 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。 |
| _config.yml                                                  | _config.yml                                                  |
| Site [configuration](https://hexo.io/docs/configuration) file. You can configure most settings here. | 网站的 [配置](https://hexo.io/zh-cn/docs/configuration) 信息，您可以在此配置大部分的参数。 |
| package.jsonpackage.json                                     | package.jsonpackage.json                                     |
| Application data. The [EJS](https://ejs.co/), [Stylus](http://learnboost.github.io/stylus/) and [Markdown](http://daringfireball.net/projects/markdown/) renderers are installed by default. If you want, you can uninstall them later. | 应用程序的信息。[EJS](https://ejs.co/), [Stylus](http://learnboost.github.io/stylus/) 和 [Markdown](http://daringfireball.net/projects/markdown/) renderer 已默认安装，您可以自由移除 |
| scaffolds                                                    | scaffolds                                                    |
| [Scaffold](https://hexo.io/docs/writing#Scaffolds) folder. When you create a new post, Hexo bases the new file on the scaffold. | [模版](https://hexo.io/zh-cn/docs/writing) 文件夹。当您新建文章时，Hexo 会根据 scaffold 来建立文件。 |
| source                                                       | 资源                                                         |
| Source folder. This is where you put your site’s content. Hexo ignores hidden files and files or folders whose names are prefixed with `_` (underscore) - except the `_posts` folder. Renderable files (e.g. Markdown, HTML) will be processed and put into the `public` folder, while other files will simply be copied. | 资源文件夹是存放用户资源的地方。除 `_posts` 文件夹之外，开头命名为 `_` (下划线)的文件 / 文件夹和隐藏的文件将会被忽略。Markdown 和 HTML 文件会被解析并放到 `public` 文件夹，而其他文件会被拷贝过去 |
| themes                                                       | 主题                                                         |
| [Theme](https://hexo.io/docs/themes) folder. Hexo generates a static website by combining the site contents with the theme. | [主题](https://hexo.io/zh-cn/docs/themes) 文件夹。Hexo 会根据主题来生成静态页面。 |
| Configuration                                                | 配置                                                         |
| You can modify site settings in `_config.yml` or in an [alternate config file](https://hexo.io/docs/configuration#Using-an-Alternate-Config). | 您可以在 `_config.yml` 中修改大部分的配置。                  |
| Include/Exclude Files or Folders                             | 包括或不包括目录和文件                                       |
| Use the following options to explicitly process or ignore certain files/folders. Support [glob expressions](https://github.com/micromatch/micromatch#extended-globbing) for path matching. | 在 Hexo 配置文件中，通过设置 include/exclude 可以让 Hexo 进行处理或忽略某些目录和文件夹。 |
| `include` and `exclude` options only apply to the `source/` folder, whereas `ignore` option applies to all folders. | 你可以使用 [glob 表达式](https://github.com/isaacs/minimatch) 对目录和文件进行匹配。 |
| Each value in the list must be enclosed with single/double quotes. | 列表中的每一项都必须用单引号或双引号包裹起来。               |
| `include:` and `exclude:` do not apply to the `themes/` folder. Either use `ignore:` or alternatively, prepend an underscore to the file/folder name to exclude. | `include` 和 `exclude` 并不适用于 `themes/` 目录下的文件。如果需要忽略 `themes/` 目录下的部分文件或文件夹，可以使用 `ignore` 或在文件名之前添加下划线 `_`。 |
| Using an Alternate Config                                    | 使用代替配置文件                                             |
| A custom config file path can be specified by adding the `--config` flag to your `hexo` commands with a path to an alternate YAML or JSON config file, or a comma-separated list (no spaces) of multiple YAML or JSON files. | 可以在 hexo-cli 中使用 `--config` 参数来指定自定义配置文件的路径。你可以使用一个 YAML 或 JSON 文件的路径，也可以使用逗号分隔（无空格）的多个 YAML 或 JSON 文件的路径。例如： |
| Overriding Theme Config                                      | 覆盖主题配置                                                 |
| Hexo themes are independent projects, with separate `_config.yml` files. | 通常情况下，Hexo 主题是一个独立的项目，并拥有一个独立的 `_config.yml` 配置文件。 |
| Instead of forking a theme, and maintaining a custom branch with your settings, you can configure it from your site’s primary configuration file. | 你可以在站点的 `_config.yml` 配置文件中配置你的主题，这样你就不需要 fork 一份主题并维护主题独立的配置文件。 |

## 项目要求

### 项目流程要求

\1. 项目建立和实施各个步骤需按照既定实施计划表严格执行

\2. 小组成员需齐心协力去完成翻译项目

\3. 翻译过程中出现问题需提出来，以便及时解决，提高工作效率

### 翻译质量要求：

#### 译前要求

\1. 平行文本需要找一个与翻译文本类似的文本，而且翻译的类容也应术语科技类。

\2. 翻译软件统一使用MemoQ

\3. 熟读需要翻译的内容

#### 译中要求

\1. 术语不允许译错

\2. 格式需按照既定的格式翻译

\3. 不会翻的内容需要按照积极查询、小组讨论、确定译文这一流程翻译

\4. 数字翻译统一哦翻译成阿拉伯数字

\5. 网页代码中出现的英文不需要翻译

\6. 组员需全部参与翻译和审校过程，期间确保翻译术语的统一和译文的准确性

#### 译后要求

\1. 翻译完成后译员需对译文进行一次审查，发现问题及时修改

\2. 针对审校提出的问题，对自己的译文积极修改

\3. 译员需及时完成翻译并提交，审校人员需对译文提出合理意见并及时反馈给译员，以确保翻译流程及时有效进行。

## 术语表

| E-N                                                    | C-N                                                  |
| ------------------------------------------------------ | ---------------------------------------------------- |
| 第一部分                                               |                                                      |
| index                                                  | 索引                                                 |
| a pull request (PR)                                    | 拉取请求                                             |
| links                                                  | 链接                                                 |
| git GUIs (graphical user interfaces)                   | git GUI（图形用户界面）                              |
| public repositories                                    | 公共存储库                                           |
| private repositories                                   | 私人存储库                                           |
| Create a local git repository                          | 创建本地git存储库                                    |
| Navigating the Filesystem                              | 导航文件系统                                         |
| a git repository in the root of the   folder           | 文件夹的根目录                                       |
| 第二部分                                               |                                                      |
| text editor                                            | 文本编辑器                                           |
| Initial commit                                         | 初次提交                                             |
| Untracked files:                                       | 未跟踪的文件：                                       |
| staging environment                                    | 临时环境                                             |
| index                                                  | 索引                                                 |
| 第三部分                                               |                                                      |
| the asterisk                                           | 星号                                                 |
| mnelson:myproject mnelson$ git branch                  | mnelson:myproject mnelson$ git branch                |
| "asdfadsf" or   "foobar".                              | "asdfadsf" or "foobar".                              |
| a bug fix                                              | 一个错误修复                                         |
| 第四部分                                               |                                                      |
| mnelson:myproject mnelson$ git push -u   origin master | mnelson:myproject mnelson$ git push -u origin master |
| GitHub username                                        | GitHub用户名                                         |
| a remote repository                                    | 远程存储库                                           |
| screenshot                                             | 屏幕截图                                             |
| 第五部分                                               |                                                      |
| the PR page                                            | PR页                                                 |
| Merge pull request                                     | 合并拉取请求                                         |
| merge conflict                                         | 合并冲突                                             |
| hash code                                              | 拼凑代码                                             |
| undoing changes                                        | 撤消更改                                             |
| hash code number                                       | 拼凑码编号                                           |
| command to backtrack                                   | 命令回溯                                             |
| 第六部分                                               |                                                      |
| remote:                                                | 远程：                                               |
| Total 1 (delta 0), reused 0 (delta 0),   pack-reused 0 | 总计1(增量0)、重用0(增量0)、包重用0                  |
| Unpacking objects:                                     | 解包对象：                                           |
| view raw                                               | 视图原始                                             |
| insertion(+)                                           | 插入(+)                                              |
| git checkout master                                    | git 签出主机                                         |
| mnelson:myproject mnelson$ git log                     | mnelson:myproject mnelson$ git log                   |
| the PR feature                                         | 公关功能                                             |

## 所遇困难及解决方法

| 所遇困难                     | 解决方法                                                     |
| ---------------------------- | ------------------------------------------------------------ |
| 软件使用不熟悉               | 询问操作熟悉的同学，然后慢慢练习                             |
| 个别单词翻译苦难             | 针对不会翻译的单词，先在字典上面查询，查询未果的就在网上查询，最后再在得到的译文翻译中进行筛选得到满意的翻译 |
| 平行文本难找                 | 完全匹配的平行文本无法找到，就找了一份与之文本类型相似的文本 |
| 流程过于复杂                 | 针对这一问题，只有带着组员多熟悉流程，理解其内在逻辑，然后再多练。 |
| 专业术语翻译                 | 多查多问多总结                                               |
| 代码中出现英文单词需要翻译吗 | 项目要求中提出可以不用翻译                                   |
| 译文格式的改动               | 与源语文本格式相同                                           |
