---
title: git操作指南
cover: /gallery/covers/git.png
date: 2021-09-01 07:21:10
categories:
  - 学习
  - 前端
tags:
  - 前端
---

Git个人操作手册。涵盖安装配置、仓库创建、基本用法（status/add/commit/log/checkout）、三种状态（modified/staged/committed）、tag标签、分支管理（branch/checkout/merge）、远程仓库（remote/push/pull）以及日常实践命令。

### **一、安装Git**

进入官网下载[git](https://www.git-scm.com/download/)

<!-- more -->

打开cmd

git –version //查看版本

### **二、配置**

git config –global user.name “huyinkai” //添加名字

git config –global user.email “[wohuyinkai@outlook.com](mailto:wohuyinkai@outlook.com)“ //添加邮箱

git config –list //查看当前设置项目

git config -l //简写

### **三、创建仓库**

git init //初始化仓库

git init demo //初始化一个叫demo的自定义文件夹

dir/a //查看当前所有目录

git done [url] //克隆GitHub项目

### **四、基本用法**

git status //查看仓库状态

git add . //将修改添加暂存区

git commit -m “说明” //给节点取一个名字

git log //查看所有节点

git checkout XXXXXXX //切换到此ID的版本

> 状态说明
> 
> git status //查看仓库状态
> 
> _NO commits yet //还没有提交
> 
> _Untracked file //存在未被追踪的文件
> 
> _Modified //存在未被追踪的已经修改的文件
> 
> _Changes to be committed //更改已被提交
> 
> _Nothing to commit,working tree clean. //没有可提交文件

### **五、三种状态**

git checkout - //回退到上一个节点

git log -p //修改的内容追加在log后面

> modified 已修改
> 
> staged 已暂存
> 
> committed 已提交
> 
> commit的内容是暂存区的内容（add操作），如果add之后有修改了内容，这次修改的内容不会被commit

### **六、tag标签**

git add . && git commit -m “说明” //组合命令

git log –oneline //查看所有节点只显示一行

git tag -a 标签名 -m “备注” //给节点打一个标签

git tag -a 标签名 -m “备注” XXXXXXX //给指定节点打一个标签

git show 标签名 //查看某个标签的详细信息

git checkout 标签名 //回溯至标签所在的提交

### **七、分支branch**

git branch 标签名 //创建分支

git checkout 标签名 //切换分支

git log -all –graph //图形化显示

### **八、合并分支**

git checkout -b 分支名 //创建并切换至分支

git merge 分支名 //合并分支

### **九、远程仓库**

git remote add 远程名称 远程地址 //添加远程仓库

例如：

> git remote add github <https://github.com/huyinkai/class.git>
> 
> git remote add origin <https://github.com/huyinkai/class.git>

git remote //列出所有远程仓库

例如：

> git remote get-url origin

git remote -v //详细信息

git push -u 远程名 分支名 //上传代码

例如：

> git push -u github master

### **十、远程合作**

git pull //获取远程更新

### **十一、实践使用**

git add .

git commit -m “说明”

git push -u origin master

git add . ; git commit -m “说明” ; git push -u origin master
