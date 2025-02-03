```css
THE BOX MODEL

1. UNDERSTANDING THE BOX MODEL

• Every HTML element is a rectangular box consisting of four layers.

• Content:
 The actual content inside the element (text, images, etc.).

• Padding:
 Space between content and border (inside the box).

• Border:
 Surrounds the padding and content.

• Margin:
 Space between this element and other elements.

• Visual Representation of Box Model:

    | Margin (outside space)
    | Border (visible edge of the element)
    | Padding (inner spacing inside the border)
    | Content (text, image, etc.)

• Box Model:

    .box {
        width: 200px;
        height: 100px;
        padding: 20px;
        border: 5px solid black;
        margin: 30px;
    }

2. BORDER STYLES AND BORDER RADIUS

• Borders can have different styles, colors, and widths.

• Common border styles:
 solid, dashed, dotted, double, groove, ridge, inset, outset, none.

    .border-example {
        border: 3px dashed blue;
    }

• Border Radius:
 Rounds the corners of an element.

    .rounded-box {
        border: 2px solid black;
        border-radius: 15px;
    }

• Fully Rounded (Perfect Circle):
 Makes a perfect circle by setting border-radius to 50%.

    .circle {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        background-color: red;
    }

3. BOX-SIZING: CONTENT-BOX VS. BORDER-BOX

• The box-sizing property controls how the total width & height are calculated.

• Default Behavior: content-box
 Width & height apply only to content (padding and border are extra).

    .content-box-example {
        width: 200px;
        height: 100px;
        padding: 20px;
        border: 5px solid black;
        box-sizing: content-box;
    }

• Alternative: border-box
 Width & height include content, padding, and border (keeps box size fixed).

    .border-box-example {
        width: 200px;
        height: 100px;
        padding: 20px;
        border: 5px solid black;
        box-sizing: border-box;
    }

• Best practice:
 Apply border-box globally to avoid layout issues.

    * {
        box-sizing: border-box;
    }

4. OVERFLOW PROPERTIES

• Overflow controls how content behaves when it exceeds the container’s size.

• Possible values:
 visible, hidden, scroll, auto.

• visible (default):
 Content overflows outside the box.

    .overflow-visible {
        width: 150px;
        height: 50px;
        border: 1px solid black;
        overflow: visible;
    }

• hidden:
 Hides overflowing content (no scroll).

    .overflow-hidden {
        width: 150px;
        height: 50px;
        border: 1px solid black;
        overflow: hidden;
    }

• scroll:
 Always shows scrollbars (even if not needed).

    .overflow-scroll {
        width: 150px;
        height: 50px;
        border: 1px solid black;
        overflow: scroll;
    }

• auto:
 Shows scrollbars only when needed.

    .overflow-auto {
        width: 150px;
        height: 50px;
        border: 1px solid black;
        overflow: auto;
    }

EXTRA NOTES

• Padding and margin can be set individually:
 padding-top, padding-right, padding-bottom, padding-left
 margin-top, margin-right, margin-bottom, margin-left

• Shorthand:
 Padding and margin can be written in 1-4 values.

    padding: 10px 20px 30px 40px;

• 1 value = All sides same.
 • 2 values = Vertical | Horizontal.
 • 3 values = Top | Horizontal | Bottom.
 • 4 values = Top | Right | Bottom | Left.

END OF NOTES
```
