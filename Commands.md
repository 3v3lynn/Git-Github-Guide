

## **Configure Git (first time setup)**

```bash
git config --global user.name "Your Name" 
git config --global user.email "your@email.com"
```

> Sets your name and email for Git commit history.


## Start a new repo or clone one

| Command           | Explanation                                   |
| ----------------- | --------------------------------------------- |
| `git init`        | Initializes a new local Git repository.       |
| `git clone <URL>` | Clones a remote GitHub repo to your computer. |


## **Basic workflow (local changes)**

``` bash
git status               # Check status of your files 
git add <file>           # Stage a specific file 
git add .                # Stage all changes 
git commit -m "Message"  # Save staged changes as a commit
```

> These are the essential steps to save your work locally.


## View history and changes

|Command|Explanation|
|---|---|
|`git log`|Shows full commit history.|
|`git log --oneline`|Short version of commit history.|
|`git diff`|Shows unstaged changes.|
|`git diff --staged`|Shows staged but uncommitted changes.|


## Work with branches

```bash
git branch                # List all branches
git branch <name>`        # Create new branch
git checkout <name>       # Switch to a branch
git checkout -b <name>    # Create and switch to a branch
git merge <branch>`       # Merge a branch into the current one
git branch -d <branch>`   # Delete a branch
```


## **Connect Git to GitHub**

1. Create a new repo on GitHub
    
2. Link it to your local repo:

```bash
git remote add origin https://github.com/yourusername/repo-name.git
git branch -M main                         # Rename to 'main' if needed
git push -u origin main                    # Push your code to GitHub
```

`origin` is the default name for the remote repo.


## Push & pull from GitHub

|Command|Explanation|
|---|---|
|`git push`|Upload local commits to GitHub.|
|`git pull`|Download and merge changes from GitHub.|
|`git fetch`|Download changes but **don’t merge** automatically.|


## Other useful commands

|Command|Explanation|
|---|---|
|`git stash`|Temporarily saves changes without committing.|
|`git stash apply`|Re-applies stashed changes.|
|`git reset <file>`|Unstage a file.|
|`git reset --hard`|Revert all changes (⚠️ permanent).|
|`git revert <commit>`|Creates a new commit that undoes a specific commit.|


## ## **Typical Git + GitHub workflow**

1. `git init` (or `git clone`)
    
2. Make changes
    
3. `git add .`
    
4. `git commit -m "message"`
    
5. `git push`


## Git Help

If you are having trouble remembering commands or options for commands, you can use Git `help`.

There are a couple of different ways you can use the `help` command in command line:

- `git _command_ -help` -  See all the available options for the specific command
- `git help --all` -  See all possible commands