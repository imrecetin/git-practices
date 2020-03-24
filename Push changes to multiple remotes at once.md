Push changes to multiple remotes at once
Added two git remotes url to local development
  git remote add origin_gitlab https://gitlab.com/cetin.imre/iamsafe-mobile.git
  git remote add origin https://github.com/imrecetin/iamsafe-mobile.git
  origin	https://github.com/imrecetin/iamsafe-mobile.git (fetch)
  origin	https://github.com/imrecetin/iamsafe-mobile.git (push)
  origin_gitlab	https://gitlab.com/cetin.imre/iamsafe-mobile.git (fetch)
  origin_gitlab	https://gitlab.com/cetin.imre/iamsafe-mobile.git (push)
Added git alias to able to push changes to multiple remotes at once.
  git config --global --unset-all alias.pushallmaster alias.pushall alias.pullallmaster alias.pullall
  git config --global --add alias.pushall 'push origin && git push origin_gitlab'
  git config --global --add alias.pushallmaster 'push origin master && git push origin_gitlab master'
  git config --global --add alias.pullall 'pull origin && git pull origin_gitlab'
  git config --global --add alias.pullallmaster 'pull origin master && git pull origin_gitlab master'
  git config --global -l | grep pushall
  git config --global -l | grep pulllall

  Alternative Way to only push
  git remote set-url --add --push origin https://github.com/imrecetin/iamsafe-be.git
  git remote set-url --add --push origin https://gitlab.com/cetin.imre/iamsafe-be.git
  You can't pull from multiple remotes at once, but you can fetch from all of them:
  git fetch --all but you have to merge -- fast-forward
