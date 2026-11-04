# P6 - Full Portfolio Page Structure in Semantic HTML

## Aim
Build a portfolio page using semantic HTML sections.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Portfolio</title>
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>I am a student learning programming and web development.</p>
        </section>

        <section id="skills">
            <h2>Skills</h2>
            <ul>
                <li>HTML</li>
                <li>CSS</li>
                <li>Java basics</li>
                <li>Python basics</li>
            </ul>
        </section>

        <section id="projects">
            <h2>Projects</h2>
            <article>
                <h3>Portfolio Website</h3>
                <p>A simple website made using HTML and CSS.</p>
            </article>
            <article>
                <h3>Student Task Tracker</h3>
                <p>A basic project to organise student tasks.</p>
            </article>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <p>Email: student@example.com</p>
        </section>
    </main>

    <footer>
        <p>© 2026 Student Portfolio</p>
    </footer>
</body>
</html>
```

## Explanation
- `header`: page title and navigation.
- `nav`: links to different sections.
- `main`: the main portfolio content.
- `section`: groups About, Skills, Projects and Contact.
- `article`: independent project information.
- `footer`: closing details.

## Steps
1. Create `index.html`.
2. Add the semantic structure shown above.
3. Save and open it in a browser.
4. Test each navigation link.

## Result
A complete basic portfolio structure was created using semantic HTML.
