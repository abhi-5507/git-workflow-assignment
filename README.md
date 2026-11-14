# Git & GitHub Workflow Assignment

**Student:** Pasumarthi Abhiram  
**Roll Number:** 2024EB01513  
**Subject:** Software Development Practice  
**College:** BITS Hyderabad  
**Submission Date:** 14-11-2026

## Project files
- `index.html` — home page
- `about.html` — about page
- `feature.html` — feature page (created on the `feature` branch)
- `.gitignore` — ignores `.log` files and `temp/`
- `git_commands.txt` — Git commands with explanations
- `git_execution_evidence.txt` — repository history and verification record

## Public GitHub repository
https://github.com/abhi-5507/git-workflow-assignment

## Reproduce the local workflow
The assignment requires the workflow to be performed on a local machine. To reproduce it locally, create this project folder, copy the files into it, and initialize Git locally:

```bash
git init -b main
git add index.html about.html
git commit -m "Initial project structure"
git add index.html
git commit -m "Update home page content"
git switch -c feature
git add feature.html
git commit -m "Add feature page"
git switch main
git merge feature
git add .gitignore
git commit -m "Add gitignore rules"
git add about.html
git commit -m "Add temporary about page update"
git revert --no-edit HEAD
git log --oneline --graph --decorate --all
```

The public repository above contains the project files, both branches, a merge commit, and a revert commit. Check the commit graph on GitHub before submission.
