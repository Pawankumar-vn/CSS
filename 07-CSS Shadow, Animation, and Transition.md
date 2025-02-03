```css
SHADOW, ANIMATION, AND TRANSITION

1. SHADOWS IN CSS

TEXT SHADOW (Adds shadow to text)
 h1 {
 text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /_ (x-offset, y-offset, blur-radius, color) _/
 }

BOX SHADOW (Adds shadow to an element)
 .box {
 width: 200px;
 height: 100px;
 background-color: lightblue;
 box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.3); /_ (x-offset, y-offset, blur-radius, color) _/
 }

2. TRANSITIONS

• Transitions create smooth changes between CSS properties over time.
 • Syntax:
 transition: property duration timing-function delay;

EXAMPLE: Background color transition on hover
 .button {
 background-color: blue;
 color: white;
 padding: 10px 20px;
 transition: background-color 0.5s ease-in-out; /_ Smooth color change over 0.5s _/
 }

.button:hover {
 background-color: darkblue;
 }

TRANSITION PROPERTIES
 • transition: Shorthand for all transition properties.
 • transition-duration: Specifies how long the transition takes.
 • transition-timing-function: Defines the speed curve (ease, linear, ease-in-out, etc.).

MULTIPLE TRANSITIONS
 .box {
 width: 100px;
 height: 100px;
 background-color: red;
 transition: width 0.5s ease, height 0.5s ease;
 }

.box:hover {
 width: 150px;
 height: 150px;
 }

3. ANIMATIONS

• Animations allow continuous changes with keyframes.
 • Uses @keyframes to define animation steps.

KEYFRAMES: Defining animation sequence
 @keyframes bounce {
 0% { transform: translateY(0); }
 50% { transform: translateY(-20px); }
 100% { transform: translateY(0); }
 }

APPLYING ANIMATION
 .bouncing-box {
 width: 100px;
 height: 100px;
 background-color: green;
 animation: bounce 1s infinite;
 }

ANIMATION PROPERTIES
 • animation-name: Name of the keyframes animation.
 • animation-duration: How long the animation runs.
 • animation-iteration-count: Number of times the animation runs (or infinite).

EXAMPLE: Rotating animation
 @keyframes rotate {
 from { transform: rotate(0deg); }
 to { transform: rotate(360deg); }
 }

.rotating-box {
 width: 100px;
 height: 100px;
 background-color: orange;
 animation: rotate 2s linear infinite;
 }

EXTRA NOTES

• Use transitions for simple effects (hover, focus, etc.).
 • Use animations for continuous motion (spinners, loaders, etc.).
 • Prefer transform and opacity for smoother performance.

END OF NOTES
```
