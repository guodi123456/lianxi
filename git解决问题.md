git--版本控制/管理工具
本地仓库：本地被git管理的文件夹 ---注意是git管理
远程仓库：远程电脑被git管理的文件夹

github只能使用git进行提交，下载的大型仓库

同步：让本地仓库和远程仓库的代码保持一致
拉取：将远程的仓库中的代码拉取到本地仓库
推送：将本地仓库的代码提交到远程

在文件夹点击右键 -git Bash Here
新建一个文件夹，默认不会被git管理，要初始化一个仓库

git init

执行结束后，生成.git文件夹，那么就是被git管理了，-形成一个仓库了.
查看仓库状态 -git status
新建文件名称是红色，表示当前文件刚写好，暂时没写入仓库--表示在工作区
将工作区文件放入暂存区
git add --文件绿色表示进入暂存区

将暂存区的内容放到历史区
git commit -m '版本的描述'
文件被正式入库，不是红色了

注意： 所有文件最开始都在工作区
工作区-》暂存区--》历史区

git不管理空文件夹

一次性将多个文件放入暂存区
git add 文件夹 文件一

将暂存区内容还原到工作区
git reset HEAD -- 文件

将所有的内容放到暂存区
 git add .
 或者 git add --all

将暂存区内容全部返回工作区
git reset HEAD -- .
git reset HEAD -- all

git仓库有三个区域：-
1.工作区   ---在仓库外面工作
2.暂存区   ---还没有正式存入仓库，只是刚进来
3.历史区-形成版本 ----进入仓库

clear清屏

针对历史区
查看所有版本 git log

回退版本
  git reset --hard HEAD^  #回退到上一版本
  git reset --hard 版本号

让git管理空文件夹，在空文件夹，创建.gitkeep文件
.gitkeep==这个文件为了给空文件夹站位

git管理忽略文件，.gitignore

远程仓库：码云 ，github

git remote add origin 远程仓库地址
git remote add origin https://gitee.com/qweassa/a12.git
git push -u origin master







