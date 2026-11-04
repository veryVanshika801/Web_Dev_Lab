# P11 - Newspaper-Style Three-Column Layout Using CSS Grid

## Aim
Create a newspaper-style page with three columns using CSS Grid.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Campus Daily</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="masthead">
        <h1>Campus Daily</h1>
        <p>News and updates from campus</p>
    </header>

    <main class="news-grid">
        <article class="story main-story">
            <h2>Technology Club Hosts Workshop</h2>
            <p>Students explored basic web development and learned how websites are structured using HTML and CSS.</p>
        </article>
        <article class="story">
            <h2>Sports Update</h2>
            <p>College teams are preparing for the upcoming sports events.</p>
        </article>
        <article class="story">
            <h2>Library News</h2>
            <p>New learning resources have been added for students.</p>
        </article>
    </main>

    <footer><p>Campus Daily - Student Edition</p></footer>
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
    font-family: Georgia, serif;
    color: #222;
}

.masthead, footer {
    padding: 20px;
    text-align: center;
    background: #24364b;
    color: white;
}

.news-grid {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr;
    gap: 20px;
    padding: 24px;
}

.story {
    padding: 18px;
    background: #f1f3f5;
    border-top: 4px solid #24364b;
}

.main-story {
    grid-column: span 1;
}

@media (max-width: 700px) {
    .news-grid {
        grid-template-columns: 1fr;
    }
}
```

## Explanation
- `display: grid` creates a grid layout.
- `grid-template-columns` defines three columns.
- `2fr 1fr 1fr` gives the first column twice the available space of each other column.
- `gap` creates space between grid items.
- The media query changes the layout to one column on smaller screens.

## Result
A newspaper-style three-column layout was created using CSS Grid.
