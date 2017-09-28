# SOAL_CLUSTER
This repository shows detailed instructions to help you set up a local working environment on SOAL cluster. 

------------------------------

Table of Contents
------------------------------

- [GitHub Account](#github-account)
- [SOAL Cluster](#soal-cluster)
- [Anaconda](#anaconda)
- [TensorFlow](#tensorflow)

------

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
The cluster has one node (hostname: soal-1.stanford.edu) with 8 Titan X GPUs, 64 CPU ocres and 0.75 TB RAM. Please first ask Sharad Goel to help create an account for you. 

To login, you first need to connect to the Stanford VPN. Please follow the instructions [HERE](https://uit.stanford.edu/service/vpn). After connecting to the Stanford VPN, you can ssh into soal-[1-5].stanford.edu with your SUNet credentials. 
```
$ ssh [SUNetID]@soal-1.stanford.edu
```

------

### Anaconda
Since the account type is not Administrator, it is easy to set up a local environment using [Anaconda](https://docs.anaconda.com/anaconda/). Anaconda is a package manager, an environment manager, a Python distribution, and a collection of over 1,000+ open source packages. It is free and easy to install. 

1. Download the Anaconda installer for Linux. 
```
$ wget https://repo.continuum.io/archive/Anaconda3-5.0.0-Linux-x86_64.sh
```
2. Install Anaconda for Python3.6
```
$ bash Anaconda3-5.0.0-Linux-x86_64.sh
```
The installer prompts `Do you wish the installer to prepend the Anaconda<2 or 3> install location to PATH in your /home/<user>/.bashrc ?` Enter `Yes`. After the installer finishes, enter `source ~/.bashrc` for the installation to take effect. 

------

### TensorFlow
To install TensorFlow with GPU support, simply run
```
$ conda install -c anaconda tensorflow-gpu 
```
