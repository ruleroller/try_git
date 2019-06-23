直接创建一个当前线路的分支，命名未dev，并转到此新分支
	* $ git checkout -b dev
		等同于：
			* $	git branch dev
			* $	git checkout dev

修改想要做修改的文件之后，将修改后的状态提交commit
	* $	git commit -a -m "<提交的内容注释>"
		等同于：
			* $	git add .
			* $	git commit -m "<提交的内容注释>"


在本地主分支master合并dev分支，将master更新到最新
	* $	git checkout master
		切换分支时，必须先将当前的分支进行commit提交，或者stash暂存。
	* $	git merge dev
