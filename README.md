# github-practice

## Git commands

> Create git repository

    git init

> User info

    git config -g user.name "(My name)"
    git config -g user.email "(My email address)"
    
> Basic Git

    git status
    git add -A
    git commit -m "(Memo)"
    git log
    git reset (6 digits of the commit's hashcode from the left) --hard
    git revert (6 digits of the commit's hashcode from the left)
    git branch (Branch name)
    git branch
    git checkout (Branch name)
    git checkout -b (Branch name)
    git merge (Branch name)
    git rebase (Branch name)
    git branch -d (Branch name)

## GitHub commands

> Basic GitHub
    
    git remote add (Remote name) (GitHun Repository Address)
    git remote
    git push -u (Remote name) (Branch name)
    git clone (Remote name)
    git fetch
    git pull (Remote name) (Branch name)
    git branch -a
    git checkout -b (New branch name) (Remote name)/(Remote branch name)
    git push -d (Remote name) (Branch name)

Reference:
[yalco Git](https://www.yalco.kr/25_git_tutorial_1/),
[yalco GitHub](https://www.yalco.kr/26_git_tutorial_2/)
