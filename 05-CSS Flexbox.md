```css
FLEXBOX BASICS

1. INTRODUCTION TO FLEXBOX

• Flexbox is a layout model that makes it easy to align and distribute elements inside a container.
 • It provides control over spacing, alignment, and resizing of elements.
 • To use Flexbox, set "display: flex" on the parent container.

2. PARENT PROPERTIES

• display: flex
 Enables flexbox on a container.

    .flex-container {
        display: flex;
        background-color: lightgray;
        padding: 10px;
    }

• flex-direction
 Defines the direction of flex items.

    • row (default): Items are placed in a row (left to right).
    • row-reverse: Items are placed in a row (right to left).
    • column: Items are placed in a column (top to bottom).
    • column-reverse: Items are placed in a column (bottom to top).

    .flex-container-row {
        flex-direction: row;
    }

    .flex-container-column {
        flex-direction: column;
    }

• justify-content
 Aligns items along the main axis.

    • flex-start (default): Items start from the beginning.
    • flex-end: Items align at the end.
    • center: Items align at the center.
    • space-between: Items spread out with space between them.
    • space-around: Items have equal space around them.
    • space-evenly: Items have equal space between and around them.

    .flex-container {
        justify-content: center;
    }

• align-items
 Aligns items along the cross axis (vertically if row, horizontally if column).

    • flex-start: Items align at the start of the cross axis.
    • flex-end: Items align at the end of the cross axis.
    • center: Items align at the center of the cross axis.
    • stretch (default): Items stretch to fill the container.
    • baseline: Items align based on their text baseline.

    .flex-container {
        align-items: center;
    }

• align-content
 Aligns multiple flex lines when there is extra space (only applies when flex-wrap is used).

    • flex-start, flex-end, center, space-between, space-around, space-evenly work similarly to justify-content.

    .flex-container {
        flex-wrap: wrap;
        align-content: space-between;
    }

• EXAMPLE:

    <div class="flex-container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>

3. CHILD PROPERTIES

• flex
 Specifies how much a flex item should grow/shrink.

    • flex: 1; (Item takes equal space)
    • flex: 2; (Item takes twice the space of flex: 1)

    .flex-item {
        flex: 1;
    }

• align-self
 Aligns an individual item differently from align-items of the parent.

    • Values: auto, flex-start, flex-end, center, stretch, baseline

    .flex-item {
        align-self: flex-end;
    }

• order
 Controls the order of flex items.

    • Default is 0, higher numbers appear later.

    .flex-item {
        order: 2;
    }

EXTRA NOTES

• "display: flex" makes a container a flex container.
 • "flex-direction" decides the main axis (row or column).
 • "justify-content" controls horizontal alignment.
 • "align-items" controls vertical alignment.
 • "flex" is the most powerful child property for flexible sizing.
 • "order" can rearrange elements without changing the HTML.

END OF NOTES
```
