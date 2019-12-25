### 步骤8：创建请求（PR）

拉取请求（或PR）是一种提醒存储库所有者要更改其代码的方式。它允许他们检查代码，并确保代码看起来不错，然后再将更改放入主分支。

这是提交PR页之前的样子：                                     

[![说明: Git_101_Screenshot_4.png](file:///C:\Users\acer\AppData\Local\Temp\msohtmlclip1\01\clip_image001.gif)](https://cloud.githubusercontent.com/assets/5241432/9189500/4688c07e-3fb7-11e5-99ed-d75b50ed9e48.png)

 

提交PR请求后的样子：

[![说明: Git_101_Screenshot_5.png](file:///C:\Users\acer\AppData\Local\Temp\msohtmlclip1\01\clip_image002.gif)](https://cloud.githubusercontent.com/assets/5241432/9189528/b39a7176-3fb7-11e5-87b1-7fed3e63b6bb.png)

 

您可能会在底部看到一个绿色的大按钮，上面显示“合并拉取请求”。点击这意味着您将您的更改合并到主分支中。

请注意，此按钮并非总是绿色。在某些情况下，它会是灰色的，这意味着您将面临“合并冲突”。 这是当一个文件中的更改与另一个文件中的更改冲突并且git无法确定要使用哪个版本时。您必须手动输入并告诉git使用哪个版本。

有时，您将成为回购的共同所有者或唯一所有者，在这种情况下，您可能无需创建PR来合并您的更改。但是，创建一个分支仍然是一个好主意，这样您可以保留更完整的更新历史记录并确保在进行更改时始终创建一个新分支。

##  步骤9：合并成一个PR

继续并单击绿色的“合并拉取请求”按钮。这会将您的更改合并到主分支中。

[![说明: Git_101_Screenshot_6.png](file:///C:\Users\acer\AppData\Local\Temp\msohtmlclip1\01\clip_image001.gif)](https://cloud.githubusercontent.com/assets/5241432/9189587/76631d98-3fb8-11e5-9fdb-17e7dec1c2a4.png)

 

完成之后，建议您删除分支（太多分支会变得凌乱），因此也请点击灰色的“删除分支”按钮。

您可以通过单击新存储库首页上的“提交”链接来仔细检查提交是否已合并。

![说明: Git_101_Screenshot_7.png](file:///C:\Users\acer\AppData\Local\Temp\msohtmlclip1\01\clip_image002.gif)

 

这将显示该分支中所有提交的列表。您可以看到我刚刚合并的那个（合并请求2）。

![说明: Git_101_Screenshot_8.png](file:///C:\Users\acer\AppData\Local\Temp\msohtmlclip1\01\clip_image003.gif)

**您还可以看到在右侧提交的**[**哈希代码**](https://git-scm.com/docs/git-hash-object) **。**哈希码是该特定提交的唯一标识符。**这对于引用特定的提交以及撤消更改很有用（使用**[**“ git revert”**](http://git-scm.com/docs/git-revert)` **<**``**哈希码编号**``**>**``**命令回溯）。**`

​                                                                        

​                                                                        