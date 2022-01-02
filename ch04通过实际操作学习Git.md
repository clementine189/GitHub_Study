### 4.1基本操作

- git init --初始化仓库

  ```shell
  #本地新创建一个项目
  #mkdir gitname
  #cd gitname
  #git init
  #如果初始化成功，执行力git init命令的目录下就会生成 .git目录。这个.git目录里存储着管理当前目录内容所需的仓库数据。
  #在Git中，我们将这个目录的内容称为“附属于该仓库的工作树”。文件的编辑等操作在工作树中进行，然后记录到仓库中，以此
  #管理文件的历史快照。如果想将文件回复到原先的状态，可以从仓库中调取之前的快照，在工作树中打开。开发者可以通过这种
  #方式获取以往的文件
  ```

- git status --查看仓库的状态

  ```shell
  #用于显示Git仓库的状态。工作树和仓库在被操作的过程中，状态会不断发生变化。
  #git status
  On branch master
  Your branch is up to date with 'origin/master'.
  
  nothing to commit, working tree clean
  
  #结果显示我们当前正处于master分支下。接着还显示了没有可提交的内容。
  ```

  