```css
RESPONSIVE GRID

1. RESPONSIVE GRID

  • Auto-Fitting and Auto-Filling Columns

    .grid-responsive {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
        gap: 10px;
    }

  • Explanation:
    - auto-fit: Expands items to fill available space.
    - minmax(150px, 1fr): Ensures columns are at least 150px but can grow.

  • Media Queries for Responsive Grid

    @media (max-width: 768px) {
        .grid-container {
            grid-template-columns: 1fr;
        }
    }


2. ADDITIONAL GRID FEATURES

  • Grid Auto-Placement (Implicit Grid)

    .grid-auto {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-auto-rows: 100px;
    }

  • Aligning Items in Grid

    .grid-align {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        align-items: center;
        justify-items: center;
    }

  • Nested Grid (Grid Inside Grid)

    .nested-grid {
        display: grid;
        grid-template-columns: 2fr 1fr;
    }

    .inner-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
    }


END OF NOTES
```
