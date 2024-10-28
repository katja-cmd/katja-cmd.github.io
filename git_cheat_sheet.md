# Git cheat sheet

### The everyday commands

| Command                     | Description                                                                                  |
|-----------------------------|----------------------------------------------------------------------------------------------|
| `git status`                | Shows the current status of the working directory and staging area.                          |
| `git add <file>`            | Adds a file to the staging area, preparing it for a commit.                                  |
| `git add .`                 | Stages all changes (new, modified, deleted) in the current directory for commit.             |
| `git commit -m "message"`   | Commits the staged changes with a descriptive message.                                       |
| `git pull`                  | Fetches changes from the remote repository and merges them into the current branch.          |
| `git push`                  | Pushes local commits to the remote repository.                                               |
| `git fetch`                 | Retrieves changes from the remote repository without merging them into the current branch.   |


### Other commands

| Command                     | Description                                                                                  |
|-----------------------------|----------------------------------------------------------------------------------------------|
| `git init`                  | Initializes a new Git repository in the current directory.                                   |
| `git clone <repo_url>`      | Creates a local copy of a remote repository.                                                 |
| `git commit -am "message"`  | Adds and commits tracked files in one step (useful for small changes).                      |
| `git branch`                | Lists all branches in the repository.                                                        |
| `git branch <branch_name>`  | Creates a new branch.                                                                        |
| `git checkout <branch>`     | Switches to the specified branch.                                                            |
| `git checkout -b <branch>`  | Creates a new branch and switches to it immediately.                                         |
| `git merge <branch>`        | Merges the specified branch into the current branch.                                         |
| `git log`                   | Displays the commit history for the current branch.                                          |
| `git diff`                  | Shows changes between commits, branches, or the working directory and staging area.          |
| `git stash`                 | Temporarily stores uncommitted changes for later retrieval.                                  |
| `git stash pop`             | Restores the most recently stashed changes and removes them from the stash list.             |
| `git remote -v`             | Lists remote repositories associated with the project.                                       |
| `git reset <file>`          | Removes a file from the staging area without changing the working directory.                 |
| `git reset --hard`          | Discards all local changes and resets the repository to the last committed state.            |
| `git rm <file>`             | Removes a file from the repository and the working directory.                                |
| `git tag <tag_name>`        | Creates a tag at the current commit (useful for marking releases or versions).               |
| `git rebase <branch>`       | Reapplies commits from the current branch onto the specified base branch.                    |
| `git cherry-pick <commit>`  | Applies a specific commit from one branch into another branch.                               |
| `git config`                | Configures Git settings, such as user name and email.                                        |
| `git blame <file>`          | Shows the last commit made for each line in a file (useful for tracking changes).            |
