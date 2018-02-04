---
title: "Building a Test-Driven REST Subscription API"
layout: page
excerpt: "Using best practices"
last_modified_at: 2017-12-06 00:00:00 
tags: [test-driven, rest, laravel]
---

Acommon problem that once and while used to get through:

Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

1: is SSH Keys Add Remotely on Bitbucket, GitHub, GitLab??

2: Check your keys locally with:

ssh-add -l

Should look like: (can have more than one, and/or using 4096 hash key)

2048 SHA256:TC7wexj0ceYk3lvtvb0hFc1yQclWl9O0jYvPlJhyWH4 /home/USERNAME/.ssh/id_rsa (RSA)

If doesn't have SSH keys, generate them, follow the article on Bitbucket.

Set SSH keys

https://confluence.atlassian.com/bitbucket/set-up-an-ssh-key-728138079.html

For Multiple keys if is the case:
https://confluence.atlassian.com/bitbucket/configure-multiple-ssh-identities-for-gitbash-mac-osx-linux-271943168.html?_ga=2.133857606.91896796.1513512003-507030520.1505085689

2: check the connection with your server

sudo ssh -Tv git@bitbucket.org
sudo ssh -Tv git@github.com

3: check the remote url

git remote -v

origin git@bitbucket.org:USERNAMEREPO/REPOSIRTORY.git (fetch)
origin git@bitbucket.org:USERNAMEREPO/REPOSIRTORY.git (push)

Change URL, try:

git remote set-url origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git

Should look like this:

git remote -v

origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git (fetch)
origin https://USERNAME@bitbucket.org/USERNAME-REPO/REPOSITORY.git (push)

4: check use of sudo before git command when is to remote server

Ex: git push -u origin master  X sudo git push -u origin master