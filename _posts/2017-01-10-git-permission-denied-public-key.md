---
title: "Git Permissions Denied Public Key"
layout: page
tags: [Troubleshooting]
---

A common problem that once and while I used to get through:

Error:
Permission denied (publickey).
fatal: Could not read from remote repository.


Lets go through the following step/diagnostics:


Please make sure you have the correct access rights
and the repository exists.


#### 1) is SSH Keys added remotely on Bitbucket, GitHub, GitLab? #### 


#### 1.1) Check your keys locally on your *Unix/Mac shell: ####

```
ssh-add -l
```
The result should look like: (can have more than one, and/or using 4096 hash key)

```
2048 SHA256:TC7wexj0ceYk3lvtvb0hFc1yQclWl9O0jYvPlJhyWH4 /home/USERNAME/.ssh/id_rsa (RSA)
```

If doesn't have SSH keys, generate them, follow the article on Bitbucket to [set SSH keys](https://confluence.atlassian.com/bitbucket/set-up-an-ssh-key-728138079.html)

[For Multiple keys if is the case](https://confluence.atlassian.com/bitbucket/configure-multiple-ssh-identities-for-gitbash-mac-osx-linux-271943168.html?_ga=2.133857606.91896796.1513512003-507030520.1505085689)


#### 2 step/diagnostic: check the connection with your server ####

```
sudo ssh -Tv git@bitbucket.org
sudo ssh -Tv git@github.com
```

#### 3 step/diagnostic: check the remote url ####

```
git remote -v

Result 

origin git@bitbucket.org:USERNAMEREPO/REPOSIRTORY.git (fetch)
origin git@bitbucket.org:USERNAMEREPO/REPOSIRTORY.git (push)
```

Change URL, try:

```
git remote set-url origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git
```

Should look like this:

```
git remote -v

origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git (fetch)

origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git (push)
```


#### 4 step/diagnostic: check use of sudo before git command when is to remote server ####

```
git push -u origin master  
```

versus

```
sudo git push -u origin master
```