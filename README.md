# 缘起
## 万事开头难，我用这个README.md文档，简单记录一下我学习git过程，顺便学学markdown的语法，做个分享。欢迎提issue，和我进行交流。



# 直接创建一个当前线路的分支，命名未dev，并转到此新分支
```sh
$ git checkout -b dev
```
等同于：
```sh
$ git branch dev
$ git checkout dev
```

# 修改想要做修改的文件之后，将修改后的状态提交commit
```sh
$ git commit -a -m "<提交的内容注释>"
```
等同于：
```sh
     $ git add .
     $ git commit -m "<提交的内容注释>"
```

# 如何查看分支
```sh
$ git branch -a  #查看全部分支，包括本地和远程
$ git branch -l  #只查看本地分支
$ git branch -r  #只查看远程分支
```

# 在本地主分支master合并dev分支，将master更新到最新
```sh
$ git checkout master  #切换分支时，必须先将当前的分支进行commit提交，或者stash暂存。
$ git merge dev
```

# 如何push本地支路到远程仓库
```sh
$ git push origin <branch-name>  #将想要push的分支推送过去，远程仓库自动会创建同名远程支路
```

# 用git命令删除远程分支
```sh
$ git branch -r   #查看有哪些远程分支
$ git branch -r -d origin/<branch-name>  #删除某远程分支的"跟踪"
$ git push origin :<branch-name>  #删除已上传到远程的分支，相当于在web上操作删除分支的操作
```

[参考链接](https://blog.csdn.net/furzoom/article/details/53002699)

# 删除本地分支
```sh
$ git checkout <branch-name1>  #切换到其它分支
$ git branch -d <branch-name>  #删除不需要的分支
```
