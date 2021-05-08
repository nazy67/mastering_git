### Git commands

```
git init
```
this command initializes git in the working directory.
```
git add
```
this command adds the files to staging area. It doesn't just mean adding files, it means to add changes to the staging area and tracking happens only after git add. You can either files with ```git add .``` or ```git add filename``` if you want to add a specific file into the staging area.
```
git commit
```
this command records the file in the version history.
```
git diff
```
this command shows the file differences which are not staged yet. When you want to know changes which changes are made ```git diff``` is the command to run. If you want to see changes in a specific file you run ```git diff filename```. git diff shows differences between commited and modified files.
```
git diff --staged 
```
this command shows as well as previous command, the differences between staging and latest version of your file. git diff --staged will compare files in staging area with the last file version.
```
git reset
```
this command unstages staged files.
```
git status
```
this command lists all the files that have to be tracked or/and commited.
```
git restore --stage
```
this command unstages the files.
```
git log 
```
this command will show all your commits, that you made in your working directory.
```
git show "commit id" 
```
this command will show the metadata of the commit and the content of the changes.
```
git rm 
```
this command will delete a file, but you have to let commited area know about deletion (that the file was deleted)
```
git rm -f or --force
```
this command will forcefully delete a file and override the up-to-date check.
```
git revert 'commit id'
```
this command reverts commits it is a dangerous command to run, but helpful if you can revert back to the previous version of your file. 
```
git config --list
```
this command will show the global git configuration.
```
git config user.name
```
this command will show the name of the user.
```
git config user.email
```
this command will show  an email of the user(author)
the both commands above will set the author. When you git commit is done by author, it will be easier to track down who made the changes.
```
git branch "branch name"
```
this command will create a new branch, usually branches created locally.
```
git checkout "branch name"
```
this command will change the branch
```
git pull
```
this command will sync your local branch with remote branch
```
git fetch origin branch_name
git checkout branch_name
```
this command will copy the branch from remote repository.
```
git rebase origin 
```
this command will sync the remote main branch with local branch
```
git branch -d feature/nazy
```
this command will delete local feature branch
```
git push origin --delete feature/nazy
```
this command will delete remote feature branch
```
git clone --branch `branchname` git@github.com:aKumoSolutions/git-april2021.git
```
this command will clone a specific branch from the remote repository

#### Notes

- Adding/removing a content from the file is modification.

- git commit message should be (length of it) 72 characters, under 80 characters.

- Staging happens after git add, when you are commiting or staging, always run git status.

- Git doesn't recognize an empty folder, it won't track it. But if you create a file inside of it it will show on ```git status```.

- There are three states of a file in a git: modified, staged and commited.

- Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

- Merging pull requests (PR) also will be tracked as a commit

### Git vs GitHub

GitHub is not Git. GitHub is a website for hosting projects that use Git. Git is a tool a developer installs locally on their computer, while GitHub is an online service that stores  pushed code to it from computers running the Git tool. The main difference between Git and GitHub is in their functionality. While they both provide source code management (SCM) and make merging and sharing code easier, this is pretty much where their similarities end. Think of Git as a single computer and GitHub as a network of multiple interconnected computers, all with the same end goal but a wildly different role for how to get there.
GitHub is  a hosted Git ,  allows you to create repositories and keep a track of your code.  Git is a tool that supports the version control system. 
