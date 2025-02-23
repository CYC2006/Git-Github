![](https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg)

### 2025/2 Cyc
# Git and Github Tutorial

Git    - Version Control System
Github - Cloud Collaboration Platform


## 1. Download Instruction and Basic Setup (2min)

### Download
- Windows  - press “Next” to the end
- Apple - open terminal -> xcode-select --install

### Check Version
    git --version
    
### Create Account and Initialize

    git config --global user.name "Cyc"
    git config --global user.email "topcoder.cyc@gmail.com"
    git init : Initialize current file

:::success
Please create a git account yourself
:::


## 2. Types of Git Status

### Check Status
status types : untracked / unmodified / modified / staged

    git status

### Stage Files

    git add <filename1> <filename2>
    git add *.md
    git add .


## 3. Commit

### Commit a New Version

    git commit -m “commit message”

:::success
You can reate a .gitignore file to store files that don’t need to be committed
:::
:::success
Deleted files still need to be added and committed
:::


### Check Previous Versions
oneline : show each previous commits in one line

    git log
    git log --oneline

### Tips of writing Commit Message
- Independently commit each change
- Explain the commit’s What & Why
- Add a number to each commit to further track related changes
- Use git as a tool for viewing historical versions


## 4. Version Control

### Check Difference
to show the difference between **Filename** at **ID** and current file
    
    git diff <ID> <Filename>

### Back to Previous Version
Restore to a previous version
    
    git checkout <ID> <filename>
    git commit -m "restore to a previous version"

Restore to a previous version and **delete** all commits after that version

    git reset --hard <ID>
    git commit -m "restore to a previous version"


## 5. Git & Github Operations

:::success
Before Start, everyone should own a Github account
:::

### push
origin is the name of the remote database

    git remote add origin <origin’s URL>
    git branch -M main
    git push -u origin main

    git add .
    git commit -m "push a new file"
    git push

### pull
Synchronize the files on Github

    git pull
 
:::success
Github -> Branch -> pull request
:::

### branch
Check current branch (Initial : *main)

    git branch

Create a new Branch

    git checkout -b branch2 : switch branch to do whatever I want
    git add .
    git commit -m “new branch”
    git push -u origin branch2

### clone
Download the whole directory to user’s computer

    git clone <URL on Github>
    cd <filename>

### fork (on Github)
Build a completely independent repo based on someone else's repo


## 6. Homework

### Concept: fork, commit, push
1. Create an account on Git and Github
2. CYC2006 on Github has a public repository with some .md files in it. Fork my repository
3. Create a new .md file and write down "**Hello World (Your Student ID)**"
4. Add and commit the new file with commit message: "GitHW commit"
5. Push the file onto your new repository (8%)

:::warning
You will only get 8% if you complete all 5 steps
:::