#Exercise 1
## Create a project folder & initialize git

yminshuti@Inshutis-iMac ~ % cd desktop
gyminshuti@Inshutis-iMac desktop % ls
Screenshot 2024-12-17 at 10.12.13.png   Screenshot 2024-12-17 at 10.53.13.png   TG
Screenshot 2024-12-17 at 10.17.18.png   Screenshot 2024-12-17 at 11.01.13.png   trialProject
gyminshuti@Inshutis-iMac desktop % mkdir Bundle1
gyminshuti@Inshutis-iMac desktop % cd Bundle1   
gyminshuti@Inshutis-iMac Bundle1 % touch Exercise1
gyminshuti@Inshutis-iMac Bundle1 % git init 
Initialized empty Git repository in /Users/gyminshuti/Desktop/Bundle1/.git/
gyminshuti@Inshutis-iMac Bundle1 % 


## Make changes to the project (add files and contents)

gyminshuti@Inshutis-iMac Bundle1 % git branch   
gyminshuti@Inshutis-iMac Bundle1 % git add .
gyminshuti@Inshutis-iMac Bundle1 % git commit -m "Added file 1 and wrote line in it" 
[main (root-commit) 0529d76] Added file 1 and wrote line in it
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Exercise1
 create mode 100644 readme.md
gyminshuti@Inshutis-iMac Bundle1 % git branch
* main


## Rename your main branch from `master` to `main` (If your branch name is already `main` then rename it to `master` and then back to `main`)

```

gyminshuti@Inshutis-iMac Bundle1 % git branch
* main
gyminshuti@Inshutis-iMac Bundle1 % git branch -m main master
gyminshuti@Inshutis-iMac Bundle1 % git branch               
* master
gyminshuti@Inshutis-iMac Bundle1 % git branch -m master main
gyminshuti@Inshutis-iMac Bundle1 % git branch
* main
gyminshuti@Inshutis-iMac Bundle1 % 

```


## Stage your changes and commit them

/*
gyminshuti@Inshutis-iMac Bundle1 % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Exercise1

no changes added to commit (use "git add" and/or "git commit -a")
gyminshuti@Inshutis-iMac Bundle1 % git add .
gyminshuti@Inshutis-iMac Bundle1 % git commit -m "Added seconf name on a file that specify my name"

*/

## Create a Github repo and connect it with your project
## Push your changes to GitHub

/* 
gyminshuti@Inshutis-iMac Bundle1 % git remote add origin https://github.com/prince-bugingo/Gym-Git-Exercises
error: remote origin already exists.
gyminshuti@Inshutis-iMac Bundle1 % git remote set-url origin https://github.com/prince-bugingo/Gym-Git-Exercises
gyminshuti@Inshutis-iMac Bundle1 % git push origin main
To https://github.com/prince-bugingo/Gym-Git-Exercises
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/prince-bugingo/Gym-Git-Exercises'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gyminshuti@Inshutis-iMac Bundle1 % 

*/



## Create a new branch `dev`

```
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch
  dev
* main

PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git checkout dev
Switched to branch 'dev'
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch
* dev
  main
```


## From `dev` create another branch `test`

```
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch test
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git checkout test
Switched to branch 'test'
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch
  dev
  main
* test

```


## Go back to the `dev` branch and delete the `test` branch

```
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch
  delete
* dev
  main
  test
 
 
PS C:\Users\Prince BUGINGO\desktop\learn\TheGYM\3-Git\Gym-Git-Exercises> git branch --delete test
Deleted branch test (was bccae8a).

```