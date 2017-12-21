### Setup git server

  git config --global user.name "Root User"
  git config --global user.email "root@localhost"

  git config --list

  git config --global core.editor vim
  git config --global core.pager 'more'

  cat .gitignore_global
  *~
  .DS_store
  
  git config --global core.excludefile ~/.gitignore_global

### Systems Variable

  git config --system system.name "Git repo server 2"
  git config --global system.name "My git repo server 2"
