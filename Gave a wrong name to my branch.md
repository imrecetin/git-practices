Gave a wrong name to my branch

You can rename a local branch name. It so happens many times that you may wish to rename your branch based on the issue you are working on without going through the pain of migrating all your work from one location to another. For instance, you could either be on the same branch or a different branch and still be able to rename the desired branch as shown below:

Syntax: git branch -m <old_name> <new_name>
Command: git branch -m old_code old_#4920

As you may wonder does git keeps of a track of this rename? Yes, it does refer to your ‘reflog’ entries, here is mine:

![git branch -m old_name new_name](images/2020/03/git-branch-m-old-name-new-name.png)

Renaming a branch will not affect its remote-tracking branch. We shall see in the remote section how to replace a branch on the remote repository

Ref Tutorial : https://www.edureka.co/blog/common-git-mistakes/
