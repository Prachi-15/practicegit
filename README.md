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

git remote add origin https://github.com/Prachi-15/practicegit.git : 

This indicate URL of destination repository, any commited file will go to this origin. origin is a name of destination URL.

git remote -v: shows origin and destination.

git push origin main: push code into origin from main branch.


