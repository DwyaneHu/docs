### Git日常
    
#### 冲突

在多人协作的情况下，出现代码冲突的情况是非常普遍的。

    # git 解决冲突的常用命令，在使用git rebase 出现冲突的时候，要注意ours 和 theirs 是分别是指哪个branch，如果不确定，打开冲突文件查看冲突部分，head指的就是ours
    git checkout -- theirs(ours) -- ${path/to/the/conflicted/file}
