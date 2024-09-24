## Homework Assigment 1: Initializing a local Repossitory
```bash
cd e://Programming/DevOps_Training/
mk dir MyRepo
cd MyRepo
git init
touch README.md
nano README.md
## added file README.MD
git status
git add --all
git commit -m "Init commit"
```

## Homework Assignment 2: Basic Version Control
```bash
git checkout -b feature-branch
nano README.md #Maked changes
git add --all
git commit
git checkout master
git merge feature-branch
```
