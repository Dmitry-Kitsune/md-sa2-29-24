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
$ git log
commit b9def8424354adcda0ecafa3517688b003fd5005 (HEAD -> master)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:51:49 2024 +0300

    Homework Assignment 2: Basic Version Control

commit ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba (feature-branch)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:37:01 2024 +0300

    Init commit

## b9def8424354adcda0ecafa3517688b003fd5005

 git show b9def8424354adcda0ecafa3517688b003fd5005
commit b9def8424354adcda0ecafa3517688b003fd5005 (HEAD -> master)
Author: Dmitry Burlyaev <dm.burlyaev@gmail.com>
Date:   Tue Sep 24 22:51:49 2024 +0300

    Homework Assignment 2: Basic Version Control

diff --git a/README.md b/README.md
index 427f100..c948e69 100644
--- a/README.md
+++ b/README.md
@@ -11,3 +11,13 @@ git status
 git add --all
 git commit -m "Init commit"
 ```
+
+## Homework Assignment 2: Basic Version Control
+```bash
+git checkout -b feature-branch
+nano README.md #Maked changes
+git add --all
+git commit
+git checkout master
+git merge feature-branch
:
## ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba
$ git show ddb514bb02b04b0e58d4eef19a52d9e57a5c3eba
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
+## Homework Assigment 1: Initializing a local Repossitory
+```bash
+cd e://Programming/DevOps_Training/
+mk dir MyRepo
+cd MyRepo
+git init
+touch README.md
+nano README.md
+## added file README.MD
+git status
+git add --all
:

## 
diff --git a/sa.it-academy.by b/sa.it-academy.by
new file mode 160000
index 0000000..4c44452
--- /dev/null
+++ b/sa.it-academy.by
@@ -0,0 +1 @@
+Subproject commit 4c44452bbad18330428b7344edb2b83fac5d110f
(END)

## Homework Assignment 4: Creating and Applying Tags




