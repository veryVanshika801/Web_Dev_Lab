# P7 - Design Tokens and Typography System in CSS

## Aim
Create reusable CSS variables (design tokens) for colours, spacing and typography.

## Code: index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Tokens Demo</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="site-header">
        <h1>My Design System</h1>
    </header>

    <main class="content">
        <section class="card">
            <h2>Typography and Colours</h2>
            <p>This page uses CSS variables for a consistent design.</p>
            <button>Explore</button>
        </section>
    </main>
</body>
</html>
```

## Code: style.css
```css
:root {
    --color-primary: #24476b;
    --color-background: #f2f5f8;
    --color-text: #222222;
    --space-small: 8px;
    --space-medium: 16px;
    --space-large: 32px;
    --font-main: Arial, sans-serif;
    --text-small: 14px;
    --text-normal: 16px;
    --text-large: 28px;
}

body {
    margin: 0;
    font-family: var(--font-main);
    font-size: var(--text-normal);
    color: var(--color-text);
    background: var(--color-background);
}

.site-header {
    padding: var(--space-medium);
    color: white;
    background: var(--color-primary);
}

.content {
    padding: var(--space-large);
}

.card {
    max-width: 600px;
    padding: var(--space-large);
    background: white;
    border-radius: 10px;
}

h1, h2 {
    font-size: var(--text-large);
}

button {
    padding: var(--space-small) var(--space-medium);
    color: white;
    background: var(--color-primary);
    border: 0;
    border-radius: 5px;
}
```

## Explanation
- `:root` stores variables that can be reused throughout the stylesheet.
- `--color-primary` stores the main colour.
- `--space-medium` stores a spacing value.
- `var(--variable-name)` uses a stored value.
- Design tokens make it easier to update a website's design consistently.

## Steps
1. Create `index.html` and `style.css`.
2. Link the CSS file in the HTML head.
3. Add variables inside `:root`.
4. Use the variables with `var()`.
5. Open the page in a browser.

## Result
A simple design-token and typography system was created using CSS variables.
