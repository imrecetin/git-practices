Combining Git commits with squash
running the interactive rebase command with HEAD~3. This lets Git know I want to operate on the last three commits back from HEAD.
git rebase -i HEAD~3

Git will open up your default terminal text editor (most likely vim) and present you with a list of commits:
Something like that
    pick 7f9d4bf Accessibility fix for frontpage bug
    pick 3f8e810 Updated screenreader attributes
    pick ec48d74 Added comments & updated README

    # Rebase 4095f73..ec48d74 onto 4095f73 (3 commands)
    #
    # Commands:
    # p, pick <commit> = use commit
    # r, reword <commit> = use commit, but edit the commit message
    # e, edit <commit> = use commit, but stop for amending
    # s, squash <commit> = use commit, but meld into previous commit

There are a couple options here, but we’ll go ahead and mark commits we’d like to meld with it’s successor by changing pick to squash. (If you’re using VIM, type i to enter insert mode)

    pick 7f9d4bf Accessibility fix for frontpage bug
    squash 3f8e810 Updated screenreader attributes
    squash ec48d74 Added comments & updated README
Press ESC then type :wq to save and exit the file (if you are using VIM)

Git will pop up another dialog where you can rename the commit message of the new, larger squashed commit:

    # This is a combination of 3 commits
    # This is the 1st commit message:

    Accessibility fix for frontpage bug

    # This is the commit message for #1:

    Updated screenreader attributes

    # This is the commit message for #2:

    Added comments & updated README

    # Please enter the commit message for your changes. Lines starting
    # with '#' will be ignored, and an empty message aborts the commit
    
