# P12 - Portfolio Projects Grid with Advanced CSS Grid

## Aim
Display portfolio project cards using advanced CSS Grid properties such as repeat(), minmax(), auto-fit and gap.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Projects</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header><h1>My Projects</h1><p>A few things I have practised</p></header>

    <main class="projects-grid">
        <article class="project"><h2>Portfolio</h2><p>A personal webpage using HTML and CSS.</p></article>
        <article class="project"><h2>Task Tracker</h2><p>A simple way to organise tasks.</p></article>
        <article class="project"><h2>Study Notes</h2><p>A small collection of learning notes.</p></article>
        <article class="project"><h2>Club Website</h2><p>A webpage for a student technology club.</p></article>
        <article class="project"><h2>News Layout</h2><p>A newspaper layout using CSS Grid.</p></article>
        <article class="project"><h2>Bio Page</h2><p>A semantic HTML biography page.</p></article>
    </main>
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
    background: #f4f6f8;
}

header {
    padding: 28px;
    text-align: center;
    color: white;
    background: #243b53;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
    padding: 28px;
}

.project {
    min-height: 160px;
    padding: 20px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

.project h2 {
    margin-top: 0;
    color: #243b53;
}
```

## Explanation
- `repeat()` repeats a column pattern.
- `auto-fit` fits as many columns as possible into the available space.
- `minmax(220px, 1fr)` gives each column a minimum width of 220px and lets it grow.
- `gap` adds space between cards.
- The grid automatically adjusts as the screen becomes wider or narrower.

## Result
A responsive portfolio projects grid was created using advanced CSS Grid properties.
