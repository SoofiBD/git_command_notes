GIT: A Comprehensive Guide to Version Control

Git is a distributed version control system commonly used in software development. Below is an in-depth explanation of Git's key features:

1. Configuration:

Before you begin with Git, it's crucial to set up your user details.

git config --global user.name "Your Name": Identifies the author of the commit.
git config --global user.email "Your Mail": Identifies the email of the commit author.
git config --list: Displays all configuration settings.

2. Initializing and Cloning a Repository:

git init: Initializes a new Git repository in the current directory.
git clone <URL>: Downloads a repository from a remote source (like GitHub).

3. Staging Changes:
   
Before committing changes, you first stage them.

git add <filename>: Adds a specific file to the staging area.
git add .: Adds all changes in the current directory to the staging area.
git status: Shows the status of changes (staged, unstaged, and untracked).

4. Committing Changes:

git commit -m "Descriptive message": Saves your changes to the local repository.

5. Viewing Commit History and Differences:

git log: Displays the commit logs.
git diff: Shows the differences between the working directory and the last commit.

6. Branching and Merging:
7. 
Branches help you develop features or fix bugs without affecting the main codebase.

git branch: Lists all branches.
git branch <branch_name>: Creates a new branch.
git switch <branch_name> or git checkout <branch_name>: Moves to the specified branch.
git merge <branch_name>: Merges the specified branch into the current one.

7. Conflicts:

If the same part of a file has been modified differently in two branches, you'll face a merge conflict. You'll need to resolve it manually.

9. Remote Repositories:

git remote add <name> <URL>: Links a remote repository.
git push <remote_name> <branch_name>: Uploads local repository content to a remote repo.
git pull <remote_name> <branch_name>: Fetches and merges changes from a remote repository.

9. Stashing:

git stash: Temporarily saves changes that you don't want to commit yet.
git stash list: Displays all stashed changes.
git stash apply: Restores the most recently stashed changes.
git stash drop: Discards the most recently stashed changes.

10. Resetting and Reverting:

git reset --hard <commit_id>: Resets your branch to a specific commit and discards changes.
git revert <commit_id>: Creates a new commit that undoes changes from a specified commit.

11. Tagging:
    
Tags are references to specific points in Git history.

git tag: Lists all tags.
git tag -a <tag_name> -m "message": Creates an annotated tag.

12. Git Ignore:
    
Using a .gitignore file, you can specify files or directories that Git should ignore. It's essential for excluding files that you don't want to be tracked (like logs, compiled files, etc.).

14. Fetching:

git fetch: Downloads objects and refs from another repository without integrating them into your workspace. This is different from pull, which fetches and then merges.
14. Cherry-picking:

git cherry-pick <commit_id>: Allows you to take a commit from another branch and apply it onto your current branch.
