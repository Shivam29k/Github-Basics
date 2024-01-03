# Git basics commands

## Initialization of a project on local pc
### ⬇ Create a New Repo in Github account
1. copy the URL of the repo
### ⬇ Create a git Folder
2. `git init` ➡️ Initalizing git in the folder
3. `git remote set-url origin <URL of remote Repo>` ➡️ settifng up remote url
- `git remote -v` ➡️ You can see the git and push as the URL of your remote repo in your github Account


### Now your local folder will get linked to your repo in your github account

### ⬇ Keeping your commits on both local and remote repo
1. `git fetch`➡️ Downloads updates from remote repo without merging.
2. `git merge`➡️ Combines changes from fetched updates into your current branch.

- `git pull`➡️ Downloads and immediately merges updates from remote repo.


### Adding an upstream in the repo

#### what if you want to link another repo inside yours as a part of code and pull all the chages from there whenever it happens ?
### ⬇ Syncing your fork with the original repository
1. `git remote add upstream <original-assignment URL>` ➡️ Adds the repository as a remote named "upstream" as branch.
2. `git fetch upstream` ➡️ Fetches updates from the "upstream" remote (the original repository).
3. `git merge upstream/master` ➡️ Merges updates from the master branch of the "upstream" remote into your current branch.
4. `git rebase upstream/master` ➡️ Reapplies your changes on top of the updates from the master branch of the "upstream" remote.
5. `git push -f origin head` ➡️ Force pushes your current branch to your "origin" remote (your repo), updating it with all changes.


- ## Commonly used Git commands
1. `git clone <repo URL>` ➡️ Creates a local copy of a remote repository.
### ⬇ Commiting a change in repo
2. `git status` ➡️ Shows the status of changes as untracked, modified, or staged.
3. `git add <file>` ➡️ Adds a file to the staging area in preparation for a commit.
4. `git commit -m "<message>"` ➡️ Commits the staged snapshot with a brief log message.
5. `git push origin <branch>` ➡️ Pushes all committed changes on your local branch to a remote repository.

### ⬇ Working with different Brances of Repo 
1. `git checkout -b <new-branch>` ➡️ Creates a new branch and switches to it.
2. `git branch -d <branch>` ➡️ Deletes a branch.
### ⬇ Some otheruseful Commands
1. `git log` ➡️ Shows a chronological commit history for the current branch.
2. `git revert <commit>` ➡️ Creates a new commit that undoes all of the changes made in `<commit>`, then apply it to the current branch.
3. `git reset --hard` ➡️ Discards all history and changes back to the specified commit.