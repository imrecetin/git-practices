Forgot some changes in the last commit

Let’s say you forgot to make some modifications and already committed your snapshot, also you do not want to make another commit to highlight your mistake.
Command: git commit --amend

the recent commit object’s sha-1 id has been recreated and changed.

It is a rough equivalent for:

                       $ git reset --soft HEAD^
                       $ ... do something else to come up with the right tree ...
                       $ git commit -c ORIG_HEAD


Ref Tutorial : https://www.edureka.co/blog/common-git-mistakes/
