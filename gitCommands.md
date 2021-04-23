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

### If we want to stop tracking our project
rm -rf .git 

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


## Connect your local project folder to your empty folder/repository on Github.

Copy the link in the input right beneath the title.


    Go back to your project in the terminal/command line.

    In your terminal/command line, type git remote add origin [copied web address]


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

 Pull before push ALWAYS:

	git pull origin master

	

THEN PUSH:

	git push origin master - <origin> name of remote repo <master> the branch that we push to 

	

First time push of the branch:

	git push -u origin <name of the branch> - -u coordinates the two branches (local and on server)

	

Create a branch:

	git branch <name of the branch>



Checkout a branch:

	git checkout <name of the branch>



Merge a branch:

	git checkout master

	git pull origin master

	git branch --merged - see which branches are merged 

	git merge <name of the branch you want to merge>

	git push origin master 



Delete a branch:

	git branch -d <name of the branch> - this deletes it locally!!!

	git branch -a - check the repo branches 

	git push origin --delete <name of the branch> - this deletes it from the repo!