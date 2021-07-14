#### 问题：

在使用VSCode的git模块时，偶尔会因为网络问题，推送失败，包括ssl错误，连接失败错误

#### 解决办法：



```shell
#首先查看 http.sslVerify的值是否为false，如果为true或者是flase之类的拼写错误
$git config --list 
#修改设置，解除ssl验证。
$git config --global http.sslVerify “false”

#如果还是不行就是代理影响了git
$git config --global --unset http.proxy
$git config --global --unset https.proxy
```

执行了上述命令就没有问题了，在代理状态下，可以提交成功。

