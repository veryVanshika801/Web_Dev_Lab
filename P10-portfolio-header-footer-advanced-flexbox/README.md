# P10 - Portfolio Header and Footer with Advanced Flexbox

## Aim
Design a portfolio header and footer using Flexbox alignment, spacing, wrapping and flexible sizing.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="header">
        <a class="logo" href="#">MyPortfolio</a>
        <nav class="navigation">
            <a href="#about">About</a>
            <a href="#work">Work</a>
            <a href="#contact">Contact</a>
        </nav>
        <a class="resume" href="#contact">Contact Me</a>
    </header>

    <main>
        <section id="about"><h1>Welcome to My Portfolio</h1><p>I am learning web development.</p></section>
        <section id="work"><h2>My Work</h2><p>Small projects and practice work.</p></section>
    </main>

    <footer class="footer" id="contact">
        <p>© 2026 MyPortfolio</p>
        <div class="footer-links">
            <a href="#about">About</a>
            <a href="#work">Projects</a>
            <a href="mailto:student@example.com">Email</a>
        </div>
    </footer>
</body>
</html>
```

## Code: style.css
```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 16px;
    padding: 18px 5%;
    background: #1f3448;
}

.logo {
    font-size: 22px;
    font-weight: bold;
    color: white;
    text-decoration: none;
}

.navigation, .footer-links {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.navigation a, .footer a {
    color: white;
    text-decoration: none;
}

.resume {
    padding: 10px 16px;
    color: #1f3448;
    background: white;
    border-radius: 5px;
    text-decoration: none;
}

main {
    min-height: 400px;
    padding: 40px 5%;
}

.footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 16px;
    padding: 24px 5%;
    color: white;
    background: #1f3448;
}

@media (max-width: 600px) {
    .header, .footer {
        flex-direction: column;
        align-items: flex-start;
    }
}
```

## Explanation
- Flexbox arranges the header items in one row.
- `justify-content: space-between` distributes free space.
- `align-items: center` aligns items vertically in the row.
- `flex-wrap: wrap` allows items to wrap on smaller screens.
- The media query changes the header and footer to a column on narrow screens.

## Result
A portfolio header and footer were designed using advanced Flexbox properties.
