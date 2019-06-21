直接创建一个当前线路的分支，命名未dev，并转到此新分支
	git checkout -b dev
		等同于：
			git branch dev
			git checkout dev

修改想要做修改的文件之后，将修改后的状态提交commit
	git commit -a -m "<提交的内容注释>"
		等同于：
			git add .
			git commit -m "<提交的内容注释>"
