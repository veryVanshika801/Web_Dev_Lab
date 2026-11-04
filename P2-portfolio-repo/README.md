# P2 - Portfolio Repository with an Initial Commit

## Aim
Create a simple personal portfolio project, initialise Git, and save its first version as a commit.

## 1. Create the project files
```text
P2-portfolio-repo/
├── index.html
└── style.css
```

## 2. HTML file (index.html)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <p>First-year BTech student | Learning web development</p>
    </header>
    <main>
        <section>
            <h2>About Me</h2>
            <p>Hello! I am a student learning HTML, CSS and programming.</p>
        </section>
        <section>
            <h2>My Skills</h2>
            <p>HTML, CSS, Java and Python basics</p>
        </section>
        <section>
            <h2>Contact</h2>
            <p>Email: student@example.com</p>
        </section>
    </main>
    <footer><p>© 2026 My Portfolio</p></footer>
</body>
</html>
```
Replace the sample details with your own details. The email is only a placeholder.

## 3. CSS file (style.css)
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background-color: #f4f4f4;
    color: #222;
}
header, footer {
    text-align: center;
    background-color: #243447;
    color: white;
    padding: 20px;
}
main {
    max-width: 800px;
    margin: 20px auto;
    padding: 0 16px;
}
section {
    background-color: white;
    margin-bottom: 16px;
    padding: 18px;
    border-radius: 8px;
}
```

## 4. Initialise Git and make the first commit
The example is inside the lab folder for easy review. Copy it to a separate location to make it an independent portfolio repository. From the lab folder:

```bash
cp -R P2-portfolio-repo ../my-portfolio
cd ../my-portfolio
git init
git status
git add index.html style.css
git commit -m "Create initial portfolio page"
```

On Windows, copy the P2 folder using File Explorer and rename the copy to `my-portfolio`, then open a terminal inside it.

If Git asks for your name and email, configure your commit identity:
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
Then run the commit command again.

## 5. Check the result
```bash
git log --oneline
```
The first commit should appear with the message `Create initial portfolio page`.

## Result
A basic portfolio webpage was created and its first version was saved in Git history.

**Note:** This demonstrates a local Git repository and an initial commit. Connecting it to GitHub and pushing are separate steps.
