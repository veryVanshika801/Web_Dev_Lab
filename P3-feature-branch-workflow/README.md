# P3 - Feature-Branch Git Workflow

## Aim
Practise creating a separate branch, making a change, committing it, and merging it into the main branch.

## What is a branch?
A branch is a separate line of work in a Git repository. It lets us develop a feature without directly changing the main branch.

## Steps

### 1. Check the current branch
```bash
git branch
```
The current branch is marked with `*`.

### 2. Create and move to a feature branch
```bash
git switch -c feature/add-about-page
```
This creates the branch and switches to it.

### 3. Make a small change
Create a file named `about.html` in the project folder:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>About Me</title>
</head>
<body>
    <h1>About Me</h1>
    <p>This page contains information about my portfolio.</p>
    <a href="index.html">Back to Home</a>
</body>
</html>
```

### 4. Save the change in Git
```bash
git status
git add about.html
git commit -m "Add about page"
```

### 5. Return to main and merge the feature
```bash
git switch main
git merge feature/add-about-page
```
The merge brings the committed change from the feature branch into `main`.

### 6. Check branches and history
```bash
git branch
git log --oneline --graph --all
```
Optional: after confirming the merge, delete the local feature branch:
```bash
git branch -d feature/add-about-page
```

## Result
A feature was developed and committed on a separate branch, then merged into the main branch.

## Important notes
- Make sure the feature branch is committed before merging.
- If Git reports a merge conflict, open the affected file, resolve the marked sections, then stage and commit the resolved file.
- These commands work locally. Pushing to GitHub is not required unless separately asked.
