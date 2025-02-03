```css
COLORS, FONTS, AND SIZE UNITS

1. COLORS IN CSS

  • CSS allows defining colors using different formats.

  • Named Colors:
    Predefined color names like red, blue, green, etc.

    p {
        color: red;
    }

  • Hexadecimal Colors:
    Uses #RRGGBB format (00 to FF for each color).

    h1 {
        color: #ff5733;
    }

  • RGB Colors:
    Uses rgb(red, green, blue) where values range from 0 to 255.

    h2 {
        color: rgb(0, 128, 255);
    }

  • HSL Colors:
    Uses hsl(hue, saturation, lightness).

    h3 {
        color: hsl(200, 80%, 50%);
    }

  • Background Color:
    Changes the background of an element.

    body {
        background-color: #f0f0f0;
    }

  • Text Color:
    Changes the color of text content.

    p {
        color: #333;
    }

  • Transparency with RGBA & HSLA:
    Used for adding transparency to colors.

    div {
        background-color: rgba(255, 0, 0, 0.5);
        color: hsla(120, 100%, 25%, 0.7);
    }


2. FONTS IN DEPTH

  • Google Fonts Integration:
    Import and use custom fonts.
    Visit https://fonts.google.com to get font links.

    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

    body {
        font-family: 'Poppins', sans-serif;
    }

  • Custom Web Fonts using @font-face:
    This method allows using custom fonts stored locally or online.

    @font-face {
        font-family: 'MyCustomFont';
        src: url('fonts/MyCustomFont.woff2') format('woff2'),
             url('fonts/MyCustomFont.woff') format('woff');
    }

    h1 {
        font-family: 'MyCustomFont', sans-serif;
    }


3. SIZE UNITS

  • Absolute Units:
    Fixed sizes that do not change based on screen size.

  • px (pixels):
    Most common unit for web design.

    h1 {
        font-size: 24px;
    }

  • cm (centimeters), mm (millimeters):
    Rarely used for web.

    p {
        width: 5cm;
    }

  • Relative Units:
    Adjust based on parent or viewport size.

  • em:
    Relative to the parent element's font size.

    .parent {
        font-size: 16px;
    }
    .child {
        font-size: 2em;
    }

  • rem:
    Relative to the root element (<html>) font size.

    html {
        font-size: 16px;
    }
    h2 {
        font-size: 1.5rem;
    }

  • %:
    Relative to the parent element's size.

    div {
        width: 50%;
    }

  • vh (viewport height):
    Percentage of the viewport's height.

    section {
        height: 100vh;
    }

  • vw (viewport width):
    Percentage of the viewport's width.

    section {
        width: 100vw;
    }

END OF NOTES
```
