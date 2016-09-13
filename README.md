# tstgit
在github上创建仓库

第一步：在本地生产密钥 $ ssh-keygen -t rsa -C "youremail@example.com"

第二步：在github页面点击右上角的Account settings -->>SSH Keys
		点击Add SSH Keys  添上任意的Title 在Key文本框里黏贴id_rsa.pub;
		
第三步：在github的右上角找到Create a new repository ;创建一个新的仓库；
		在Repository name 填入仓库名字；其他保持默认；点击Create repository
		
第四步：在本地创建文件夹，名字与远程仓库名字一致，可以用命令mkdir name
		初始化仓库：git init 
		touch README.md 是添加这个文件的命令
		依次执行 git add 文件命 ；git add .  是添加所有文件到暂存区
		git commit -m "first commit " 是提交到本地版本仓库
		关联远程仓库：git remote add origin https://github.com/wy8473979981/仓库名.git

第五步：将本地版本库更新到远程仓库：git push -u origin master
		以后提交就可以用git push
