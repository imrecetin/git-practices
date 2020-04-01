Stashes

you may have stashed the data instead of committing it and then forgotten about it. You can use the git stash list command or inspect them visually using:

gitk --all --date-order $(git stash list | awk -F: '{print $1};')
