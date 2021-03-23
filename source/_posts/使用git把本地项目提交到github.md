---
title: 使用git把本地项目提交到github
date: 2021-03-23 18:28:03
tags:
---

## 1. 安装git

[git下载地址](https://git-scm.com/downloads)

## 2. 本地git连接github账号

[本地git工具绑定github账号](./本地git工具绑定github账号.md)

## 3. 创建github仓库

创建仓库并**复制**仓库地址

![仓库名自取](使用git把本地项目提交到github/image-20210323183225770.png)

![创建完成](使用git把本地项目提交到github/image-20210323183327182.png)

## 4. 本地项目初始化并连接仓库

打开项目文件右键选择 `Git Bash Here`

![启动Git Bash](使用git把本地项目提交到github/image-20210323183608476.png)

初始化git，把这个文件夹变成Git可管理的仓库

```
git init
```

把本地项目与github仓库进行关联

```
git remote add origin {复制过来的仓库地址}
```

![没反应就是成功](使用git把本地项目提交到github/image-20210323183939139.png)

查看文件状态

```
git status
```

![红色为未添加到缓存区的文件](使用git把本地项目提交到github/image-20210323184056345.png)

把所有文件添加到缓存区

```
git add . #.代表所有文件
```

