# P9 - Responsive Navbar and Card Grid Using Flexbox

## Aim
Create a navigation bar and a group of cards that adjust to different screen widths using Flexbox.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Flexbox Layout</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar">
        <h1>Student Hub</h1>
        <div class="nav-links">
            <a href="#">Home</a>
            <a href="#">Courses</a>
            <a href="#">Contact</a>
        </div>
    </nav>

    <main>
        <h2>Learning Cards</h2>
        <div class="card-container">
            <article class="card"><h3>HTML</h3><p>Learn webpage structure.</p></article>
            <article class="card"><h3>CSS</h3><p>Style webpages.</p></article>
            <article class="card"><h3>JavaScript</h3><p>Add interactions.</p></article>
        </div>
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
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 12px;
    padding: 16px 24px;
    background: #263d55;
    color: white;
}

.nav-links {
    display: flex;
    flex-wrap: wrap;
    gap: 18px;
}

.nav-links a {
    color: white;
    text-decoration: none;
}

main {
    padding: 24px;
}

.card-container {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
}

.card {
    flex: 1 1 220px;
    padding: 20px;
    background: #eef3f7;
    border-radius: 8px;
}

@media (max-width: 500px) {
    .navbar {
        align-items: flex-start;
        flex-direction: column;
    }
}
```

## Explanation
- `display: flex` activates Flexbox.
- `justify-content: space-between` places items apart along the main axis.
- `align-items: center` aligns items on the cross axis.
- `flex-wrap: wrap` allows items to move to another line.
- `gap` creates space between items.
- `flex: 1 1 220px` lets cards grow and shrink with a preferred base width.

## Steps
1. Create the HTML and CSS files.
2. Add the navigation and card elements.
3. Apply Flexbox properties.
4. Resize the browser to test the responsive layout.

## Result
A responsive navigation bar and card layout were created using Flexbox.
