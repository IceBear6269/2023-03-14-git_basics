# 2023-03-14-git_basics

- 'git init': initialize git repository in current directory
	-make sure that you don't nest git repositories
- 'git status': tells you things about your current git repo


- 'git add <FILE>': puts <FILE> into your staging area
- 'git commit': open up editor for you to write a message and create 
commit
	-'git commit -m "MESSAGE"': writes commit message without editor


-'git log': shows us the log / commit history
	-'git log --oneline': shows us the 1 line per commit version


-'HEAD': tells you where you are
-'git diff': shows you new changes to a file that has not been commited
	-'git diff --staged": shows you changes in the staging area
	-'git diff <HASH=˜> <FILE>': shows you difference between current 
and commit
		-'HEAD˜1': to use relative to head
		-'<HASH>': to use the actual hash location


-'git checkout <HASH> <FILE>': restore <FILE> from version in <HASH>
-'git checkout <HASH>': brings HEAD to <HASH> so you can run things
	-'git checkout main': bring you back to main
	-'git switch main': also brings you back to main
-'git log --oneline --all': show you all the history not just from HEAD

-'.gitkeep': file used as a convention to "keep" folders that are empty 
-'.gitignore': file used by git to match files to ignore

-'ssh-keygen': create an ssh key
	- copy your '˜/.ssh/id_rsa.pub' into your github account
	- use SSH in github not HTTPS

-'git remote add <NAME> <URL>': 'git remote add origin <SSH URL>': create remote >
-'git push origin main': sends code to remote
-'git pull origin main': brings code down from the remote to your local computer
