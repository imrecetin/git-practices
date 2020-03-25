Re-arrange history logs before pushing to remote

How I wish I would have made certain commits earlier than others and would have not made some commits at all. Interactively re-arrange and edit the old commits to effectively fix-up or enhance the code
Syntax: git rebase -i <after-this-commit_id>

Command: git rebase -i fb0a90e –start rebasing the commits that were made after the commit-id fb0a90e
