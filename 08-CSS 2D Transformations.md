```css
2D TRANSFORMATIONS

1. INTRODUCTION TO 2D TRANSFORMATIONS

  • 2D transformations modify an element in two dimensions (X and Y axes).
    They can move, rotate, scale, or skew elements.


2. TYPES OF 2D TRANSFORMATIONS

  • Translate (Moves an element)

    .translate-box {
        width: 100px;
        height: 100px;
        background-color: lightblue;
        transform: translate(50px, 20px);
    }

  • Rotate (Rotates an element)

    .rotate-box {
        width: 100px;
        height: 100px;
        background-color: lightcoral;
        transform: rotate(45deg);
    }

  • Scale (Resizes an element)

    .scale-box {
        width: 100px;
        height: 100px;
        background-color: lightgreen;
        transform: scale(1.5);
    }

  • Scale X & Scale Y (Resizes width or height independently)

    .scale-x-box {
        width: 100px;
        height: 100px;
        background-color: lightskyblue;
        transform: scaleX(2);
    }

    .scale-y-box {
        width: 100px;
        height: 100px;
        background-color: lightgoldenrodyellow;
        transform: scaleY(0.5);
    }

  • Skew (Tilts an element)

    .skew-box {
        width: 100px;
        height: 100px;
        background-color: lightsalmon;
        transform: skew(20deg, 10deg);
    }


3. COMBINING MULTIPLE TRANSFORMATIONS

  • Multiple transformations can be applied at once.
    Order matters (e.g., rotate before scale may have a different effect).

    .combined-transform {
        width: 100px;
        height: 100px;
        background-color: deepskyblue;
        transform: translate(50px, 20px) rotate(30deg) scale(1.2);
    }


4. EXTRA NOTES

  • Use transform-origin to change the transformation point.
    Example: transform-origin: top left;

  • Applying transitions makes transformations smooth.
    Example: transition: transform 0.5s ease-in-out;


END OF NOTES
```
