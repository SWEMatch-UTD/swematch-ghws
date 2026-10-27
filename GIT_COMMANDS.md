# Introductory Git Commands

## Setup
- `git clone <url>`: copies a GitHub repo onto your computer.

## Checking the state
- `git status`: shows which files changed and what's staged.
- `git log --oneline`: lists past commits, one line each.
- `git branch`: lists your local branches and marks the current one.
- `git branch -a`: lists your local and remote branches.

## Saving your work
- `git diff`: shows exactly which lines you changed.
- `git add .`: stages every changed file in the folder.
- `git commit -m "message"`: saves the staged changes as a snapshot with a message.

## Sharing with GitHub
- `git push`: uploads your commits to GitHub.
- `git push -u origin <branch>`: pushes a new branch for the first time and links it to GitHub.
- `git pull`: downloads new commits from GitHub and merges them into your branch.
- `git pull --no-rebase origin main`: downloads the latest `main` and merges it into your current branch. Use this to get new files (like `styles.css`) from `main`.
- `git pull --no-rebase origin <your-branch>`: if your push is rejected because a teammate pushed first, run this, then push again.
- `git fetch`: downloads new commits from GitHub without changing your files.

## Branching
- `git switch <branch>`: moves you onto an existing branch.
- `git checkout <branch>`: also moves you onto an existing branch.
- `git checkout -b <branch>`: Creates a new branch from your current branch and moves you to that newBranch.


## Pull requests (on GitHub)
- After you push, open your repo on GitHub and click **Compare & pull request** to ask for your branch to be merged into `main`.

## Combining and updating
- `git merge <branch>`: brings another branch's commits into your current branch.
- `git pull --rebase origin main`: updates your branch by replaying your commits on top of the latest `main`.
- `git rebase --continue`: carries on a rebase after you've fixed a conflict.
- `git rebase --abort`: cancels a rebase and puts everything back as it was.
- `git push --force-with-lease`: safely force-pushes after a rebase, failing if someone else pushed.

## Undoing mistakes
- `git restore <file>`: throws away your unsaved changes to a file.
- `git restore --staged <file>`: unstages a file but keeps your edits.
- `git revert <commit>`: makes a new commit that undoes an earlier one.
