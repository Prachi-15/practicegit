#  Practicing git commands 

git init: It initialization current folder as git repository.

git status: hows status of files. U - untracked changes, A - tracked changes.

git add [filename] : add a new file to next commit(stage).

git rm --chached <file> : to remove or unstage the changes. 

Staging environment: staging environment is a temperory environment where we commit changs and then push it into github repository.

git commit -m "[descriptive message]" : Use to commit , -m : message about the commit, this message will pass as it is in github repository.

Push this file into staging environment in local (commit your staged content as a new commit snapshot).

git config --global user.name "Prachi-15" : give github username

git config --global user.name "prachiagrawal1509@gmail.com" : give github password.

git branch -M main :Create a new branch with name "main" in local (can name master also).

git branch: show branch

git remote add origin https://github.com/Prachi-15/practicegit.git : 

This indicate URL of destination repository, any commited file will go to this origin. origin is a name of destination URL.

git remote -v: shows origin and destination.

git push origin main: push code into origin.

git add. : Add all the files (new or updated) together.

Make .gitignore new file from github repossitory and set python and then pull it in local environment.

git pull origin main: pull data from origin repository too local environment.

.gitignore: 

what is the use of gitignore ?

While working on project we create multiple environments and packages and we don't want them to be on github because their file size is large. Github has a limitation to on size of file to be uploaded.

If we want that specific file should not commit we can put it in .gitignore. 

Like virtual environment: install only those packages in virtual environment which we will use.

Ex: virtual env name is myvenv, then put it's name in the .gitignore file like myvenv/

on git add. myvenv will not add becoz it is in .gitignore.

Make comit and push it to main branch

git commit -m "Fourth commit"
git push origin main





