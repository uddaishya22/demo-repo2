# Demo Repo 2
here we created another repo out of git repository
if we gonna use any git command it will show:

 fatal: not a git repository (or any of the parent directories): .git

## Initializing Git repository
we would have to initialize a new git repo
>> git init

we will get:
 Initialized empty Git repository

now we can check the status 

-> create a README.md file
 then add and commit this file 

## Pushing the new repo created locally
as we know that we haven't cloned this repo from GitHub inplace of that we made this repo locally 
Try to push this repo as:
>> git push origin master

we will get:
 fatal: 'origin' does not appear to be a git repository
 fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

This is because our git dont know where to push this file so several steps shall be taken to push the work files on GitHub

1. Create a new empty repository on GitHub
    -> I created by the name of "demo-repo2"
2. Copy the SSH/HTTP code of the respective repo from GitHub
3. In the terminal paste the link of origin using command 
    >> remote add origin https://github.com/uddaishya22/demo-repo2.git

4. Check the remote origin by command:
    >> git remote -v

   we will get:
     origin  https://github.com/uddaishya22/demo-repo2.git (fetch)
     origin  https://github.com/uddaishya22/demo-repo2.git (push)

5. Now push the work files using:
    >> git push origin master

[If we want to make the pushing repository path default we can add -u (upstream) prior to origin so that next time we can just use 'git push'
for example-
>> git push
]