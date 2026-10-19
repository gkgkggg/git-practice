# Git Command Notes

## Three areas

Working directory -> staging area -> local repository.

`git add` stages the current contents of a file. `git commit` records the staged
snapshot. `git push` sends local commits to a remote repository.

## Common commands

| Command | Purpose |
| --- | --- |
| `git init` | Initialize a repository in the current directory |
| `git status` | Check tracked, untracked, modified, and staged files |
| `git add <file>` | Stage the current changes to one file |
| `git add .` | Stage changes under the current directory |
| `git commit -m "message"` | Record staged changes with a message |
| `git log --oneline` | Show a compact commit history |
| `git branch` | List local branches |
| `git branch -M main` | Rename the current branch to main |
| `git remote -v` | Show configured remote repository URLs |
| `git push -u origin main` | Push main and set its upstream branch |

## Undoing changes

- `git restore --staged <file>` unstages a file while keeping working changes.
- `git restore <file>` discards unstaged changes to a tracked file by restoring
  its staged version. Use it only when those changes are no longer needed.

## Removing and renaming files

- `git rm <file>` removes the working file and stages its deletion.
- `git rm --cached <file>` stops tracking the file but keeps the working copy.
  This does not remove the file from earlier commits.
- `git mv <old> <new>` renames a file and stages the change.

## Ignored files

`.gitignore` defines files that Git should ignore when they are untracked.
Adding an already tracked file to `.gitignore` does not stop tracking it.

## Connecting to GitHub

```bash
git remote add origin https://github.com/gkgkggg/git-practice.git
git remote -v
git push -u origin main
```

Authenticate through a trusted GitHub sign-in flow. Never put an access token
in a remote URL, command note, or committed file.
