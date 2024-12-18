# Git-task3
# Task List: Focused on Repository Management, Commits, Branching, and Merging

# Part 1: Creating and Cloning Repositories

## Task 1: Create a New Repository
1. Create a new folder for your project and navigate to it:
```bash
mkdir git_task_list3
cd git_task_list3
``` 
2. Initialize git in it
```bash
git init
```
3. Verify the repository status
```bash
git status
```

## Task 2 : Clone a Remote Repository

1. Clone a GitHub repository:

``` bash
git clone https://github.com/Hardagya12/salesforce-clone.git
```
Explanation : This command clones the repository from the specified URL to the current directory.

2.Verify the cloned repository structure:

``` bash
cd repo 
ls -a
```
Explanation : This command lists all the files and directories in the cloned repository.

# Part 2 : Understanding Commits and Commit Messages

## Task 3 : Committing Changes Locally

1. Create new file and add content:

``` bash
echo "Welcome to Git " > README.md
```

2. Stage the file :

``` bash    
git add README.md
```

## Task 4: Write Effective Commit Message

1. Commit the changes:

``` bash
git commit -m "Added initial version of README.md with project overview"
```

Explanation : This command creates a commit with the specified message, which is a description of the changes made in the commit.

2. Commit multiple files with one message:

``` bash
touch file1.txt file2.txt
git add .
git commit -m "Added two new files for feature setup"
```

# Part 3: Viewing Commit History with git log

## Task 5: View Commit History

1. View the commit history:

``` bash
git log
```
Explanation : This command lists the commits in the repository, including commit messages and timestamps.

2. View commit history in a compact format:

``` bash 
git log --oneline
```
Explanation : This command lists the commits in a more compact format, showing only the commit hashes and commit messages.

## Task 6 : Customize Log Outputs

1. View logs with a graphical representation:

``` bash
git log --oneline --graph --decorate
```
Explanation : This command lists the commits in a more compact format, including a graphical representation of the commit history.

2. Filter logs for a specific file :

```
git log README.md
```
Explanation : This command lists the commits that affect the specified file, including commit messages and timestamps.

# Part 4 : Branching and Merging

## Task 7 : Understanding Branches

1. List all branches:

``` bash
git branch
```
Explanation : This command lists all the branches in the repository.

2. Create a new branch:

``` bash
git branch feature-branch
```
Explanation : This command creates a new branch named feature-branch.

3. Switch to a branch:

``` bash    
git checkout feature-branch
```
Explanation : This command switches to the feature-branch branch.

# Part 5 : Creating and Working with Branches

## Task 8 : Make Changes in a Branch

1. Add content to a file:

``` bash
echo "Feature in progress" > feature.txt
git add feature.txt
git commit -m "Added feature.txt in feature-branch"
```
Explanation : This command adds the feature.txt file to the staging area and creates a commit with the specified message.

## Task 9 : Merge Branches

1.Switch back to the main branch:

``` bash
git checkout main
```
Explanation : This command switches back to the main branch.

2. merge the feature-branch branch into the main branch:

``` bash
git merge feature-branch
```
Explanation : This command merges the feature-branch branch into the main branch.

# Part 6 : FUll process to resolve merge conflict

Make two branches main and feature-branch

1. Add content to a file in main branch:

``` bash
echo "Feature in progress" > feature.txt
git add feature.txt
git commit -m "Added feature.txt in feature-branch"
```
Explanation : This command adds the feature.txt file to the staging area and creates a commit with the specified message.

2. Add content to a file in feature-branch branch:

``` bash
echo "Feature in progress" > feature.txt
git add feature.txt
git commit -m "Added feature.txt in feature-branch"
```
Explanation : This command adds the feature.txt file to the staging area and creates a commit with the specified message.

3. Switch back to the main branch:

``` bash
git checkout main
```
Explanation : This command switches back to the main branch.

4. merge the feature-branch branch into the main branch:

``` bash
git merge feature-branch
```
Explanation : This command merges the feature-branch branch into the main branch.

5. Resolve the merge conflict:

Resolve the conflict manually in Vs Code and commit the changes.

``` bash
git commit -m "Resolved merge conflict"
git push origin main
```

---
# Part 7 : Deleting and renaming branch

### Task 11 : Delete a local branch

1. Delete a local branch

``` bash
git branch -d feature-branch
```
Explanation : This command deletes the feature-branch branch locally.

2. Force - delete a branch

``` bash
git branch -D feature-branch
```
Explanation : This command deletes the feature-branch branch forcefully.It will remove the branch even if it has uncommitted changes.

### Task 12 : Rename a branch

1. Rename the current branch

``` bash
git branch -m new-branch-name
```

2. Rename another branch (not checked out)

``` bash 
git branch -m old-branch-name new-branch-name
```
# Summary of Commands

| Command | Description |
| --- | --- |
| `git init` | Initialize a new git repository in the current directory |   
| `git status` | Show the status of the working directory and the staging area |
| `git add <file>` | Add a file to the staging area |
| `git commit -m "<message>"` | Commit the changes in the staging area with a message |
| `git log` | View the commit history |
| `git checkout <branch>` | Switch to a different branch |
| `git branch <branch>` | Create a new branch |
| `git merge <branch>` | Merge a branch into the current branch |
| `git branch -d <branch>` | Delete a local branch |
| `git branch -D <branch>` | Delete a local branch forcefully |
| `git branch -m <old-branch> <new-branch>` | Rename a local branch |
| `git remote add <remote-name> <remote-url>` | Add a remote repository |
| `git push <remote-name> <branch>` | Push a local branch to a remote repository |
| `git pull <remote-name> <branch>` | Pull changes from a remote repository |
| `git fetch <remote-name>` | Fetch changes from a remote repository |
| `git clone <remote-url>` | Clone a remote repository |
| `git stash` | Save uncommitted changes |
| `git stash apply` | Apply saved changes |
| `git stash list` | List saved changes |
| `git stash drop` | Drop saved changes |
| `git stash pop` | Apply and delete saved changes |
| `git tag -a <tag-name> -m "<message>"` | Create a tag and annotate it |
| `git tag -d <tag-name>` | Delete a tag |
| `git tag` | List all tags |
| `git checkout -b <branch>` | Create and switch to a new branch |
| `git rebase -i <commit>` | Use interactive rebase to modify commit messages |
| `git reset --hard <commit>` | Reset the current branch to a specific commit |
| `git reset <file>` | Unstage a file |
| `git clean -f` | Remove untracked files |
| `git config --global alias.st status` | Create an alias for the status command |
| `git config --global alias.cm commit` | Create an alias for the commit command |






