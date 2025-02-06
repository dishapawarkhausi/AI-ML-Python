# Git Commands Cheat Sheet

## Setup & Configuration
```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git config --list
```

## Repository Management
```sh
git init                 # Initialize a new Git repository
git clone <repo_url>     # Clone a repository
```

## Basic Snapshotting
```sh
git status                # Check status of working directory
git add <file>            # Stage a specific file
git add .                 # Stage all files
git commit -m "Message"   # Commit staged changes
git commit --amend -m "New Message"  # Amend last commit message
```

## Branching & Merging
```sh
git branch              # List all branches
git branch <branch>     # Create a new branch
git checkout <branch>   # Switch to a branch
git checkout -b <branch>  # Create and switch to a new branch
git merge <branch>      # Merge a branch into the current one
git branch -d <branch>  # Delete a branch
git branch -D <branch>  # Force delete a branch
```

## Remote Repositories
```sh
git remote add origin <url>  # Add a remote repository
git remote -v                # List remote repositories
git push origin <branch>     # Push changes to remote
git push -u origin <branch>  # Push and track branch
git pull origin <branch>     # Pull latest changes
git fetch                    # Fetch changes without merging
git remote remove <name>     # Remove a remote repository
```

## Stashing & Cleaning
```sh
git stash                  # Stash changes
git stash list             # List stashed changes
git stash apply            # Apply last stashed changes
git stash drop             # Drop last stash
git clean -f               # Remove untracked files
```

## Logs & History
```sh
git log                    # View commit history
git log --oneline --graph  # Compact commit history
git diff                   # View unstaged changes
git diff --staged          # View staged changes
```

## Undoing Changes
```sh
git reset HEAD <file>      # Unstage a file
git reset --hard HEAD      # Reset all changes
git revert <commit>        # Revert a commit
```

## Tagging
```sh
git tag                             # List all tags
git tag <tagname>                   # Create a new tag
git tag -a <tagname> -m "Message"   # Annotated tag
git push origin <tagname>           # Push a tag to remote
```

## Submodules
```sh
git submodule add <repo_url>  # Add a submodule
git submodule update --init   # Initialize and update submodules
```

## Git Aliases
```sh
git config --global alias.st status  # Create an alias for status
git config --global alias.co checkout # Create an alias for checkout
```

## Advanced Git
```sh
git cherry-pick <commit>    # Apply a specific commit
git rebase -i HEAD~n       # Interactive rebase of last n commits
git reflog                 # Show history of changes
```

---
**Happy Coding!** 🎯
