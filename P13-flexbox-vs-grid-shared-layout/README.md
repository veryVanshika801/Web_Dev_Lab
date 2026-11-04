# P13 - Choosing Between Flexbox and Grid for a Shared Layout

## Aim
Understand when to use Flexbox or Grid and create a shared page layout using both.

## Difference between Flexbox and Grid

| Flexbox | CSS Grid |
|---|---|
| Mainly one-dimensional | Two-dimensional |
| Arranges items in a row or column | Arranges items in rows and columns |
| Useful for navigation bars and button groups | Useful for page sections and card layouts |
| Controls space along one main axis | Controls rows and columns together |

## Example: HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox and Grid</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="topbar">
        <h1>Student Space</h1>
        <nav>
            <a href="#">Home</a>
            <a href="#">Notes</a>
            <a href="#">Projects</a>
        </nav>
    </header>

    <main class="page-grid">
        <section class="content">
            <h2>Welcome</h2>
            <p>This main area is placed using CSS Grid.</p>
        </section>
        <aside class="sidebar">
            <h2>Quick Links</h2>
            <p>Notes, timetable and resources.</p>
        </aside>
    </main>

    <footer><p>© 2026 Student Space</p></footer>
</body>
</html>
```

## Example: CSS
```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.topbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 12px;
    padding: 16px 24px;
    color: white;
    background: #263d55;
}

.topbar nav {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
}

.topbar a {
    color: white;
    text-decoration: none;
}

.page-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 20px;
    padding: 24px;
    min-height: 300px;
}

.content, .sidebar {
    padding: 20px;
    background: #eef3f7;
    border-radius: 8px;
}

footer {
    padding: 18px;
    text-align: center;
    color: white;
    background: #263d55;
}

@media (max-width: 650px) {
    .page-grid {
        grid-template-columns: 1fr;
    }
}
```

## Explanation
- Flexbox is used for the header because its items are arranged in one row and may wrap.
- Grid is used for the main content because it needs two columns: content and sidebar.
- Both systems can be used together in the same webpage.
- Choose the layout system based on how the elements need to be arranged.

## Result
A shared webpage layout was created using Flexbox for the header navigation and Grid for the main content.
