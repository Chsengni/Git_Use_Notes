<img src="images/1.png" alt="Git工作流示意图">

初始化目录(工作区)
	
	git init

<img src="images/2.png" alt="操作图">

创建文件夹

	mkdir MyGit
<img src="images/3.png" alt="操作图">

创建文件
		
	touch README.md
<img src="images/4.png" alt="操作图">


查看状态

	git status

<img src="images/5.png" alt="操作图">

添加文件到暂存区

	git add README.md

<img src="images/6.png" alt="操作图">

提交到master默认分支

	git commit -m "add README.md 2018/10/28 20:44:24 "

<img src="images/7.png" alt="操作图">
<img src="images/8.png" alt="操作图">

新增文件时
<img src="images/9.png" alt="操作图">
<img src="images/10.png" alt="操作图">

将新文件添加并提交

	git add 1.html
	git commit -m "1.html commit 2018/10/28 20:53:13 "
<img src="images/11.png" alt="操作图">


修改1.html文件，向文本追加

	echo "<--这是一段注释 version 1.0-->" >> 1.html

<img src="images/12.png" alt="操作图">


查看状态

<img src="images/13.png" alt="操作图">

添加到暂存区

<img src="images/14.png" alt="操作图">


恢复到未添加注释的1.html文件

首先把1.html从暂存区恢复工作区

	git reset HEAD 1.html
<img src="images/15.png" alt="操作图">

然后在工作区检出

	git checkout -- 1.html

<img src="images/16.png" alt="操作图">



恢复到只有README.md文件的时候

	git log

<img src="images/17.png" alt="操作图">

复制 commit后面的序列号

	git reset --hard 179dd71912d65cfae463d04620017493c70d668d

Date 一行是系统记录生成的时间

根据时间或者备注可以知道，第一次提交的序列号

<img src="images/18.png" alt="操作图">


清空本地仓库

	git rm README.md

<img src="images/19.png" alt="操作图">

	git commit -m "delete myGit"

<img src="images/20.png" alt="操作图">
<img src="images/21.png" alt="操作图">
