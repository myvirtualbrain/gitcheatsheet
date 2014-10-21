Install git
http://git-scm.com

Check git version (if it's installed)
$ git --version

Set your git name (globally)
$ git config --global user.name "your username"

Set your git email address (globally)
$ git config --global user.email "your email address"

Set your github username
$ git config --global user.username "YourGithubUsername"

Initiate a new repository. This creates a hidden .git folder.
$ git init

Remove bindings (git repositry from projects root folder)
$ rm -R .git 

See git status
$ git status

Add a file to be commited
$ git add "filename"

Add all changed files
$ git add .

Commit added changes in repository
$ git commit -m "your message about the committed files"

Commit all files (without having to add them manually beforehand)
$ git commit -a 

See difference between your current file now and it's last commit
$ git diff

Setup main remote repository 
$ git remote add origin "https://github.com/myvirtualbrain/practise.git"

Push changes to remote repository, master is the default branch name and origin is our remote main repository
$ git push origin master


==== Fork others repos ====
1. In github, press the fork icon for wanted repo
Copy the github address to your forked repo

To make a local repository from the forked (in a non-git folder)
$ git clone "Url from github"

We want to be getting changes from original repo aswell so we need to add an remote connection. Most person use the name: upstream
$ git remote add "a name" "url to orginial repo"

Pull from original repo
$ git pull upstream "branch name"

==== Branches ====
Create a new branch of a repository
$ git branch "your branch name"

Switch to a certain branch
$ git checkout "branch name"

Delete a local branch
$ git branch -d "branch name"

Delete a remote branch
$ git push origin :"branch name"
OR
$ git push "remote name" --delete "Branch name"

Push new branch to remote repository
$ git push origin "branch name"

====

Get changes from others, if any
$ git pull "remote name" "branch name"

==== Merging ====
Stand in the target branch and merge from given source branch
$ git merge "source branch name"






