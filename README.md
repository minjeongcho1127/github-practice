# Docker

## Run Docker images containing Jupyter applications
> Prepare the image (once)
Pull the image from [Docker Hub](https://hub.docker.com/r/jupyter/datascience-notebook/):

    $ docker pull jupyter/datascience-notebook

> Run Docker images and open Jupyter notebooks
start the Jupyter server inside the container:

    $ docker run --rm -p 8888:8888 -v "$PWD":/home/jovyan/work jupyter/datascience-notebook

## Run Docker images by using 'docker-compose up' and open Jupyter notebooks
> Prepare the image (once)
Pull the image from [Docker Hub](https://hub.docker.com/r/ageron/handson-ml2):

    $ docker pull ageron/handson-ml2
    
Confirm the image (ageron/handson-ml2:latest):

    $ docker images
    REPOSITORY            TAG         IMAGE ID            CREATED             SIZE
    ageron/handson-ml2    latest      3ebafebc604a        2 minutes ago       4.87GB
    
> Run Docker images and open Jupyter notebooks
start the Jupyter server inside the container:

    $ cd /corresponding_path/docker
    $ docker-compose up
    
Go to the URL printed on the screen and done!
  
Reference: 
[Hands-on Machine Learning GitHub](https://github.com/ageron/handson-ml2/tree/master/docker),
[Project Jupyter GitHub](https://github.com/jupyter/docker-stacks)

---

# Git/GitHub

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
[yalco's Git](https://www.yalco.kr/25_git_tutorial_1/),
[yalco's GitHub](https://www.yalco.kr/26_git_tutorial_2/)


