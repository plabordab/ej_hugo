---
title: "Git"
date: 2022-09-27T19:54:33+02:00
draft: false
---

# REPOSITORY ON GITHUB

## create a new repository and link it to the local repository

1. Log in to github with your username and password.
2. In our account we create a repository
3. It shows us the commands to execute in local. The actions are:
4. We go to local to the directory where our project is
5. We execute: 

a.

```
git init 
```
>  This command initializes our directory as a git project. You will have created a directory named .git


b. 

```
git add . 
```
>  with this command we add the files from my directory (all to be specified .) to the repository


c.

```
git comit -m "checkpoint message" 
```
>  with this command we specify a message for the current changes


d. 

```
git branch -M main 
```
>  with this command we create a branch or working directory associated with the local repository


e.

```
git add remote origin https://github.com/plabordab/ej_hugo 
```
>  with this command we link the local repository to the remote repository

f.

```
git push origin main  
```
>  with this command we add the added files to the remote one


## copy a project to another destination

1. I access git hub and copy the url of the repository

2. I type:

```
git clone https://github.com/plabordab/ej_hugo 
```
> will create a directory with the name of the project and all the content (it is only done the first time)

3. I download also the theme

4. After working, to save it we do a push:


```
git add *
git commit -m "nuevos cambios"
git push -u origin main  
```
>  update the project in github with the latest changes

### updating a modified project somewhere else

```
git pull  
```
>  update the local project with the remote one

