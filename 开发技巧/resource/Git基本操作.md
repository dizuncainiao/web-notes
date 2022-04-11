# Git 基本操作

[TOC]

### 设置用户名和邮箱

```shell
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```

此设置可以在 `Git` 历史中看到你的提交信息。

### 生成 ssh 密钥

使用 `https url` 克隆对初学者来说会比较方便，复制 `https url` 然后到 _git Bash_ 里面直接用 `clone` 命令克隆到本地。
但是每次 `fetch` 和 `push` 代码都需要输入账号和密码，这也是 `https` 方式的麻烦之处。
而使用 `ssh url` 克隆却需要在克隆之前先配置和添加好 `ssh key`。

```shell
$ ssh-keygen -t rsa -C "你的邮箱"
```

一路回车即可生成 `RSA` 加密的 `ssh key`。一般情况下，在 `C:\Users\Administrator\.ssh` 目录下查看生成的密钥。
`Github` 在 Setting 中添加密钥后，即可使用 `ssh url` 克隆仓库。

![image-20220411153937897](..\images\开发技巧\image-20220411153937897.png)



### 遇到了其他问题？

1. [Git 上传代码报错 ssh: connect to host github.com port 22: Connection timed out 解决办法](https://blog.csdn.net/qq_42146613/article/details/82772734) 
2. [其他操作请参考——廖雪峰Git教程](https://www.liaoxuefeng.com/wiki/896043488029600) 

