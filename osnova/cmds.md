# vytvoreni git repa
git init

# prirazeni na server (gitlab)

## vytvoreni projektu
https://gitlab.quadient.group/projects/new

- internal

###Command line instructions
You can also upload existing files from your computer using the instructions below.


Git global setup
git config --global user.name "Radek Sedlák"
git config --global user.email "r.sedlak@neopost.com"

Create a new repository
git clone ssh://git@gitlab.quadient.group:22022/r.sedlak/graphics-lib.git
cd graphics-lib
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Push an existing folder
cd existing_folder
git init
git remote add origin ssh://git@gitlab.quadient.group:22022/r.sedlak/graphics-lib.git
git add .
git commit -m "Initial commit"
git push -u origin master

Push an existing Git repository
cd existing_repo
git remote rename origin old-origin
git remote add origin ssh://git@gitlab.quadient.group:22022/r.sedlak/graphics-lib.git
git push -u origin --all
git push -u origin --tags

# prirazeni
### add origin
git remote add origin https://gitlab.quadient.group/r.sedlak/graphics-lib.git

## prvni commit
create README
git add README
git status
git commit -m "readme"
git push
git push --set-upstream origin master

## new branch, checkout, commit
git branch -m feature
git checkout feature

## checkout conflict
!!!!
edit README
git add README
git commit -m "New readme"
edit README
git checkout master
git checkout master --force 

## edit, new commit
reword, ammend commit

## merge
git merge feature

fix README file
git add README
git commit

## changelist feature
## shelf unshelf
## cherry pick

