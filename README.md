# Common Git Commands

Common Commands

| Commands | Description |
| -------- | ----------- |
| git init |  Initializes a new Git repository in the current directory. |
| git init \<directory> | Creates a new Git repository in the specified directory.| 
| git status	| Shows the current state of your repository, including tracked and untracked files, modified files, and branch information.| 
| git log --oneline	| Displays the commit history of the current branch.| 
| git add \<file>	| Adds a specific file to the staging area.| 
| git add . or git add –all	| Adds all modified and new files to the staging area.| 
| git commit	| Creates a new commit with the changes in the staging area and opens the default text editor for adding a commit message.| 
| git commit -m “\<message>” | Creates a new commit with the changes in the staging area and specifies the commit message inline.| 
| git diff	| Shows the changes between the working directory and the staging area (index).| 
| git diff \<commit1> \<commit2>	| Displays the differences between two commits.| 
| git diff –staged 	| Displays the changes between the staging area (index) and the last commit.| 
| git diff HEAD	| Display the difference between the current directory and the last commit| 

Branching and Merging 

| Commands | Description |
| -------- | ----------- |
| git branch	| Lists all branches in the repository.|
| git branch \<branch-name>	Creates a new branch with the specified name.| 
| git branch -d \<branch-name>	| Deletes the specified branch.| 
| git switch \<branch-name>	| Switches to the specified branch.| 
| git switch -c \<branch-name>	| Creates a new branch and switches to it.| 
| git merge \<branch>	| Merges the specified branch into the current branch.| 
| git stash	| Stashes the changes in the working directory, allowing you to switch to a different branch or commit without committing the changes.| 
| git stash list	| Lists all stashes in the repository.| 
| git stash pop	| Applies and removes the most recent stash from the stash list.| 
| git stash drop	| Removes the most recent stash from the stash list.| 
| git tag	| Lists all tags in the repository.| 
| git tag \<tag-name>	| Creates a lightweight tag at the current commit.| 
| git tag \<tag-name> \<commit>	| Creates a lightweight tag at the specified commit.| 
| git tag -a \<tag-name> -m “\<message>”	| Creates an annotated tag at the current commit with a custom message.| 

Remote Repositories

| Commands | Description |
| -------- | ----------- |
| git fetch	| Retrieves change from a remote repository, including new branches and commit.| 
| git fetch \<remote>	| Retrieves change from the specified remote repository.| 
| git fetch –prune	| Removes any remote-tracking branches that no longer exist on the remote repository.| 
| git pull	| Fetches changes from the remote repository and merges them into the current branch.| 
| git pull \<remote>	| Fetches changes from the specified remote repository and merges them into the current branch.| 
| git pull –rebase	| Fetches changes from the remote repository and rebases the current branch onto the updated branch.| 
| git push	| Pushes local commits to the remote repository.| 
| git push \<remote>	| Pushes local commits to the specified remote repository.| 
| git push \<remote> \<branch>	| Pushes local commits to the specified branch of the remote repository.| 
| git push –all	| Pushes all branches to the remote repository.| 
| git remote | Lists all remote repositories.| 
| git remote add \<name> \<url>	| Adds a new remote repository with the specified name and URL.| 

Git Comparison

| Commands | Description |
| -------- | ----------- |
| git show	| Shows the details of a specific commit, including its changes.| 
| git show \<commit>	| Shows the details of the specified commit, including its changes.| 
| git reflog	| Shows history of git commands used.| 

Git Managing History

| Commands | Description |
| -------- | ----------- |
| git checkout \<commit-hash>	| Allows us to go back to a previous commit in detached head state. HEAD points directly at that commit rather than a branch | 
| git restore --source HEAD~1 \<filename>	| Restores the contents of the file to its state from the commit prior to HEAD.| 
| git restore --staged \<filename>	| Unstage current staging area so it will not be in the next commit.| 
| git revert \<commit>	| Creates a new commit that undoes the changes introduced by the specified commit.| 
| git revert –no-commit \<commit>	| Undoes the changes introduced by the specified commit, but does not create a new commit.| 
| git reset \<commit-hash>	| Resets the repo back to a specific commit. The commits are gone but not the changes.| 
| git reset --hard \<commit>	| Delete last commit and associated changes.| 
| git rebase \<branch>	| Reapplies commits on the current branch onto the tip of the specified branch.| 

Github

| Commands | Description |
| -------- | ----------- |
| git clone \<repository_url> |  Clones a repository from a remote server to your local machine.| 
| git clone –branch \<branch_name> \<repository_url>	| Clones a specific branch from a repository.| 
