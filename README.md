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