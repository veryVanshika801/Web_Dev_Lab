# P8 - Sticky Navbar and Card Overlay Using CSS Positioning

## Aim
Create a navigation bar that stays at the top while scrolling and a card with text placed over an image.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Positioning</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar">
        <h2>My Website</h2>
        <a href="#home">Home</a>
        <a href="#about">About</a>
    </nav>

    <main id="home">
        <h1>CSS Positioning Demo</h1>
        <div class="image-card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=900" alt="Laptop on a desk">
            <div class="card-text">
                <h2>Learn and Build</h2>
                <p>Practise HTML and CSS every day.</p>
            </div>
        </div>
        <section id="about">
            <h2>About this page</h2>
            <p>Scroll down to see the sticky navigation bar remain at the top.</p>
        </section>
    </main>
</body>
</html>
```

## Code: style.css
```css
body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.navbar {
    position: sticky;
    top: 0;
    z-index: 10;
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 12px 24px;
    background: #20364d;
    color: white;
}

.navbar a {
    color: white;
    text-decoration: none;
}

main {
    padding: 24px;
}

.image-card {
    position: relative;
    max-width: 700px;
    height: 350px;
    overflow: hidden;
}

.image-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.card-text {
    position: absolute;
    left: 20px;
    bottom: 20px;
    padding: 16px;
    color: white;
    background: rgba(0, 0, 0, 0.65);
}

#about {
    min-height: 500px;
    padding-top: 30px;
}
```

## Explanation
- `position: sticky` keeps the navbar near the top while scrolling.
- `top: 0` sets its top position.
- `position: relative` makes the card the positioning reference.
- `position: absolute` places the text over the image.
- `z-index` controls which positioned element appears in front.

## Steps
1. Create `index.html` and `style.css`.
2. Add the navbar and image card.
3. Link the stylesheet.
4. Open the page and scroll to test the navbar.

## Result
A sticky navbar and an image card with an overlay were created using CSS positioning.

Note: The sample image uses an online image URL, so an internet connection is needed to display it.
