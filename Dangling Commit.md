Dangling Commit

The following command helps you visualize these dangling commits. Look for dots without children and without green labels.

gitk --all --date-order $(git fsck | grep "dangling commit" | awk '{print $3;}')
