# P1 - Project Folder and Terminal Navigation

## Aim
Create a project folder and practise moving between folders using the terminal.

## 1. Create a project folder

Open Terminal and move to the location where you want to keep your lab work.

```bash
mkdir web-development-lab
cd web-development-lab
```

- `mkdir` creates a new folder.
- `cd` changes the current directory.

## 2. Check the current location

```bash
pwd
```

`pwd` prints the path of the folder you are currently working in.

## 3. Create folders for the practicals

```bash
mkdir P1-project-folder-and-terminal-navigation
mkdir P2-portfolio-repo
mkdir P3-feature-branch-workflow
mkdir P4-readme-and-version-tags
```

## 4. List files and folders

```bash
ls
```

To include hidden files:

```bash
ls -a
```

## 5. Move between folders

```bash
cd P1-project-folder-and-terminal-navigation
cd ..
```

- The first command enters the P1 folder.
- `cd ..` moves one level back to the parent folder.

## 6. Create a small practice file

From inside the P1 folder, run:

```bash
touch notes.txt
```

Open the folder in VS Code (if the `code` command is installed):

```bash
code .
```

## Expected result

The project folder should contain separate folders for the practicals. The terminal commands should let you enter a folder, return to the parent folder, and list the folder contents.

## Commands used

| Command | Purpose |
|---|---|
| `mkdir` | Creates a folder |
| `cd folder-name` | Enters a folder |
| `cd ..` | Goes to the parent folder |
| `pwd` | Shows the current folder path |
| `ls` | Lists visible files and folders |
| `ls -a` | Lists visible and hidden files |
| `touch file-name` | Creates an empty file |

## Note
Run these commands one at a time. If a folder already exists, `mkdir` may show a message; that does not mean the existing folder was deleted.
