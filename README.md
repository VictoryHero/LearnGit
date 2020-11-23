Table of Contents
=================

* [Table of Contents](#table-of-contents)
  * [本地仓库基础](#%E6%9C%AC%E5%9C%B0%E4%BB%93%E5%BA%93%E5%9F%BA%E7%A1%80)
      * [初始化仓库](#%E5%88%9D%E5%A7%8B%E5%8C%96%E4%BB%93%E5%BA%93)
      * [配置姓名和邮箱](#%E9%85%8D%E7%BD%AE%E5%A7%93%E5%90%8D%E5%92%8C%E9%82%AE%E7%AE%B1)
      * [添加修改到暂存区](#%E6%B7%BB%E5%8A%A0%E4%BF%AE%E6%94%B9%E5%88%B0%E6%9A%82%E5%AD%98%E5%8C%BA)
      * [查看工作区状态](#%E6%9F%A5%E7%9C%8B%E5%B7%A5%E4%BD%9C%E5%8C%BA%E7%8A%B6%E6%80%81)
      * [提交修改到本地仓库](#%E6%8F%90%E4%BA%A4%E4%BF%AE%E6%94%B9%E5%88%B0%E6%9C%AC%E5%9C%B0%E4%BB%93%E5%BA%93)
      * [查看本地仓库提交记录](#%E6%9F%A5%E7%9C%8B%E6%9C%AC%E5%9C%B0%E4%BB%93%E5%BA%93%E6%8F%90%E4%BA%A4%E8%AE%B0%E5%BD%95)
  * [远程仓库基础](#%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93%E5%9F%BA%E7%A1%80)
      * [clone远程仓库](#clone%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93)
      * [添加远程仓库](#%E6%B7%BB%E5%8A%A0%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93)
      * [推送本地内容到远程仓库](#%E6%8E%A8%E9%80%81%E6%9C%AC%E5%9C%B0%E5%86%85%E5%AE%B9%E5%88%B0%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93)
      * [拉取远程内容到本地仓库](#%E6%8B%89%E5%8F%96%E8%BF%9C%E7%A8%8B%E5%86%85%E5%AE%B9%E5%88%B0%E6%9C%AC%E5%9C%B0%E4%BB%93%E5%BA%93)
  * [分支](#%E5%88%86%E6%94%AF)
      * [创建分支](#%E5%88%9B%E5%BB%BA%E5%88%86%E6%94%AF)
      * [切换分支](#%E5%88%87%E6%8D%A2%E5%88%86%E6%94%AF)
      * [删除本地分支](#%E5%88%A0%E9%99%A4%E6%9C%AC%E5%9C%B0%E5%88%86%E6%94%AF)
      * [删除远程分支](#%E5%88%A0%E9%99%A4%E8%BF%9C%E7%A8%8B%E5%88%86%E6%94%AF)
      * [本地分支合并](#%E6%9C%AC%E5%9C%B0%E5%88%86%E6%94%AF%E5%90%88%E5%B9%B6)
      * [远程分支合并](#%E8%BF%9C%E7%A8%8B%E5%88%86%E6%94%AF%E5%90%88%E5%B9%B6)
  * [历史与撤销](#%E5%8E%86%E5%8F%B2%E4%B8%8E%E6%92%A4%E9%94%80)
      * [git log进阶](#git-log%E8%BF%9B%E9%98%B6)
      * [git revert实现版本回滚](#git-revert%E5%AE%9E%E7%8E%B0%E7%89%88%E6%9C%AC%E5%9B%9E%E6%BB%9A)
      * [git reset实现版本回退](#git-reset%E5%AE%9E%E7%8E%B0%E7%89%88%E6%9C%AC%E5%9B%9E%E9%80%80)
      * [git checkout 撤销工作区更改](#git-checkout-%E6%92%A4%E9%94%80%E5%B7%A5%E4%BD%9C%E5%8C%BA%E6%9B%B4%E6%94%B9)
      * [git reset 撤销暂存区更改](#git-reset-%E6%92%A4%E9%94%80%E6%9A%82%E5%AD%98%E5%8C%BA%E6%9B%B4%E6%94%B9)
      * [git rm 删除or屏蔽文件](#git-rm-%E5%88%A0%E9%99%A4or%E5%B1%8F%E8%94%BD%E6%96%87%E4%BB%B6)
  * [标签](#%E6%A0%87%E7%AD%BE)
      * [创建标签](#%E5%88%9B%E5%BB%BA%E6%A0%87%E7%AD%BE)
        * [(1)不含附注的标签](#1%E4%B8%8D%E5%90%AB%E9%99%84%E6%B3%A8%E7%9A%84%E6%A0%87%E7%AD%BE)
        * [(2)包含附注的标签](#2%E5%8C%85%E5%90%AB%E9%99%84%E6%B3%A8%E7%9A%84%E6%A0%87%E7%AD%BE)
      * [查看标签](#%E6%9F%A5%E7%9C%8B%E6%A0%87%E7%AD%BE)
      * [查看标签附注](#%E6%9F%A5%E7%9C%8B%E6%A0%87%E7%AD%BE%E9%99%84%E6%B3%A8)
      * [推送标签到远程仓库](#%E6%8E%A8%E9%80%81%E6%A0%87%E7%AD%BE%E5%88%B0%E8%BF%9C%E7%A8%8B%E4%BB%93%E5%BA%93)
        * [(1)推送指定标签](#1%E6%8E%A8%E9%80%81%E6%8C%87%E5%AE%9A%E6%A0%87%E7%AD%BE)
        * [(2)推送全部标签](#2%E6%8E%A8%E9%80%81%E5%85%A8%E9%83%A8%E6%A0%87%E7%AD%BE)
      * [删除本地标签](#%E5%88%A0%E9%99%A4%E6%9C%AC%E5%9C%B0%E6%A0%87%E7%AD%BE)
      * [删除远程标签](#%E5%88%A0%E9%99%A4%E8%BF%9C%E7%A8%8B%E6%A0%87%E7%AD%BE)
  * [忽略文件](#%E5%BF%BD%E7%95%A5%E6%96%87%E4%BB%B6)
      * [创建忽略文件](#%E5%88%9B%E5%BB%BA%E5%BF%BD%E7%95%A5%E6%96%87%E4%BB%B6)
      * [忽略文件格式](#%E5%BF%BD%E7%95%A5%E6%96%87%E4%BB%B6%E6%A0%BC%E5%BC%8F)
  * [配置别名](#%E9%85%8D%E7%BD%AE%E5%88%AB%E5%90%8D)
      * [设置别名](#%E8%AE%BE%E7%BD%AE%E5%88%AB%E5%90%8D)
      * [查看别名](#%E6%9F%A5%E7%9C%8B%E5%88%AB%E5%90%8D)
      * [删除别名](#%E5%88%A0%E9%99%A4%E5%88%AB%E5%90%8D)
  * [冲突与强制](#%E5%86%B2%E7%AA%81%E4%B8%8E%E5%BC%BA%E5%88%B6)
      * [冲突的产生](#%E5%86%B2%E7%AA%81%E7%9A%84%E4%BA%A7%E7%94%9F)
        * [(1)内容冲突](#1%E5%86%85%E5%AE%B9%E5%86%B2%E7%AA%81)
        * [(2)树冲突](#2%E6%A0%91%E5%86%B2%E7%AA%81)
      * [解决冲突](#%E8%A7%A3%E5%86%B3%E5%86%B2%E7%AA%81)
        * [(1)内容冲突](#1%E5%86%85%E5%AE%B9%E5%86%B2%E7%AA%81-1)
        * [(2)树冲突](#2%E6%A0%91%E5%86%B2%E7%AA%81-1)
      * [强制操作](#%E5%BC%BA%E5%88%B6%E6%93%8D%E4%BD%9C)
  * [变基](#%E5%8F%98%E5%9F%BA)
      * [merge和rebase的不同](#merge%E5%92%8Crebase%E7%9A%84%E4%B8%8D%E5%90%8C)
      * [分支变基](#%E5%88%86%E6%94%AF%E5%8F%98%E5%9F%BA)
      * [分支变基冲突](#%E5%88%86%E6%94%AF%E5%8F%98%E5%9F%BA%E5%86%B2%E7%AA%81)
  * [储藏](#%E5%82%A8%E8%97%8F)
      * [储藏的概念](#%E5%82%A8%E8%97%8F%E7%9A%84%E6%A6%82%E5%BF%B5)
      * [实现保存](#%E5%AE%9E%E7%8E%B0%E4%BF%9D%E5%AD%98)
      * [查看保存](#%E6%9F%A5%E7%9C%8B%E4%BF%9D%E5%AD%98)
      * [应用保存](#%E5%BA%94%E7%94%A8%E4%BF%9D%E5%AD%98)
  * [搭建本地Git服务器](#%E6%90%AD%E5%BB%BA%E6%9C%AC%E5%9C%B0git%E6%9C%8D%E5%8A%A1%E5%99%A8)
      * [安装并配置git](#%E5%AE%89%E8%A3%85%E5%B9%B6%E9%85%8D%E7%BD%AEgit)
          * [安装git](#%E5%AE%89%E8%A3%85git)
          * [创建一个用户用来运行git服务的用户](#%E5%88%9B%E5%BB%BA%E4%B8%80%E4%B8%AA%E7%94%A8%E6%88%B7%E7%94%A8%E6%9D%A5%E8%BF%90%E8%A1%8Cgit%E6%9C%8D%E5%8A%A1%E7%9A%84%E7%94%A8%E6%88%B7)
          * [创建证书登录](#%E5%88%9B%E5%BB%BA%E8%AF%81%E4%B9%A6%E7%99%BB%E5%BD%95)
          * [初始化git仓库](#%E5%88%9D%E5%A7%8B%E5%8C%96git%E4%BB%93%E5%BA%93)
          * [禁用shell登录](#%E7%A6%81%E7%94%A8shell%E7%99%BB%E5%BD%95)
  * [常见问题(持续更)](#%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98%E6%8C%81%E7%BB%AD%E6%9B%B4)

Created by [gh-md-toc](https://github.com/ekalinin/github-markdown-toc.go)

## 本地仓库基础

本地`Git`操作三部曲，是“修改-添加-提交”。

#### 初始化仓库

当初始化一个仓库时，我们需要进入项目目录，使用`git init `命令来初始化该目录作为仓库，同时会在目录下生成.git仓库文件。

```shell
#创建文件夹code 并初始化为仓库
mkdir code
cd code
git init
```

#### 配置姓名和邮箱

通过 `git config` 命令可以修改局部配置文件(位于.git/config) ，加上参数`--global`可修改全局配置文件(位于~/.gitconfig)。在创建好仓库以后必须设置user域下的name和email字段，才能正常提交内容到仓库。

```shell
#设置提交者的姓名
git config --global user.name"xxxx"
git config --global user.email"xxxx@xxx"
```

#### 添加修改到暂存区

添加修改，并保存至工作区，需要用到`git add`命令，使用方式如下所示：

```shell
#添加所有修改
git add .
#添加hello.txt文件
git add hello.txt
```

#### 查看工作区状态

你可以随时使用`git status`命令查看工作区状态，它将提示你之后该做什么，使用方式如下所示：

```shell
#查看工作区状态
git status
```

#### 提交修改到本地仓库

提交修改到本地仓库，使用命令`git commit`，其使用方式如下所示：

```shell
#将暂存区的内容提交到本地仓库 完成一次对象记录
git commit -m "示例提交"
```

`-m`参数后面跟的是本次提交的具体内容，用来说明你这次的提交，主要是做了哪些修改，这个说明内容是必须的。

#### 查看本地仓库提交记录

查看本地仓库的提交记录，使用命令`git log`，其使用方式如下所示：

```shell
git log
```

`--oneline`参数可以被添加，使得每次记录只显示单行的摘要，当记录较多时建议采用。

## 远程仓库基础

#### clone远程仓库

克隆操作需要用到的命令是`git clone`，它的具体用法如下所示：

```shell
git clone https://sample.git
```

通过这样的操作，就能将远程版本库复制到本地了，而且会默认克隆到`sample`文件夹下（对应于远程版本库地址中指定的`sample`）。同时，你也可以根据需要，指定克隆到其他目录下，其命令格式为：

```shell
git clone https://sample.git "指定目录"
```

需要指明的是，仓库的位置**可以是本地路径**。

#### 添加远程仓库

对于自己的项目，我们更多的会采用在第三方托管平台建立远程仓库后，在本地仓库中添加远程仓库，从而使二者可以关联。添加远程仓库需要用到命令是`git remote add “远程仓库名” “远程仓库地址”`，它的具体用法如下:

```
#在本地仓库中添加远程分支origin 指向远程仓库
git remote add origin https://sample.git
```

#### 推送本地内容到远程仓库

推送本地内容时，会将所有未推送至远程仓库的内容，都提到远程仓库。它用到的命令是`git push 远程仓库名 本地分支名:远程分支名 `

具体的使用方法如下：

```shell
#将本地仓库的master分支中的内容 推送到远程仓库origin的master分支
git push origin master:master
```

`-u`参数可以被添加，建立起本地`master分支`和远程`master`分支之间的对应关系，下一次如果再推送本地`master`分支，就可以忽略远程仓库名和分支名了。

`-f`参数可以被添加，用本地分支内容强制覆盖远程分支内容。

#### 拉取远程内容到本地仓库

拉取远程仓库的内容到本地，需要使用`git pull 远程主机名 远程分支名 本地分支名`命令，使用示例如下:

```shell
#将远程仓库origin的master分支的内容拉取到本地master分支
git pull origin master:master
```

`-f`参数可以被添加，用远程分支内容强制覆盖本地分支内容。

如果已在push时建立分支对应关系，则此处就可以忽略远程仓库名和分支名了。

当远程分支和本地分支对同一内容做了修改，这就会导致将远程分支的修改，合并到本地分支的时候发生**冲突**。这个时候，可以选择手动修改差异文件解决冲突，然后合并。也可以选择直接强制拉取。

## 分支

#### 创建分支

创建新的分支 当你需要创建一个新的分支的时候，可以使用`git branch`命令，其具体使用格式为： `git branch 新的分支名字` 使用示例如下：

```shell
#创建名为new_branch的新分支
git branch new_branch
```

#### 切换分支

分支切换 可以使用`git checkout 分支名` 命令切换到其他分支 使用示例如下：

```shell
#切换到new_branch分支
git checkout new_branch
```

创建新分支的同时切换 切换到一个新的分支，有一个更为简洁的命令：`git checkout -b`，它的使用格式为： `git checkout -b 新的分支名字`,使用示例如下：

```shell
#创建名为new_branch的新分支并切换到新分支
git checkout -b new_branch
```

#### 删除本地分支

删除本地分支，需要用到`git branch`命令，且需要`-D`参数，具体命令格式为： 　`git branch -D 需要删除的分支的名字` 使用示例如下：

```shell
 #删除develop分支
 git branch -D develop
```

#### 删除远程分支

推送空分支实现远程分支的删除方法,具体的命令格式为：`git push 远程主机名 :远程分支`

```shell
  #删除远程develop分支,其中origin为远程主机名
  git push origin :develop
```

  除了推送空分支到远程分支外，也可以通过`delete`参数实现删除。

具体的命令格式为： 　`git push 远程主机名 --delete 远程分支名` 具体使用示例如下：

```shell
  #删除远程develop分支,其中origin为远程主机名
  git push origin --delete  develop
```

#### 本地分支合并

分支合并需要用到`git merge`命令，具体的命令格式为：`git merge 需要合并的分支`

分支合并也分为正常合并和快进式合并，默认采用的是快进合并，即`fast-farward merge`。通过为`git merge`添加参数`--no-ff`，即可实现正常合并。

![img](https://www.educoder.net/api/attachments/184238)![img](https://www.educoder.net/api/attachments/184240)



具体使用示例如下：

```shell
#在本地master下执行，实现将develop以快进方式合并到master
git merge develop
#在本地master下执行，实现将develop以正常方式合并到master
git merge --no-ff develop
```

#### 远程分支合并

合并远程分支的一般步骤是：

**第一步，分别获取要合并的两个远程分支内容到本地；**

**第二步，在本地将两个分支合并；**

**第三步，将合并后的本地分支推送到远程分支，完成合并。**

我们以将远程`develop`分支合并到远程`master`分支为例，操作过程如下：

1. 获取远程`develop`分支到本地分支（如`develop`分支）。如果本地已经有分支对应远程`develop`分支，则可以直接在该分支上执行`pull`操作或者`fetch/merge`操作，以获取远程最新内容。否则，可以新建分支跟踪远程`develop`分支，并获取最新内容到本地；
2. 切换到`master`分支，并获取远程`master`分支的最新内容到本地；
3. 将本地`develop`分支合并到本地`master`分支；
4. 将本地`master`分支推送到远程`master`分支。

以合并远程`develop`分支到远程`master`分支为例，其具体操作步骤如下：

```shell
#切换到develop分支
git checkout develop
#获取远程develop分支的内容到本地
git pull origin develop:develop
#切换到master分支
git checkout master
#拉取远程master分支内容到本地
git pull origin master:master
#合并本地develop分支到master分支
git merge develop
#将合并后的分支推送到远程master分支
git push origin master:master
```

## 历史与撤销

#### git log进阶

在之前，我们已经介绍了`git log`的基本使用方法，这里我们要进一步介绍`git log`的使用。

查看提交的内容差异 `git log`提供了`-p`参数，用于查看每次提交之间的内容差异，如下： 　`git log -p` 即可显示每次提交之间的变化

而如果想限制显示的范围，则可以再添加参数用于限定： 　`git log -p -2` 如上，则仅显示最近的两次更新。 如上所示，这一选项附带了每次`commit`的内容变化，这就为代码审查或者浏览某个搭档的修改内容，提供了很好的参考。

- 其他`git log`选项：
  1. 单词层面对比 `Git`提供了`--word-diff`选项，可以显示单词层面的差异。当需要在书籍、论文这种很大的文本文件上，进行对比的时候，这个功能就非常有用。
  2. 显示简要的增改行数 `Git`提供了`--stat`选项，则可以仅显示增加或者减少了多少行。
  3. `pretty`选项 使用`--pretty` 选项选项，可以指定不同的显示属性，如`oneline` 将每个提交放在一行显示。 `short`，`full` 和 `fuller` 可以指定展示的信息的多少。

#### git revert实现版本回滚

版本回退可以用`git revert`命令。`git revert`撤销提交时，会保留所撤销的提交的记录和历史，并将回滚操作做为一次新的提交。即提交一个新的版本，将需要`revert`的版本的内容再反向修改回去，版本会递增，不影响之前提交的内容。其具体的使用方法如下：

   

```shell
#回滚到前一次commit
git revert HEAD                
#回滚到前前一次commit
git revert HEAD^    
#回滚指定id的commit（commit-id可通过git log 查看 形如：fa042ce57ebbe5b）
git revert commit-id 
```



#### git reset实现版本回退

`git reset`也能实现版本回退，但是`git revert` 和 `git reset`也存在一定的区别 ：

- `git revert`是用一次新的`commit`来回滚之前的`commit`，`git reset`是直接删除指定的`commit`；
- 在回滚这一操作上看，效果差不多。但是，在日后继续`merge`以前的老版本时有区别。因为`git revert`是用一次逆向的`commit`，“中和”之前的提交，因此日后合并老的`branch`时，导致这部分改变不会再次出现。但是`git reset`是把某些`commit`在某个`branch`上删除，因而和老的`branch`再次`merge`时，这些被回滚的`commit`应该还会被引入；
- `git reset` 是把`HEAD`向后移动了一下，而`git revert`是`HEAD`继续前进，只是新的`commit`的内容和要`revert`的内容正好相反，能够抵消要被`revert`的内容。

`git reset`用法如下：

- `git reset HEAD` 回到当前最近一次 `commit`。
- `git reset HEAD^` 回到前一次 `commit`。
- `git reset HEAD~n` 回到前n次 `commit`。
- `git reset commit-id` 比如：`commit = fa042ce57ebbe5b`，回到指定的版本。(撤销记录会保存 可以在git reflog中查看)

另外`git reset`也可以指定`reset`的模式：`hard`、`soft`、`mixed`、`merged`、`keep`。 这几种模式的差别如下：

- `--soft`  缓存区和工作目录都不会被改变；
- `--mixed` – 默认选项。**缓存区和你指定的提交同步**，但工作目录不受影响；
- `--hard` – 缓存区和工作目录，都同步到你指定的提交。

几种模式的具体使用方法如下：

```shell
#直接丢弃工作区和暂存区的修改
git reset --hard commit-id
#暂存区内容保留，工作区修改丢弃
git reset --mixed commit-id
#暂存区和工作区内容都保留
git reset --soft commit-id
```

#### git checkout 撤销工作区更改

如果只是工作区有了修改，则可以直接使用`git checkout`进行撤销，具体操作如下： 　`git chekcout hello` 通过这种方式，就可将`hello`文件自上个`commit`之后，尚未`add`进暂存区的修改丢弃。（git checkout实际是用仓库内最新的更改同步到工作区）。

#### git reset 撤销暂存区更改

如果将错误的文件添加进暂存区后，想从暂存区移回工作区，需要采用git reset命令:`git reset HEAD 文件名`

```shell
#将添加到暂存区的hello重新移回工作区 等价于暂存区和最新的一次提交进行了部分同步
git reset HEAD hello
```

#### git rm 删除or屏蔽文件

当我们需要删除暂存区或分支上的文件，同时工作区也不再需要这个文件了，可以使用： 　`git rm 文件路径` 

当我们**需要删除暂存区或分支上的文件**，但本地又需要使用， 只是**不希望这个文件被提交到版本库**，可以使用： 　`git rm --cached 文件路径`

`-f`参数可以被添加，用于强制删除。

但是无论使用哪种方式，**都相当于在本地做了修改**，因此，还需要通过`git commit`操作将修改提交。

```shell
#从物理上 删除文件
git rm filename1
#只是屏蔽对该文件的仓库跟踪 但文件还在磁盘上
git rm --cached filename1
```

## 标签

在开发过程中，`commit ID`是一串无序的字符，它虽然能唯一标记一次代码提交，即一个版本。但是，它很难记忆和辨识。所以，为了给不同的版本起一个容易辨识的名字，我们可以给这次提交打上一个标签，用不同的标签来对应不同的版本。实际上，在为某次提交创建标签的时候，`Git`**会为标签生成一个指针，以指向其对应的提交**。然后，我们就可以通过标签找到对应的提交，这样对我们版本发布和代码审查都很有帮助。

#### 创建标签

##### (1)不含附注的标签

创建标签的命令格式为`git tag 标签名 commitID`

参数`commitID`标识了该标签对应的代码版本，如果不提供`commitID`，就默认为最近一次提交后的代码打标签。使用实例如下:

```shell
#为最近一次commit打标签
git tag v1.0
#为指定id的commit打标签
git tag v1.0 7f8buir2
```

##### (2)包含附注的标签

如果需要像提交代码时增加提交日志那样，为每个标签添加说明信息，则需要使用`git tag -a 标签名 -m "说明信息" commitID`，使用实例如下:

```
git tag -a v1.0 -m 'version 1.0测试版本' 7f8buir2
```

表示为7f8buir2打标签v1.0，增加一个`version 1.0测试版本`的说明信息。

#### 查看标签

查看当前所有标签需要用到`git tag`命令，其具体使用示例如下: 

```shell
#列出所有的标签，显示的标签按字母顺序排列，所以标签的先后并不表示重要程度的轻重。
git tag
```

如果标签过多，而你指向显示指定的某些标签，则可以使用`-l`参数配合正则表达式：

```shell
#列出如下开头的tag
git tag -l 'v5.1.2.*'
```

#### 查看标签附注

查看标签附注需要用到`git show 标签名`命令，其具体使用示例如下: 

```shell
#列出标签v1.0的附注信息
git show v1.0
```

#### 推送标签到远程仓库

##### (1)推送指定标签

推送指定标签到远程仓库的`Git`命令如下：`git push 远程仓库名 tag名`

##### (2)推送全部标签

推送本地全部标签到远程仓库的`Git`命令如下： `git push --tags 远程仓库名 `  

使用示例如下：

```shell
#该语句表示将`v1.0`标签，推送到`origin`对应的远程仓库。
git push origin v1.0
#该语句表示将本地全部标签，推送到`origin`对应的远程仓库。
git push --tags origin 
```

#### 删除本地标签

删除本地标签，需要用到的命令格式为`git tag -d 标签名`具体使用方法示例如下：

```shell
#这样就能实现删除`v1.0`标签
git tag -d v1.0
```

#### 删除远程标签

删除远程`tag`，可以使用命令`git push origin --delete tag 标签名` (形如删除分支)

或者命令 `git push origin :refs/tags/标签名` 即推送一个空的`tag`名到远程仓库。使用实例如下:

```shell
#第一种方法
git push origin --delete tag v1.0
#第二种方法
git push origin :refs/tags/v1.0
```

## 忽略文件

如果你在本地版本库里，放入了仅供本地测试用的文件，但是你并不想将其推送到远程仓库，而且不想每次都被提醒你本地有未提交文件的话，就需要用到`Git`忽略文件提醒的功能。

#### 创建忽略文件

在`Git`工作区的根目录下，创建一个特殊的`.gitignore`文件，把要忽略的文件名或者文件名的通配符填进去，然后将`.gitignore`提交到本地仓库，这样`Git`就会在你添加或者提交时，自动忽略这些文件。

```shell
vim .gitignore
git add .gitignore
git commit -m"添加忽略文件"
```

#### 忽略文件格式

如果我们需要自己定义忽略哪些文件，就需要将其添加到`.gitignore`文件中去。你可以使用文件的全称，或者使用正则匹配的通配符。常用的通配符格式如下所示：

```makefile
 # 忽略指定文件
 HelloWrold.class
 # 忽略指定文件夹
 bin/
 bin/gen/
 # 忽略.class的所有文件
 *.class
 # 忽略名称中末尾为ignore的文件夹
 *ignore/
 # 忽略名称中间包含ignore的文件夹
 *ignore*/
```

## 配置别名

在操作`Git`的过程中，我们经常需要手动敲入类似于`git status`或`git checkout`等命令。而`status`和`checkout`这些单词较长，每次都要完整敲入的话，不仅浪费时间，而且还容易输错。如果可以为命令设置简写的话，比如以`git st`来代替`git status`，则会使操作变得更加简单方便。实际上，`Git`允许我们为`git`命令设置别名，以达到简化操作的目的。

别名设置的本质是在配置文件的alias域下增加"别名=真名"的字段项。

#### 设置别名

设置别名需要使用的命令是`git config --global alias`，其具体使用方法示例如下：

```shell
#为status设置别名st
git config --global alias.st status
```

执行以上步骤，即可将`st`设置为`status`的别名，即执行： `git st`的效果等效于执行`git status`。 同样，如果需要为其他命令设置别名，也可以采用相同的方式：

```shell
#为checkout设置别名ck
git config --global alias.ck checkout
#为commit设置别名cm
git config --global alias.cm commit
#为branch设置别名br
git config --global alias.br branch
```

需要指出的是`--global`参数是一个全局参数，即设置的这些别名可以在这台主机的所有`Git`仓库下使用。如果不加这个参数，则只对当前的仓库起作用。

#### 查看别名

如果要查看当前主机已经设置了哪些别名，则可以执行以下命令：

```
git config --list | grep alias
```

会得到类似于`alias.st=status`的信息，这就是说系统当前已经为`status`设置了别名`st`。

#### 删除别名 

如果需要删除已经设置的别名的时候，则需要执行以下步骤：

删除所有别名： 删除所有别名用到的命令为：

```
git config [--global] --remove-section alias
```

其中，`--global`是可选参数，加上这个参数也将本主机所有`git`仓库下的别名都删除，不加这个参数则仅删除本仓库下的别名。

删除指定别名：

```
git config [--global] --unset alias.指定别名
```

如果要删除本主机所有仓库下的`st`别名，则可以执行以下命令：

```
git config --global --unset alias.st
```

## 冲突与强制

#### 冲突的产生

##### (1)内容冲突

`Git`内容冲突产生的原因是，针对版本库中某个文件的某项内容，不同的操作对其做了不同的修改，以致于在合并不同的操作时发生矛盾，git程序无法做出采纳判断。

例如我们在本地master分支，添加了文件hello，其内容如下：

```
Learning English is easy and simple
```

然后，我们由master分支切换到一个新的分支develop并修改hello文件内容如下:

```
Learning English is easy & simple
```

将其提交到了本地develop分支后，我们又切换回master分支，并再次对hello内容进行了修改：

```
Learning English is easy or simple
```

这样，当我们**将develop分支合并到master分支**的时候，就会出现冲突提示如下：

```shell
Auto-merging helloCONFLICT (content): Merge conflict in helloAutomatic merge failed; fix conflicts and then commit the result.
```

冲突出现的原因是，我们在develop分支和master分支上，都对hello文件的内容做了修改，这样当将develop合并到master时，Git就不确定究竟应该采用哪个修改。

##### (2)树冲突

**文件名**修改造成的冲突，称为树冲突。比如，`A`用户把文件`cfile`改名为`afile`，`B`用户把文件`cfile`改名为`bfile`，那么`B`合并这两个提交时，就会出现冲突：

```shell
CONFLICT (rename/rename): Rename "cfile"->"bfile" in branch "HEAD" renameAutomatic merge failed; fix conflicts and then commit the result.
```

树冲突产生的原因是，我们将同一文件名，在不同操作中，修改为不同的名字。

#### 解决冲突

##### (1)内容冲突

当产生内容冲突时，如果你打开冲突发生的文件，你会在冲突区域发现类似于下面的内容：

```
<<<<<<< HEAD
Learning English is easy or simple
=======
Learning English is easy & simple
>>>>>>> develop
```

这个就是我们上面所举的内容冲突的例子，冲突文件的内容。从中可以看到`<<<<<<< HEAD`与`=======`包括的是我们当前分支的内容，而`=======`和`>>>>>>> develop`之间的则是需要合并过来的内容，为了解决冲突我们可以手动解决这些冲突，也可以使用图形化工具帮助解决。如果以手动方式解决，我们可以编辑冲突区域内容为我们想要的内容，比如将其修改成如下内容：

```
Learning English is easy and simple
```

然后再执行`git add`和`git commit`操作提交，这样就能将冲突解决了。 即解决冲突的一般过程为：

1. **手动编辑冲突区域；**
2. **执行`git add`，将编辑提交到暂存区；**
3. **执行`git commit`，将编辑提交到本地仓库以解决冲突。**

##### (2)树冲突

解决树冲突时，对于上面示例中的树冲突，如果最终决定采用文件`B`，我们可以采用如下方式解决：

```shell
#从本地仓库中删除afile
git rm afile
#从本地仓库中删除cfile
git rm cfile
#再添加bfile
git add bfile
#最终提交
git commit
```

#### 强制操作

如果远程仓库中的某个分支已经无法使用，需要强制覆盖将其更新；或者你的本地代码已经完全不能用，而需要用远程仓库中的某个分支进行覆盖时，你就需要强制操作。

使用最频繁的强制操作，主要在以下几个方面：

- 强制推送(push) 如果远程的某个分支的内容需要被覆盖，这个时候就需要你进行强制推送，使用本地内容去覆盖该分支。
- 强制合并(merge/pull) 如果本地分支的内容需要被远程内容覆盖，这个时候就需要强制合并远程分支内容到本地。
- 强制丢弃(checkout) 如果你需要强制丢弃版本库、暂存区或者工作区的内容时，就需要强制丢弃。

强制推送 强制推送和普通推送的区别，就在于在末尾加上了-f参数，即`git push -f 远程主机名 本地分支名：远程分支名 `，具体使用方法如下：

```shell
#将本地分支强制推送到远程主机origin的master分支
git push -f origin master:master 
```

强制合并 强制合并和普通合并的区别，也是其在末尾加上了-f参数，即`git pull 远程主机名 远程分支名：本地分支名 -f`，具体使用方法如下：

```shell
#将远程master分支强制合并到本地master分支
git pull -f origin master:master 
```

强制丢弃 我们之前介绍的`checkout`，就可以使用`-f`参数，强制丢弃本地修改，具体使用方法如下：

```shell
#强制丢弃本地文件hello的修改
git checkout -f hello
```

## 变基

合并不同分支，除了使用`merge`操作之外，还可以使用`rebase`操作。相比于`merge`操作，使用`rebase`会使分支树更为清晰、干净。

#### merge和rebase的不同

`merge`的工作流程如下图：

![img](https://www.educoder.net/api/attachments/184290)

如上图所示，我们从远程仓库`origin`的`C2`版本，创建一个新的分支`develop`进行开发，并进行了`C5`、`C6`两次提交。之后团队中其他成员又向`origin`推送了两次提交`C3`、`C4`。为了合并远程分支上的新内容到本地，我们进行`merge`操作，将内容合并到`develop`之后，生成了一次新的提交`C7`。此时，`develop`分支还是一个独立的分支。

而`rebase`的工作流程如下图：

![img](https://www.educoder.net/api/attachments/184291)

`rebase`又可称为‘变基’，结合上图的话，这个词就很容易理解了。即：

1. `C5`、`C6`本来是在`C2`这次提交的基础上进行修改的；
2. 现在我们将这个‘基础’改为`C4`，即将`C5`、`C6`的提交作用到`C4`上去；
3. 在这个过程中，可能会有冲突产生，解决冲突之后就完成了`rebase`。

由图可以看到，`rebase`实质是将一条分支的旧基点变更为新的基点。

#### 分支变基

`rebase`的基本操作是将某个分支的修改到指定分支，其命令格式为：`git rebase 基分支 源分支`

其中‘基分支’是我们的新的‘基’，而‘源分支’就是需要进行变基操作的分支。这样就能实现将源分支变基到基分支。具体使用示例如下：

```shell
#将develop变基到master分支的新节点
git rebase master develop
```

 如果是将当前分支变基到指定分支，则可以直接使用`git rebase 源分支`，会默认当前分支是`基分支`。具体使用示例如下：

```shell
#默认将当前分支变基到mater分支新节点
git rebase master
```

#### 分支变基冲突

由于变基是将修改作用到一个不同的版本上，因此很可能在`rebase`的过程中出现冲突。和`merge`一次性合并所有冲突不同的是，`rebase`的冲突是一个一个解决的。以上图中的`rebase`操作为例，需要分别解决和`C3`、`C4`的冲突。在解决`rebase`冲突的过程中，当解决完一个冲突的时候，使用如下命令后，才会**出现下一个冲突**：

```shell
#将本次冲突加入
git add -u 
#继续获取下一个冲突
git rebase --continue 
```

冲突全部解决完后，`rebase`操作就完成了。 如果在解决冲突的过程中，想放弃`rebase`操作，则可以使用如下命令撤销`rebase`操作：

```shell
#退出rebase，并回退到rebase前的状态
git rebase --abort
```

## 储藏

#### 储藏的概念

“储藏”可以获取你工作目录的中间状态（包括修改过的被追踪的文件和已经暂存的变更），并将其保存到一个未完结变更的堆栈中，而且随时可以重新应用。当你不想提交，也不想丢弃当前工作区中的内容，而想切换到其他分支的时候，可以使用储藏命令先暂存工作区中的内容。然后，再回到当前分支的时候，将储藏起来的内容，恢复到工作区之后，即可恢复之前的工作。

储藏分为**保存和应用**两个部分。保存就是将当前工作区的内容保存到一个栈中，而应用就是从栈中取出内容，重新应用被保存的工作。

#### 实现保存

保存用到的命令是`git stash`，只需在当前分支执行此命令，即可将当前工作区的内容保存起来。

如你在本地版本库创建了`helloGit`文件，此时 `git status`查看工作区状态可以得到如下所示提示：

```shell
On branch master
Unt\fracked files:  
  (use "git add <file>..." to include in what will be committed)        
  helloGit
 nothing added to commit but unt\fracked files present (use "git add" to t\frack)
```

当你执行`git stash`命令，将工作区保存起来之后，再次查看可以得到如下提示：

```shell
On branch masternothing to commit, working tree clean
```

此时已经将工作区内容保存了起来，所以才会提示工作区是干净（`clean`）的。

#### 查看保存

你可能执行了多次保存，所以你需要查看已经保存起来的内容有哪些。查看已经保存的工作的命令如下：`git stash list`

会得到类似于如下输出：

```
stash@{0}: WIP on master: bguebge add helloGit1
stash@{1}: WIP on master: 7gder34 add helloGit2
stash@{2}: WIP on master: 3frfg4g add helloGit3
```

如上所示，可以得知一共有三次保存。

#### 应用保存

想要重新应用最近保存的内容，只需要命令`git stash apply`即可。

如果要应用指定的储藏，则可以使用命令`git stash apply 储藏标识`即可。

这里的`储藏标识`就是`git stash list`中显示的类似于`stash@{0}`的字符串。使用实例如下:

```shell
#重新应用了第二次储藏helloGit2
git stash apply stash@{2}
#默认应用最近的储藏helloGit3
git stash apply
```

## 搭建本地Git服务器

虽然有提供托管代码服务的公共平台，但是对一部分开发团队来说，为了不泄露项目源代码、节省费用及为项目提供更好的安全保护，往往需要搭建私有`Git`服务器用做远程仓库。`Git`服务器为团队的开发者们，提供了协作开发平台，开发者可以基于私有的`Git`服务器进行项目开发。

`Git`服务器必须搭建在`Linux`系统下，因此必须准备一台运行`Linux`系统的主机，这里我们推荐`Ubuntu`或者`Debian`系统。

#### 安装并配置git

###### 安装git

首先要在主机上安装`git`服务，在`Ubuntu`下安装`git`只需要一条命令即可：

```
sudo apt-get install git
```

这样就在该主机上安装了`Git`服务，然后执行`git config`，即可完成`git`的配置。

###### 创建一个用户用来运行git服务的用户

创建一个专门的服务，来运行`git`服务，是为了使`git`服务和系统的其它服务不冲突。如果`git`服务可以`在root`权限下运行，则以`root`用户使用`git`服务即可，并不需要创建专门的用户去运行`git`服务。这里，我们假设创建一个名为`educoder`的用户，来运行`git`服务：

```
sudo adduser educoder
```

这样就可以在`educoder`用户下运行`git`服务。

###### 创建证书登录

虽然是私有的`Git`服务器，但是也不能允许主机随意向`Git`服务器推送代码。因此，需要登录到`Git`服务器的主机的公钥（即`id_rsa.pub`文件）导入`Git`服务器的`/home/git/.ssh/authorized_keys`文件里，一行一个。

###### 初始化git仓库

然后，就需要在主机下，选定一个目录做为`Git`仓库。如果我们使用`/tmp/educoder.git`做为远程仓库，则需要执行：

```
cd /tmp
sudo git init --bare educoder.git
```

`Git`就会创建一个空白的仓库，里面**没有内容，也不存在工作区和暂存区**。这是因为`Git`仓库只是为了托管代码，所以不需要用户直接登录到`Git`服务器上去做修改。当我们创建了`Git`仓库之后，对应第二步创建专门的用户来运行`Git`，这一步需要将仓库的所属关系更改为相应用户，即：

```
sudo chown -R educoder:educoder educoder.git
```

###### 禁用shell登录

出于安全考虑，第二步创建的`educoder`用户不允许登录`shell`，可以通过编辑`/etc/passwd`文件完成。找到类似下面的一行：

```
educode:x:1001:1001:,,,:/home/educode:/bin/bash
```

改为： `educode:x:1001:1001:,,,:/home/educode:/usr/bin/git-shell` 这样，`eudcoder`用户可以正常通过`ssh`使用`git`，但是无法登录`shell`。 通过以上步骤就完成了`Git`服务器的搭建，然后就可以通过`Git`命令，克隆远程仓库，并向远程仓库推送代码了。

## 常见问题(持续更)

[Markdown中Tob生成目录在github的README中失效](https://blog.csdn.net/weixin_34146986/article/details/89651958)

[未配置密钥时如何pull/push记住账密](https://blog.csdn.net/l1175832366/article/details/103328167)

[Git在Windows上中文乱码](https://blog.csdn.net/weixin_44256848/article/details/88716176?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromBaidu-1.not_use_machine_learn_pai&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromBaidu-1.not_use_machine_learn_pai)

[Git提交出现ssl_connect错误](https://blog.csdn.net/l1175832366/article/details/103339851)