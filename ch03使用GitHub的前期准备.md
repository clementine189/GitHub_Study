### 3.1使用前的准备

- 设置SSH Key

GitHub上连接已有仓库时的认证，是通过使用了SSH的公开密钥认证方式进行的。

```
$ssh-keygen -t rsa -C "clementine189@163.com"

id_rsa文件是私有密钥
id_rsa.pub是公开密钥
```

- 添加公开密钥

### 3.2实际动手使用

```
#clone仓库，
$git clone git@github.com:clementine189/learngit.git

#查看状态
$git status

#假设增加了文件hello.cpp 提交至仓库
#git add命令将文件加入暂存区，再通过git commit命令提交
$git add hello.cpp
$git commit -m "Add hello"

#查看提交日志
$git log

#执行push，GitHub上的仓库就会被更新，这是一种简写模式，不建议使用，详情请见ch04
$git push
```

