# PullProject Command line instructions

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


Merging via command line

If you do not want to use the merge button or an automatic merge cannot be performed, you can perform a manual merge on the command line.
 HTTPS
 Git
Patch

https://github.com/sonnymyet/PullProject.git

Step 1: From your project repository, bring in the changes and test.

git fetch origin
git checkout -b dev origin/dev
git merge master
Step 2: Merge the changes and update on GitHub.

git checkout master
git merge --no-ff dev
git push origin master