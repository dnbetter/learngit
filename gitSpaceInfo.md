###<div style="color:blue">git工作区，暂存区，版本库
工作区：可以看到的目录，gitBox  
版本库：包括暂存区（stage）和当前分支暂存区：，.git中的文件  
git分支：master分支自动创建，含HEAD指针
  
	$ git add <file>  //添加文件从工作区到版本库中的暂存区
	需要提交的文件修改通通放到暂存区
	$ git commit  //添加暂存区所有文件到版本库当前master分支
	一次性提交暂存区的所有修改
	$ git checkout -- file   //取消工作区的修改，并且将文件恢复到最近一次add或者commit的位置，版本库里的版本替换工作区的版本
	$ git reset HEAD file    //取消暂存区修改，回到工作区
	$ rm readme.txt   //删除文件
	
###<div style="color:blue">git远程管理
关联一个远程库：  
	
	$ git remote add origin https://github.com/path/learngit.git；
第一次推送master分支的所有内容
	
	$ git push -u origin master
以后每次提交最新修改内容：
	
	$ git push origin master
github创建一个仓库，本地进行克隆
	
	$ git clone https://github.com/dnbetter/gitskills.git
Git支持多种协议，包括https，但通过ssh支持的原生git协议速度最快。

	git@server-name:path/repo-name.git；//原生git协议
	git@github.com:michaelliao/learngit.git
	https://github.com/path/learngit.git；//https协议
	