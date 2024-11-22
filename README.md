[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tbEHDGEc)
# Git and Github Introduction

| Nama  | Division        | Sub-Division  |
| ----- | ---------- | ---------- |
| Khrisna Nova Pratama  | ELC | Electrical Design |

## A. Early Procedure
### 1. Instal git to PC/Laptop
https://git-scm.com/downloads
### 2. Create a github account
  https://github.com/join
### 3. Configure Git
Open Git Bash or Terminal, then enter the following commands:
   ```
   git config --global user.name "Enter Your Username"
   git config --global user.email "Enter Your Email"
```
### 4. Generate an SSH Key
##### a. Go to Settings > SSH and GPG keys > New SSH Key in GitHub.
##### b. Create an SSH Key via Git Bash with the following command:
```
ssh-keygen -t ed25519 -C "Enter Your Email"
```
#### then press enter twice
#### c. Copy the SSH Key using this command:
```
clip < ~/.ssh/id_ed25519.pub
```
#### or
```
cat ~/.ssh/id_ed25519.pub | clip
```
#### d. Paste the copied key into the Key field on the New SSH Key page in GitHub.
## B. Create Repository
### 1. Visit  https://github.com/new
### 2. Enter the repository name and select its type (public or private), then click Create Repository.
### 3. Copy the SSH link by clicking Code > SSH > copy button (double-box icon).

## C. Connecting a Local Repository to GitHub
### 1. Manual Method
#### a. Create a local folder with the same name as the repository.
#### b. Open Git Bash in the folder and run the following commands:
```
git init
git remote add origin <SSH link>
git branch -M main
git pull origin <branch>
```
### 2. Using Git Clone
#### a. Open Git Bash in the parent folder where you want the repository to appear.
#### b. Run:
```
git clone <SSH link>
```
#### c. Navigate to the cloned folder, open Git Bash, and run:
```
git branch -M main
```
## D. Uploading Files to GitHub
### 1. Add files to the local folder.
### 2. Open Git Bash in the folder and run the following commands:
```
git add .
git commit -m "Feel free to write a description or the change of your files"
git push origin <branch>
```

## E. Create New Branch in Github 
### 1. Open the folder connected to GitHub.
### 2. Run the following command in Git Bash:
```
git checkout -B <branch name>
```
### 3. To switch to another branch, use:
```
git checkout <branch name>
```

## F. Delete Branch in Github
### 1. Switch to a branch that is not being deleted
```
git checkout <another branch name>
```
### 2. Delete the branch with the following command:
```
git branch -d <branch name>
```

## G. Merging Branch in Github
### 1. Switch to the branch you want to merge changes into:
```
git checkout <main branch name>
```
### 2.Merge the branch with the following command :
```
 git merge <branch name>
```
## Other Procedure
