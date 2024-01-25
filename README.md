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

#  Make comit and push it to main branch:

git commit -m "Fourth commit"
git push origin main

# MAKE NEW BRANCH:

git branch devepolera

# DELETE ANY BRANCH FROM LOCAL:

git branch --delete devepolera

# DEVELOPER A gets a story of division so first he will MAKE NEW BRANCH and then CHECKOUT in it.

# 1. MAKE ANOTHER BRANCH:

git branch developera   

# This developera branch is an exact replica of main branch. A developer can do any story in it and merge it to main branch and then delete developera.

# 2. CHANGE GIT BRANCH FROM MAIN TO DEVELOPERA by doing CHECKOUT to complete the story. 

git checkout developera

# 3. Complete the story and then ckeck
git status: 
# can see modified files

# 4. Add this file using:
git add .

# 5. Check status:
git status

# changes are modified in developera branch.

# 6. Commit the changes using

git commit -m "developera story"

# 7. Merge this developera branch with main branch

# a. Switch to main branch
git checkout main

# In main branch you can't see developer a story because branch is not merged.

# b. Merge main branch to developera branch

git merge developera

# After merging we can see all the changes of developer a story into main branch.

# 8. Delete the developera branch

git branch -d developera

# 9. Push changes from origin to main

git push origin main

# RESOLVING CONFLICTS:

# 1. Do some changes in app.py on github and save it.
# 2. Do some other changes in local app.py and then 
git add .

# 3. commit those changes
git commit -m "substraction"

# 4. Push into main
git push origin main

# Throw error because their is some change in the main which are not updated here, so first we need to pull those changes.

# 5. Pull changes done in repository
git pull origin main

# 6. Push this into min
git push origin main

# MERGING CONFLICT:

# 1. Another developer working in same function and in repository instead of using -c he use -e and commit changes.

# 2. In local you place -d instead of -c and commit changes, add and commit changes.

git add .
git commit -m "changes"

# 3. Push changes into main
git push origin main

# 4. This will throw error becoz of change , need to pull
git pull origin main

# 5. Conflict : merge conflict in app.py
# Accept Current Change/ Accept Incomming Changes/ Accept Both Changes/ Compare Changes 
Accept Current Changes

# 6. add and commit
git add .
git commit -m "merge conflicts"









