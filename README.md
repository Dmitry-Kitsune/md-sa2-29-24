
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

## Homework Assignment 3: Exploring Git History
```bash
 git log
```
commit b9def8424354adcda0ecafa3517688b003fd5005 (HEAD -> master)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:51:49 2024 +0300

    Homework Assignment 2: Basic Version Control

commit ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba (feature-branch)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:37:01 2024 +0300

    Init commit

+# b9def8424354adcda0ecafa3517688b003fd5005
```bash
 git show b9def8424354adcda0ecafa3517688b003fd5005
```
commit b9def8424354adcda0ecafa3517688b003fd5005 (HEAD -> master)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:51:49 2024 +0300

    Homework Assignment 2: Basic Version Control

diff --git a/README.md b/README.md
index 427f100..c948e69 100644
--- a/README.md
+++ b/README.md
@@ -11,3 +11,13 @@ git status
+```bash
+git add --all
+ git commit -m "Init commit"
+```
+## Homework Assignment 2: Basic Version Control
+```bash
+git checkout -b feature-branch
+nano README.md #Maked changes
+git add --all
+git commit
+git checkout master
+git merge feature-branch
+```
:
+# ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba
```bash
 git show ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba
```
commit ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba (feature-branch)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:37:01 2024 +0300

    Init commit

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..427f100
--- /dev/null
+++ b/README.md
@@ -0,0 +1,13 @@

+# Homework Assigment 1: Initializing a local Repossitory0
+```bash
+cd e://Programming/DevOps_Training/
+mk dir MyRepo
+cd MyRepo
+git init
+touch README.md
+nano README.md
+# added file README.MD
+git status
+git add --all
:

+# 
diff --git a/sa.it-academy.by b/sa.it-academy.by
new file mode 160000
index 0000000..4c44452
--- /dev/null
+++ b/sa.it-academy.by
@@ -0,0 +1 @@
+Subproject commit 4c44452bbad18330428b7344edb2b83fac5d110f
(END)

 git commit -m "Homework Assignment 3 Exploring Git History"


## Homework Assignment 4: Creating and Applying Tags
```bash
git log --oneline
```
e8bc005 (HEAD -> master) Working with branches
1b49005 Homework Assignment 3 Exploring Git History
b9def84 Homework Assignment 2: Basic Version Control
ddb514b (feature-branch) Init commit


``` bash
 git log ddb514b
```
commit ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba (tag: v1.0, feature-branch)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:37:01 2024 +0300

    Init commit
```bash
git log --oneline
```
e8bc005 (HEAD -> master, tag: v1.3) Working with branches
1b49005 (tag: v1.2) Homework Assignment 3 Exploring Git History
b9def84 (tag: v1.1) Homework Assignment 2: Basic Version Control
ddb514b (tag: v1.0, feature-branch) Init commit
```bash
git log e8bc005
```
commit e8bc0059eae754b3fe9868a7b588dda3459b47af (HEAD -> master, tag: v1.3)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 23:19:59 2024 +0300

    +## Working with branches

commit 1b490051079a3b409810a51988bc088aa50eb251 (tag: v1.2)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 23:12:29 2024 +0300

    +## Homework Assignment 3 Exploring Git History

commit b9def8424354adcda0ecafa3517688b003fd5005 (tag: v1.1)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:51:49 2024 +0300

   +## Homework Assignment 2: Basic Version Control

commit ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba (tag: v1.0, feature-branch)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:37:01 2024 +0300

    Init commit
``` bash
nano README.md
git add --all
git commit
git tag -a v2.0 -m "Version 2.0
```
```bash
git log --oneline
```
686ee0f (HEAD -> master, tag: v2.0) Homework Assignment 4: Creating and Applying Tags
e8bc005 (tag: v1.3) Working with branches
1b49005 (tag: v1.2) Homework Assignment 3 Exploring Git History
b9def84 (tag: v1.1) Homework Assignment 2: Basic Version Control
ddb514b (tag: v1.0, feature-branch) Init commit

+# lightweight tags

```bash
git tag v1.5-lw b9def84
```
Fuzzy@Kitsune-PC MINGW64 /e/Programming/DevOps_Training/MyRepo (master)
```bash
git tag
```
v1.0
v1.1
v1.2
v1.3
v1.5-lw
v2.0

Fuzzy@Kitsune-PC MINGW64 /e/Programming/DevOps_Training/MyRepo (master)
```bash
git log --oneline
```
686ee0f (HEAD -> master, tag: v2.0) Homework Assignment 4: Creating and Applying Tags
e8bc005 (tag: v1.3) Working with branches
1b49005 (tag: v1.2) Homework Assignment 3 Exploring Git History
b9def84 (tag: v1.5-lw, tag: v1.1) Homework Assignment 2: Basic Version Control
ddb514b (tag: v1.0, feature-branch) Init commit

+# Force tag changed
```bash
git log --oneline
```
e066565 (HEAD -> master, tag: v2.0) Applying Lightweight Tags
686ee0f (tag: v1.9-lw) Homework Assignment 4: Creating and Applying Tags
e8bc005 (tag: v1.3) Working with branches
1b49005 (tag: v1.2) Homework Assignment 3 Exploring Git History
b9def84 (tag: v1.5-lw, tag: v1.1) Homework Assignment 2: Basic Version Control
ddb514b (tag: v1.0, feature-branch) Init commit
```bash
git tag
```
v1.0
v1.1
v1.2
v1.3
v1.5-lw
v1.9-lw
v2.0

```bash
git show v1.9-lw
```
commit 686ee0fe1e6fb20626338289ef5be8ae58c7ddd3 (tag: v1.9-lw)
commit 686ee0fe1e6fb20626338289ef5be8ae58c7ddd3 (tag: v1.9-lw)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 23:53:53 2024 +0300

 +##  Homework Assignment 4: Creating and Applying Tags

diff --git a/README.md b/README.md
index bee8184..5c83d42 100644
--- a/README.md
+++ b/README.md
@@ -1,4 +1,6 @@


 +## Homework Assigment 1: Initializing a local Repossitory

 +```bash
 +cd e://Programming/DevOps_Training/
 +mk dir MyRepo
+@@ -11,8 +13,10 @@ git status
 +git add --all
 +git commit -m "Init commit"
 +```
-

 +## Homework Assignment 2: Basic Version Control

+
+ ```bash
+ git checkout -b feature-branch
+ nano README.md #Maked changes
+ @@ -21,8 +25,10 @@ git commit
+ git checkout master
+ git merge feature-branch
+ ```
-

 +## Homework Assignment 3: Exploring Git History

+```bash
+ git log --binary
+```

## Homework Assignment 5: Undoing Changes

Sat Sep 28 13:54:24 BST 2024
e066565 Applying Lightweight Tags
686ee0f Homework Assignment 4: Creating and Applying Tags
e8bc005 Working with branches
1b49005 Homework Assignment 3 Exploring Git History
b9def84 Homework Assignment 2: Basic Version Control
ddb514b Init commit
```bash
git status >> README.md
```
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md
	modified:   sa.it-academy.by (new commits)

no changes added to commit (use "git add" and/or "git commit -a")
bug-fix
