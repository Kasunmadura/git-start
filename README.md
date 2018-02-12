### Setup basic

    mkdir testgit
    cd testgit
    git init

    echo "test 1st file" > test.txt
    git add .
    git commit

### Adding tags

    git add tag tagname
    git show tagname

    git describe --tags
    git tag -a v1 -m "version 1.0 release"

### Adding branch

    git branch -a
    git checkout -b deverlopment
    git merge deverlopment --no-ff
    git push origin deverlopment

    git remote add origin git@github.com:kasunr/test.git   

### git logs
    git log
    git log -p -2
    git log --stat
    git log --pretty=online
    git log --pretty=format:"%h: %an, %ae , %cd - %s" --graph

### git commands

    git branch
    git orgin
    git merge new_feather (fast forword and recursive)


### git tags

    git tag
    git show

    git tag <tag name> <commit id>
    git tag -d <tag name> (deleted tag)

    git tag v1.0 gsaseed
    git tag -d v1.0

    git push
    git ls-remote (view tags in the centrla repo)
    git fetch (pull all tags to central repo)

    git tag v1.2 ewewew
    git push remote-name tagname
    git ls-remote --tags
    git fetch --tags
    git push --delete remove-name tagname





### git remove and ignore

    git rm testremove.txt
    git commit -m "remove the file"
    echo *.md >  .gitignore
    git clone /home/kasunr/gitrepopath /newpath




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
