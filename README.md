# SOAL_CLUSTER
This repository shows detailed instructions to help you set up a local working environment on SOAL cluster. 

------------------------------

Table of Contents
------------------------------

- [GitHub Account](#github-account)
- [SOAL Cluster](#soal-cluster)
- [Anaconda](#anaconda)
- [TensorFlow](#tensorflow)

### GitHub Account
GitHub is a web-based Git or version control repository and Internet hosting service. It offers all of the distributed version control and source code management functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project. 

GitHub is free to use for **public** and **open source** projects. You are able to create unlimited public repositories and work with unlimited collaborators. Working with private repositories involves a paid plan. 

To set up an account, go to [SIGN UP](https://github.com/join) page and enter your **username**, **e-mail address** and **password**. To choose your personal plan, select **Unlimited public repositories for free**. 

Below are some commonly used git commands. A more detailed cheat sheet can be found [HERE](https://education.github.com/git-cheat-sheet-education.pdf). 

#### SETUP & INIT
Configure user information used across all local repositories
```
$ git config --global user.name "[firstname lastname]"
$ git config --global user.email "[valid-email]"
```
Clone repositories
```
$ git clone [url]
```
#### STAGE
Show modified files in working directory
```
$ git status
```
Add a file to your next commit
```
$ git add [file]
```
Show difference of what is changed but not staged
```
$ git diff
```
Commit your staged content as a new commit snapshot
```
$ git commit -m "[descriptive message]"
```
#### Branch
List your branches
```
$ git branch
```
Create a new branch
```
$ git branch [branch-name]
```
Switch to another branch
```
$ git checkout [branch-name]
```
#### Update
Fetch down all the branches from that Git remote
```
$ git fetch [alias]
```
Transmit local branch commits to the remote repository branch
```
$ git push [alias] [branch]
```
Fetch and merge any commits from the tracking remote branch
```
$ git pull
```

------

### SOAL Cluster

------

### Anaconda

------

### TensorFlow

------

### Reference
