```css
CSS GRID

1. CSS GRID BASICS

  • CSS Grid is a two-dimensional layout system.
  • It allows precise control over rows and columns.

  • Defining a Grid Container

    .grid-container {
        display: grid;
        grid-template-columns: 200px 200px 200px;
        grid-template-rows: 100px 100px;
        gap: 10px;
        background-color: lightgray;
    }

  • Grid Items

    .grid-item {
        background-color: steelblue;
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 18px;
    }

  • Auto-Sizing Columns with Fractions

    .grid-container-fr {
        display: grid;
        grid-template-columns: 1fr 2fr 1fr;
    }


2. GRID LINES, TRACKS, AND AREAS

  • Grid Lines (Explicit Row and Column Positioning)

    .grid-container-lines {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(2, 100px);
    }

    .grid-item-1 {
        grid-column: 1 / 3;
        grid-row: 1 / 2;
    }

  • Grid Areas (Named Layouts)

    .grid-container-areas {
        display: grid;
        grid-template-areas:
            "header header"
            "sidebar main"
            "footer footer";
        grid-template-columns: 1fr 2fr;
        grid-template-rows: 50px auto 50px;
    }

    .header {
        grid-area: header;
        background-color: navy;
    }

    .sidebar {
        grid-area: sidebar;
        background-color: darkslategray;
    }

    .main {
        grid-area: main;
        background-color: darkgreen;
    }

    .footer {
        grid-area: footer;
        background-color: darkred;
    }


END OF NOTES
```
