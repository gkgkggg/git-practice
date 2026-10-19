# git-practice

A small repository for practicing Git and GitHub in an open source software class.

## Learning goals

- Initialize a Git repository and check file status.
- Stage changes and record meaningful commits.
- Use `.gitignore` to exclude local and private files.
- Connect a local repository to GitHub and push commits.

## Files

| File | Purpose |
| --- | --- |
| `README.md` | Repository overview and usage |
| `.gitignore` | Rules for excluding local files and secrets |
| `git_commands.md` | Notes on the Git commands covered in class |
| `practice.txt` | A short version control practice checklist |
| `hello.py` | A runnable Python example |

## Run the example

Requires Python 3. No additional packages are needed.

```bash
python hello.py
```

Expected output:

```text
Hello, Git and GitHub!
```

## Basic workflow

```bash
git status
git add hello.py
git commit -m "Update greeting example"
git push
```

Never commit passwords, access tokens, or private configuration files.
