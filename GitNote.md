# GitNote

[TOC]

## git使用简单指南

https://www.bootcss.com/p/git-guide/

### 1.开始

**创建**

```
git init
git remote add origin <server>
```

**检出仓库**（就不用remote了）

```
git clone
```

### 2.简单工作

![image-20210810153925370](GitNote.assets/image-20210810153925370.png)

**添加到缓存区**

```
git add <filename>
git add .
```

**添加到HEAD**

```
git commit -m "代码提交信息"
```

**推送到远程**

```
git push origin <branch>
```

### 3.分支

![image-20210810154819264](GitNote.assets/image-20210810154819264.png)

**创建**

```
git checkout -b feature_x
```

**切换**

```
git checkout master
```

**删除**

```
git branch -d feature_x
```

### 4.更新与合并

**更新到最新改动**

```
git pull
```

**查看区别**

```
git diff <source_branch> <target_branch>
```

**合并其他分支到当前分支**

```
git merge <branch>
```

### 5.替换本地改动

**使用HEAD中的最新内容替换你的工作目录中的文件**

```
git checkout -- <filename>
```

**丢弃所有的本地改动与提交，到服务器上获取最新的版本并将本地主分支指向它**

```
git fetch origin
git reset --hard origin/master
```

### 6.标签

**执行如下命令以创建一个叫做 *1.0.0* 的标签**

```
git tag 1.0.0 1b2e1d63ff
```

**使用如下命令获取提交 ID**

```
git log
```

你也可以用该提交 ID 的少一些的前几位，只要它是唯一的

## Pro Git详细深入

https://git.oschina.net/progit/