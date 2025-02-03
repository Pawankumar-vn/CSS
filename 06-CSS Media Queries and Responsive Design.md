```css
MEDIA QUERIES AND RESPONSIVE DESIGN

1. INTRODUCTION TO MEDIA QUERIES

• Media queries allow us to apply CSS rules based on screen size, resolution, or device type.
 • It helps in making websites responsive by adjusting styles for different devices.

Syntax:
 @media (condition) {
 CSS rules here...
 }

2. BREAKPOINTS FOR RESPONSIVENESS

• Breakpoints define the screen width where styles should change.
 • Common breakpoints:
 • Mobile: max-width: 600px
 • Tablet: min-width: 601px and max-width: 1024px
 • Desktop: min-width: 1025px

MOBILE STYLES (for screens up to 600px wide)
 @media (max-width: 600px) {
 body {
 background-color: lightblue; /_ Example of changing background for mobile _/
 }

      .container {
          flex-direction: column; /* Stack items in a column */
          padding: 10px;
      }

}

TABLET STYLES (for screens between 601px and 1024px)
 @media (min-width: 601px) and (max-width: 1024px) {
 body {
 background-color: lightgreen; /_ Example of changing background for tablets _/
 }

      .container {
          flex-direction: row; /* Items are in a row */
          justify-content: space-between;
      }

}

DESKTOP STYLES (for screens 1025px and above)
 @media (min-width: 1025px) {
 body {
 background-color: white; /_ Default background for desktops _/
 }

      .container {
          max-width: 1200px;
          margin: auto;
      }

}

3. USING MEDIA QUERIES TO MAKE A SIMPLE LAYOUT RESPONSIVE

Example of a responsive navigation bar:
 .navbar {
 display: flex;
 justify-content: space-between;
 padding: 20px;
 }

MOBILE VIEW: Stack menu items vertically
 @media (max-width: 600px) {
 .navbar {
 flex-direction: column;
 text-align: center;
 }
 }

EXTRA: Hide an element on small screens
 @media (max-width: 500px) {
 .desktop-only {
 display: none; /_ Hides element on screens smaller than 500px _/
 }
 }

EXTRA NOTES

• "max-width" applies styles when the screen is smaller than the given width.
 • "min-width" applies styles when the screen is larger than the given width.
 • Combining min-width and max-width targets specific screen ranges.
 • Always test media queries on real devices or browser dev tools for accuracy.

END OF NOTES
```
