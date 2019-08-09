### Git日常
    
#### git rebase 冲突

在多人协作的情况下，出现代码冲突的情况是非常普遍的。 
当远程代码库出现更新时，我们经常需要更新本地库；当我们提交代码到远程库的时候，提交之前，我们也需要先更新一下本地代码库。

    # git 解决冲突的常用命令，在使用git rebase 出现冲突的时候，要注意ours 和 theirs 是分别是指哪个branch，如果不确定，打开冲突文件查看冲突部分，head指的就是ours
    git checkout -- theirs(ours) -- ${path/to/the/conflicted/file}
