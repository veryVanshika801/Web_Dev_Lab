# P4 - GitHub README and Version Tags

## Aim
Write a useful README file for a project and learn how to create and view Git version tags.

## 1. Purpose of README.md
A README is the main information page of a repository. It explains what the project does and how someone can use it.

A useful README normally contains:
- Project name and short description
- Features
- Tools or technologies used
- Folder structure
- Steps to run or view the project
- Author or contact information, if required

## 2. Example README for the portfolio project
Save this as `README.md` in the root of the portfolio repository and change sample details if needed.

```markdown
# My Portfolio

A simple personal portfolio webpage created using HTML and CSS.

## About
This project introduces me and presents my basic skills and contact information.

## Features
- About Me section
- Skills section
- Contact section
- Simple CSS styling

## Technologies Used
- HTML5
- CSS3

## How to View
1. Download or clone the project.
2. Enter the project folder.
3. Open index.html in a web browser.

## Project Files
- index.html - webpage structure
- style.css - webpage styling

## Author
Your Name
```

## 3. Add and commit the README
Run these commands from the repository folder:
```bash
git add README.md
git commit -m "Add project README"
```

## 4. Create a version tag
A Git tag marks a particular commit, often to identify a release version.
```bash
git tag v1.0.0
```
To see available tags:
```bash
git tag
```
To see the commit details for a tag:
```bash
git show v1.0.0
```
An annotated tag can also be created with a message:
```bash
git tag -a v1.0.0 -m "First portfolio version"
```
Use one of the tag-creation commands, not both for the same tag name.

## 5. Push a tag to GitHub (only after permission)
```bash
git push origin v1.0.0
```
To push all local tags:
```bash
git push origin --tags
```
These commands contact GitHub. Do not run them until the work is ready and permission has been given.

## Result
A project README was prepared and Git version-tag commands were practised to identify a project version.

**Note:** The lab sheet gives the practical title but does not specify a required README template or tag number. The example uses `v1.0.0` as a sample version.
