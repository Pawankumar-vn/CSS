/_ * CSS BASICS AND TYPOGRAPHY * _/

/\* 1. INTRODUCTION TO CSS

- CSS stands for Cascading Style Sheets.
- It is used to style HTML elements (e.g., colors, fonts, layouts).
  \*/

/_ 2. HOW TO INCLUDE CSS IN HTML _/

/_ - Inline CSS: Add styles directly to an HTML element using the "style" attribute. _/

<p style="color: red; font-size: 16px;">This is inline CSS.</p>

/_ - Internal CSS: Add styles inside a <style> tag in the <head> section of HTML. _/

<style>
    p {
        color: blue;      /* Sets the text color to blue */
        font-size: 18px;  /* Sets the font size to 18px */
    }
</style>

/_ - External CSS: Link an external .css file using the <link> tag in the <head> section. _/

<link rel="stylesheet" href="styles.css">

/_ 3. CSS SYNTAX AND SELECTORS _/

/_ - Syntax: selector { property: value; } _/

/_ - Element Selector: Targets HTML elements by tag name. _/
h1 {
color: green; /_ Sets the color of <h1> text to green _/
}

/_ Types of Selectors: _/
/_ 1. Universal selector: _ { } _/
/_ 2. Element selector: p { } _/
/_ 3. Class selector: .class-name { } _/
/_ 4. ID selector: #id-name { } \*/

/_ - Class Selector: Targets elements with a specific class (use .classname). _/
.my-class {
font-size: 20px; /_ Sets font size to 20px for elements with class "my-class" _/
}

/_ - ID Selector: Targets a single element with a specific ID (use #idname). _/
#my-id {
color: purple; /_ Sets the color of element with ID "my-id" to purple _/
}

/_ 4. TYPOGRAPHY _/

/_ - Font Properties _/
p {
font-family: Arial, sans-serif; /_ Sets the font family to Arial or sans-serif _/
font-size: 16px; /_ Sets the font size to 16px _/
font-style: italic; /_ Makes the text italic _/
font-weight: bold; /_ Makes the text bold _/
}

/_ - Text Properties _/
h2 {
text-align: center; /_ Aligns the text to the center _/
text-decoration: underline; /_ Underlines the text _/
text-transform: uppercase; /_ Converts the text to uppercase _/
}

/_ - Line Spacing _/
p {
line-height: 1.5; /_ Sets the space between lines (1.5 times the font size) _/
}

/_ - Letter and Word Spacing _/
h3 {
letter-spacing: 2px; /_ Adds 2px space between letters _/
word-spacing: 5px; /_ Adds 5px space between words _/
}

/_ END OF NOTES _/
