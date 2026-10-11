# Proof of Work

## Git Log
```
2cccf4e Merge pull request #1 from Afaqahmed138/development
27ae09b fix: resolved merge conflict
94bdf1f fix: staging label
04094c1 feat: updated script with staging env
3538227 feat: initial commit with deploy script
```

## Reflection Questions
**Q1: Difference between Git and GitHub**

Git is a version control tool that you install on your own machine to record the history of your project's files. It runs fully offline, so you can commit, branch and merge without needing the internet. GitHub is an online service that stores Git repositories in the cloud so many people can work on the same project. It also provides extra tools like pull requests, issue tracking and code review, which Git alone does not have.

**Q2: Working Directory, Staging Area and Local Repository**

The Working Directory is the project folder where you create, edit and delete files directly. The Staging Area is a holding space where you collect the specific changes you want to include in your next commit, which you do with `git add`. The Local Repository is the `.git` folder that keeps the permanent history, and a change reaches it once you run `git commit`. So every change travels from the Working Directory to the Staging Area and finally to the Local Repository.

**Q3: git stash pop vs git stash apply**

Both commands take the changes you previously saved with `git stash` and put them back into your working files. With `git stash pop`, the saved entry is deleted from the stash list right after it is applied. With `git stash apply`, the entry stays in the stash list even after the changes are restored. This makes `apply` helpful when you want to use the same saved changes on more than one branch, while `pop` suits a one-time restore.

**Q4: git fetch vs git pull**

`git fetch` only downloads the latest commits and branch updates from the remote repository and leaves your own files and branch untouched. It lets you look at what others have changed before you decide to combine it with your work. `git pull` performs a fetch and then automatically merges the downloaded changes into your current branch. Because of this, `fetch` is the safer option, while `pull` is quicker but may trigger a merge conflict immediately.
