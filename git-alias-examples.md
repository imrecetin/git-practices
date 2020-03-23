user.name=Çetin İmre
user.email=ctn.imre@gmail.com
alias.hist=log --pretty=format:"%C(yellow)%h%Creset %ad | %C(green)%s%Creset%C(red)%d%Creset %C(blue)[%an]" --graph --decorate
alias.root=!pwd
alias.co=checkout
alias.br=branch
alias.ci=commit
alias.cm=commit -m
alias.st=status
alias.unstage=reset HEAD --
alias.last=log -1 HEAD
alias.cob=checkout
alias.git=push
alias.gel=pull
alias.remotes=remote -v
alias.ba=branch -a
alias.bd=branch -d
alias.bd=branch -D
alias.amendno=commit --amend --no-edit


git config --global alias.ba "branch -a"
git config --global --list
git config --global --unset-all alias.ba
