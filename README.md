# 直接创建一个当前线路的分支，命名未dev，并转到此新分支
	* $ git checkout -b dev
		等同于：
			* $	git branch dev
			* $	git checkout dev

# 修改想要做修改的文件之后，将修改后的状态提交commit
	* $	git commit -a -m "<提交的内容注释>"
		等同于：
			* $	git add .
			* $	git commit -m "<提交的内容注释>"


# 在本地主分支master合并dev分支，将master更新到最新
	* $	git checkout master
		切换分支时，必须先将当前的分支进行commit提交，或者stash暂存。
	* $	git merge dev

# 用git命令删除远程分支
	* $ git branch -r   #查看有哪些远程分支
	* $ git branch -r -d origin/<branch-name>  #删除某远程分支的"跟踪"
	* $ git push origin :<branch-name>  #删除已上传到远程的分支，相当于在web上操作删除分支的操作

	参考链接：https://blog.csdn.net/furzoom/article/details/53002699

# 删除本地分支
	* $ git checkout <branch-name1>  #切换到其它分支
	* $ git branch -d <branch-name>  #删除不需要的分支
		
