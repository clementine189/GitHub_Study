### 1.1什么是GitHub

GitHub和Git的区别

在Git中，开发者将源代码存入名叫“Git仓库”的资料库中并加以使用。

GitHub则是在网络上提供Git仓库的一项服务。



GitHub上公开的软件源代码全都由Git进行管理。理解Git，是熟练运用GitHub的关键所在。



### 1.2使用GitHub会带来哪些变化

- #### 在开发者之间引发化学反应的Pull Request

Pull Request是指开发者在本地对源代码进行更改后，向GitHub中托管的Git仓库请求合并的功能。开发者还可以在这个功能中进行讨论交流。

通过这个功能，开发者可以轻松更改源代码，并公开更改的细节，然后向仓库提交合并请求。

- #### 对特定用户进行评论

任务管理和BUG报告可以通过Issue进行交互。

- #### GitHub Flavored Markdown

### 1.3社会化编程

随着GitHub的出现，软件开发者们才真正意义上拥有了源代码。

ps：当有人向你请求代码时，不妨给他github链接



世界上任何人都可以比以前更加容易地获得源代码，将其自由更改并加以公开。

### 1.4为什么需要社会化编程

GitHub最大的特征是“面向人”

### 1.5GitHub提供的主要功能

- Git仓库

- Organization

- Issue

  Issue功能，是将一个任务或问题分配给一个Issue进行追踪或管理的功能。在GitHub上，每当进行我们即将讲解的PullRequest，都会同时创建一个Issue。

  每一个功能更改或修正都对应一个Issue，讨论或修正都以这个Issue为中心进行。只要查看Issue，就能知道和这个更改相关的一切信息，并以此进行管理。

  ```
  #这里创建了第一个Issue，在GitHub_Study.git中，内容是日常学习，在学习《GitHub入门与实践》的日常中，提交笔记都需要在提交信息中加上Issue的ID（#1），GitHub就会自动生成从Issue到对应的提交链接。
  ```

  

- Wiki

通过Wiki功能，任何人都能随时对一篇文章进行更改并保存，因此可以多人共同完成一篇文章。该功能常用在开发文档或手册的编写中。

Wiki页也是作为Git仓库进行管理的，改版的历史纪录会被切实保存下来，使用者可以放心改写。

- PullRequest

开发者向GitHub的仓库推送更改或功能添加后，可以通过Pull Request功能向别人的仓库提出申请，请求对方合并。

```shell
#实验：实践一次pull request
1.主账号：clementine189，有一个公开仓库learngit
2.注册另一个账号：luotongwx，去主账号下fork了learngit仓库，稍作修改
3.在luotongwx/learngit下做一些修改，然后发起一次PullRequest
4.在clementine189/learngit中可以看到这次请求，接受合并请求

```

