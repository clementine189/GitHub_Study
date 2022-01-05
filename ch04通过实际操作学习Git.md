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
  
  #touch ch05详细解说GitHub的功能.md
  #git status
  On branch master
  Your branch is up to date with 'origin/master'.
  
  Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
          modified:   "ch04\351\200\232\350\277\207\345\256\236\351\231\205\346\223\215\344\275\234\345\255\246\344\271\240Git.md"
  
  Untracked files:
    (use "git add <file>..." to include in what will be committed)
          "ch05\350\257\246\347\273\206\350\247\243\350\257\264GitHub\347\232\204\345\212\237\350\203\275.md"
  
  no changes added to commit (use "git add" and/or "git commit -a")
  
  #可以看到在Untracked files中显示了ch05详细解说GitHub的功能.md文件
  ```

- git add --向暂存区中添加文件

```shell
#如果只是用Git仓库的工作树创建了文件，那么该文件并不会被计入Git仓库的版本管理对象当中。因此上面新创建的文件会被显示在Untracked #files中。要想让文件成为Git仓库的管理对象，就需要git add命令及那个其加入暂存区（Stage或者Index）中。
#git add ch05详细解说GitHub的功能.md
#git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   "ch05\350\257\246\347\273\206\350\247\243\350\257\264GitHub\347\232\204\345\212\237\350\203\275.md"

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   "ch04\351\200\232\350\277\207\345\256\236\351\231\205\346\223\215\344\275\234\345\255\246\344\271\240Git.md"
#可以看到该文件显示在Changes to be committed中了
```

- git commit -- 保存仓库中的历史记录

  ```shell
  #git commit命令可以将当前暂存区中的文件实际保存到仓库的历史记录中。通过这些记录，我们就可以在工作树中复原文件
  
  ##记录第一行提交信息
  #git commit -m "first commit"
  [master 27ed21c] first commit
   1 file changed, 0 insertions(+), 0 deletions(-)
   create mode 100644 "ch05\350\257\246\347\273\206\350\247\243\350\257\264GitHub\347\232\204\345\212\237\350\203\275.md"
  #-m参数后的“first commit”称作提交信息，是对这个提交的概述
  
  ##记录详细提交信息
  
  
  ```

  