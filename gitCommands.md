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

### Initialize a repository from existing code
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
git log
