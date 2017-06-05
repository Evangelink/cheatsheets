#GIT Cheatsheet

##Keep fork up-to-date

###1. Clone your fork:

    git clone git@github.com:YOUR-USERNAME/YOUR-FORKED-REPO.git

###2. Add remote from original repository in your forked repository:

    cd into/cloned/fork-repo
    git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME/REPO-YOU-FORKED-FROM.git
    git fetch upstream

###3. Updating your fork from original repo to keep up with their changes:

    git pull upstream master

##Change source of PR
###1. Rename original PR branch
    git checkout my-branch
    git branch -m original-my-branch
    git push origin original-my-branch

###2. Rename new PR branch
    git checkout other-branch
    git branch -m my-branch
    git push origin my-branch -f

###3. Refresh PR