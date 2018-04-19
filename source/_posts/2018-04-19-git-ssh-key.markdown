---
layout: post
title: "git_ssh_key"
date: 2018-04-19 23:47:08 +0800
comments: true
categories:
---
# 管理电脑上的多个ssh key

为不同的网站（github、bitbucket、gitee）等：
`ssh-keygen -t rsa -C "yao.lu@sesamefin.com"`

编辑`~/.ssh/config`文件
```
Host github.com
  HostName github.com
  IdentityFile ~/.ssh/id_rsa
  PreferredAuthentications publickey
  User 467097950@qq.com

Host bitbucket.org
  HostName bitbucket.org
  IdentityFile ~/.ssh/id_rsa_sesame
  PreferredAuthentications publickey
  User yao.lu@sesamefin.com
```
