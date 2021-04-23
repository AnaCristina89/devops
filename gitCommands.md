##Git

git --version

### set config values
git config --global user.name "ana"
git config --global user.email "xxx@gmail.com"

 Check the values
git config --list


### need help?
git help config
git config --help
git add help 

## Initialize a repository from existing code
In the local directory or repo: cd Local-Repo
git init

### Before first commit
This command shows all files'states to commit green/red

git status

### Add gitignore file
This file is a text file where we can add files that we want to ignore and we can also use wildcards (*.pyc)
touch .gitignore

### Add files to staging area
git add -A

git add .gitignore

git status
(files in green color to be commited)

### Remove files from staging area
git reset
git reset file_name.ext

git status


### Our first commit

git add -A
git commit -m "Initial commit"
git status
Working directory is clean that's because we've commited those files and now we don't have any modified or untracked files

git log

## Cloning a remote repo

cd Cloned-Repo/
ls -la (clean repo)

git clone <url> <where to clone>
git clone ../remote_repo.git .

### Viewing information about the remote repository

git remote -v
git branch -a

### Pushing changes
 
diff is going to  show me the changes that i have made to the code

git diff
git status
git add -A
git commit -m "Modified multiply function"

Then push:
 git pull origin master
 git push origin master