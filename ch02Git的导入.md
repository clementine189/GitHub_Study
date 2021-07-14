### 2.2什么是版本管理

git是分散型版本管理系统。

Fork就是将GitHub的某个特定仓库复制到自己的账户下。Fork出的仓库的原仓库是两个不同的仓库，开发者可以随意编辑。

在git中，本地开发环境中就有仓库，所以开发者不必连接远程仓库就可以进行开发。

实际上，所有仓库之间都可以进行push和pull。即便不通过GitHub，开发者A也可以直接向开发者B的仓库进行push或pull。

### 2.4初始设置

#### 设置姓名和邮箱地址

```
$git config --global user.name "clementine189"
$git config --global user.email "clementine189@163.com"

#通过下面的命令查看是否设置成功
$git config --list

```

