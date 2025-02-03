```css
DISPLAY, INLINE-BLOCK, AND POSITIONING

1. DISPLAY PROPERTIES

• The display property controls how an element behaves in the document layout.

• block:
 Takes full width, starts on a new line (default for div, p, h1, etc.).

    .block-example {
        display: block;
        width: 200px;
        height: 50px;
        background-color: lightblue;
    }

• inline:
 Takes only as much width as needed, stays in the same line (default for span, a, etc.).

    .inline-example {
        display: inline;
        background-color: yellow;
        padding: 5px;
    }

• inline-block:
 Like inline, but allows setting width & height.

    .inline-block-example {
        display: inline-block;
        width: 150px;
        height: 50px;
        background-color: lightgreen;
        padding: 10px;
    }

• none:
 Completely removes the element from the page (no space taken).

    .none-example {
        display: none;
    }

• EXAMPLES:

    <div class="block-example">Block Element</div>
    <span class="inline-example">Inline Element</span>
    <div class="inline-block-example">Inline-Block Element</div>
    <div class="none-example">This won't be visible</div>

2. POSITIONING

• The position property controls how elements are placed in the document.
 • Values: static, relative, absolute, fixed, sticky.

• static (default):
 Elements follow normal document flow (no special positioning).

    .static-example {
        position: static;
    }

• relative:
 Moves element relative to its normal position (without affecting others).

    .relative-example {
        position: relative;
        top: 20px;
        left: 10px;
        background-color: lightcoral;
    }

• absolute:
 Removes element from normal flow, positions it relative to nearest positioned ancestor (or <html> if none).

    .absolute-example {
        position: absolute;
        top: 50px;
        left: 30px;
        background-color: lightgoldenrodyellow;
    }

• fixed:
 Stays fixed at a position relative to the viewport (doesn’t move when scrolling).

    .fixed-example {
        position: fixed;
        bottom: 10px;
        right: 10px;
        background-color: lightskyblue;
        padding: 10px;
    }

• sticky:
 Behaves like relative but becomes fixed when scrolling past a certain point.

    .sticky-example {
        position: sticky;
        top: 0px;
        background-color: lightpink;
        padding: 5px;
    }

• EXAMPLES:

    <div class="relative-example">Relative Position</div>
    <div class="absolute-example">Absolute Position</div>
    <div class="fixed-example">Fixed Position</div>
    <div class="sticky-example">Sticky Position</div>

3. Z-INDEX AND STACKING CONTEXT

• z-index controls the layering of elements (higher values appear on top).
 • Works only on positioned elements (relative, absolute, fixed).

.box1 {
 position: absolute;
 top: 50px;
 left: 50px;
 width: 100px;
 height: 100px;
 background-color: red;
 z-index: 1;
 }

.box2 {
 position: absolute;
 top: 70px;
 left: 70px;
 width: 100px;
 height: 100px;
 background-color: blue;
 z-index: 2;
 }

• If two elements have the same z-index, the one that comes later in the HTML appears on top.

EXTRA NOTES

• Positioning and display properties are crucial for page layouts.
 • "position: absolute" removes an element from the normal document flow.
 • "position: fixed" is useful for navigation bars or floating buttons.
 • "position: sticky" is great for headers that stay visible while scrolling.
 • z-index works only when an element has a position other than static.

END OF NOTES
```
