# git_banbne

1 // 二选一，即可
2 git clone https://github.com/git/git.git
3 
4 git clone git@github.com:/git/git.git
 

 

 

 

git源码下载完成之后，切换到第一次提交的源码，步骤如下：

切换到git源码所在的目录下，命令行中键入如下代码

1 cd /your_local_directory/git
2 
3 git log --reverse    // 打印顺序从最早到现在
4  
5 git reset --hard 083c516331   //  git 源码的第一次提交号


##一行命令就可以切到最旧的版本:


 git log --reverse |awk 'NR==1 {print $2}' |  xargs   git reset --hard
