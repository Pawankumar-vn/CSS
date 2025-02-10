```css

 SASS CSS

  • Variables in SASS

    $primary-color: #3498db;
    $secondary-color: #2ecc71;
    $font-size: 16px;

    body {
        background-color: $primary-color;
        color: white;
        font-size: $font-size;
    }

  • Nesting in SASS

    .container {
        width: 100%;

        .header {
            background: $secondary-color;

            h1 {
                color: white;
            }
        }
    }


1. ADVANCED SASS FEATURES

  • Partials & Imports

    // _variables.scss
    $main-bg: #333;

    // style.scss
    @use 'variables';

    body {
        background: variables.$main-bg;
    }

  • Mixins (Reusable Code)

    @mixin flex-center {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .box {
        @include flex-center;
        width: 100px;
        height: 100px;
        background: red;
    }

  • Mixins with Parameters

    @mixin button-style($bg-color, $text-color) {
        background: $bg-color;
        color: $text-color;
        padding: 10px 20px;
    }

    .button {
        @include button-style(blue, white);
    }


2. ADDITIONAL SASS FUNCTIONALITIES

  • Extend / Inheritance

    %base-style {
        font-family: Arial, sans-serif;
        padding: 10px;
    }

    .card {
        @extend %base-style;
        background: lightgray;
    }

  • Functions in SASS

    @function calculate-rem($size) {
        @return $size / 16px * 1rem;
    }

    .text {
        font-size: calculate-rem(24px);
    }

  • Conditionals & Loops

    @for $i from 1 through 5 {
        .box-#{$i} {
            width: $i * 50px;
            height: $i * 50px;
        }
    }

    $theme: dark;

    body {
        @if $theme == dark {
            background: black;
            color: white;
        } @else {
            background: white;
            color: black;
        }
    }


3. RESPONSIVE DESIGN IN SASS

  • Mixin for Responsive Design

    @mixin responsive($size) {
        @media (max-width: $size) {
            @content;
        }
    }

    .container {
        width: 80%;

        @include responsive(768px) {
            width: 100%;
        }
    }


4. COMPILING SASS TO CSS

  • Install SASS

    npm install -g sass

  • Compile SASS

    sass style.scss style.css

  • Auto-Compile

    sass --watch style.scss:style.css


END OF NOTES
```
