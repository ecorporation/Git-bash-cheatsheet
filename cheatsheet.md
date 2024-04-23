## Getting Started

```git config --global user.name "[USERNAME]"```

```git config --global user.email [EMAIL]```

## Repository actions

### Initialize repository

```git init -b [BRANCH NAME]``` : Initializes a new Git repository in the current directory and sets the initial branch to `[BRANCH NAME]`. If `[BRANCH NAME]` is not provided, it defaults to main.

```git add . / [FILENAME]``` : Adds all files `.` or specific files `[FILENAME]` to the staging area, preparing them for the first commit.

```git commit -m "[COMMIT MESSAGE]"``` : Commits the staged changes with a descriptive commit message.

```git remote add origin [REMOTE URL]``` : Sets the URL for the remote repository, named 'origin' by convention.

```git remote -v``` : Verifies that the remote URL is correctly set.

```git push origin [BRANCH NAME]``` : Pushes the committed changes from the local repository to the remote repository specified by `origin`.

### Rename repository

```git remote rename [OLD NAME] [NEW NAME]```

### Delete repository

```git remote remove [REPO NAME]```

### Clone repository 

```git clone [REMOTE URL]``` : Copies a remote repository to your local machine.

### Pull repository

```git pull origin [BRANCH NAME]``` : Fetches changes from the remote repository and integrates them into the current local branch.

## File actions

```git rm [FILENAME]``` : Removes the specified file from the staging area and working directory.

```git status``` : Displays the status of the working directory, including which files are staged, unstaged, or untracked.

## Commit history

```git log``` : Displays the commit history of the current branch.

```git log -p``` : Shows the commit history with the diff of each commit.

```git log --stat``` : Provides a concise summary of the commit history with statistics like insertions and deletions.

```git log --graph``` : Visualizes the commit history as a graph, showing branching and merging.

## Branch actions

### Creating branch

```git branch [BRANCH NAME]``` : Creates a new branch named `[BRANCH NAME]`.

### Change branch

```git checkout testing``` :  Switches to the branch `[BRANCH NAME]`.

### Delete branch

```git branch -d [BRANCH NAME]```

### Create and change branch

```git checkout -b testing``` :  Creates and switches to a new branch named `[BRANCH NAME]`.

### Merge branch

```git merge [BRANCH NAME (FROM)]``` : Integrates changes from `[BRANCH NAME (FROM)]` into the current branch.

### List branches

```git branch``` :  Lists all local branches.

```git branch -v``` : Lists all local branches with additional information like the last commit on each branch.
