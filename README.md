# Git-Course
This repository is part of git course from @jgsnto. It should be used as reference to your study. It is important to say that the best reference is always the documentation. So if you need more information, always search the Git documentation highlighted in the end of this document.

## Introduction

### What is Git, Github and Gitlab

- Git is the free open source version control system most used nowdays. Git allows you to manage and track changes in your documents over your project. Git was created in 2005 by Linus Torvalds. 
- Github and Gitlab are web-based git repository hosting services that allow you to store git repositories and colaborate with other developers. 
- Github is primaly used by open source projects and individual developers. Provides a wide range of features, including issue tracking, pull request and project management. 
- Gitlab is more used by enterprises companies. Offers built-in continuous integration/continuous delivery pipelines. Provides a wide range of features, including issue tracking, pull request and project management. 

### How git works

- The first step to understand who git works is to understand about the Github objects, those are:
1. Blob(Content Objects): Is used to store the files content in the respositories
2. Tree(Directory Objects): Is used to store the directory state. Points for blobs and other trees. 
3. Commit(Commit Objects): Is used to register a set of changes in many files in one object 

- After study about the git objects we need to understand the encryption algorithm used by git. The SHA-1. First is important to say that a Secure Hash Algorithm(SHA), uses a hash algorithm that takes an variable length input and as result we have a fixed size set of character. Git uses the SHA1 algorithm to make sure that the objects do not changed.

- The last important part to understand are the different stages of managing code: 
1. Working Directory: Directory on your local machine where you are currently working on code.
2. Staging Area: This is an intermediate area where you can review and select changes that you want to commit to your repository.
3. Repository Local: This is the local copy of your respository, which contains all the versions of your code that you have been committed. 
4. Repository Remote: This is the copy of your Git repository that is hosted on a remote serve, such as Github. 

### Basic commands on Git
- Start one empty repository.
```
git init 
```
- Add files to staging area.
```
git add
```
- Create one new commit whith the stagging area files.
```
git commit -m 
```
- Exihibit the repository status. 
```
git status
```
- Exihibit the commit history. 
```
git log
```
- List all the branchs.
```
git branch
```
- Alows you change branchs or create new one.
```
git checkout 
```
- Mix two branchs.
```
git merge
```
- Update the local repository based on the remote repository.
```
git pull
```
- Send the changes on the local repository for the remote repository.
```
git push
```

## Starting with git 

### Configure the user 
- Username and Email

```
git config --global user.name "name"
```
```
git config --global user.email "name@example.com"
```

- List all the configuration

``` 
git config -l
``` 

- Set the editor

```
git config --global core.editor "editor name"
``` 
### Working with branches 

- First is important to understand what is a branch. Which is a ramification of the code, what means that you have a copy of the code that you can edit whitou change the code in the master(main) branch. Usually branches are used to develop new features. 

- Create branches
```
git checkout -b branch_name
```
- Change branches 
```
git checkout desired_branch_name
```
- List all branches
```
git branch
````
- Delete branches 
```
git branch -D branch_name
````
