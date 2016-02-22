# PullProject

Command line instructions


Git global setup

git config --global user.name " "
git config --global user.email " @sfu.ca"

Create a new repository

git clone git@csil-git1.cs.surrey.sfu.ca:shm6/pullproject.git
cd pullproject
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Existing folder or Git repository

cd existing_folder
git init
git remote add origin git@csil-git1.cs.surrey.sfu.ca:shm6/pullproject.git
git add .
git commit
git push -u origin master