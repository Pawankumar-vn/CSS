```css
CSS BASICS AND TYPOGRAPHY

1. INTRODUCTION TO CSS

  • CSS stands for Cascading Style Sheets.  
    It is used to style HTML elements (e.g., colors, fonts, layouts).

  
2. HOW TO INCLUDE CSS IN HTML

  • Inline CSS: Add styles directly to an HTML element using the "style" attribute.  
    <p style="color: red; font-size: 16px;">This is inline CSS.</p>

  • Internal CSS: Add styles inside a <style> tag in the <head> section of HTML.  
    <style>  
        p {  
            color: blue;  
            font-size: 18px;  
        }  
    </style>

  • External CSS: Link an external .css file using the <link> tag in the <head> section.  
    <link rel="stylesheet" href="styles.css">


3. CSS SYNTAX AND SELECTORS

  • CSS syntax consists of a selector and a property value pair.  
    selector { property: value; }

  Types of Selectors:  
  • Universal selector: * { }  
  • Element selector: p { }  
  • Class selector: .class-name { }  
  • ID selector: #id-name { }

  
  • Element Selector:  
    Targets HTML elements by tag name.  

    h1 {  
        color: green;  
    }

  • Class Selector:  
    Targets elements with a specific class (use .classname).  

    .my-class {  
        font-size: 20px;  
    }

  • ID Selector:  
    Targets a single element with a specific ID (use #idname).  

    #my-id {  
        color: purple;  
    }

  
4. TYPOGRAPHY

  • Font Properties:  
    Used to set the font type, size, style, and weight.  

    p {  
        font-family: Arial, sans-serif;  
        font-size: 16px;  
        font-style: italic;  
        font-weight: bold;  
    }

  • Text Properties:  
    Controls text alignment, decoration, and transformation.  

    h2 {  
        text-align: center;  
        text-decoration: underline;  
        text-transform: uppercase;  
    }

  • Line Spacing:  
    Controls the space between lines of text.  

    p {  
        line-height: 1.5;  
    }

  • Letter and Word Spacing:  
    Adjusts the space between letters and words.  

    h3 {  
        letter-spacing: 2px;  
        word-spacing: 5px;  
    }


END OF NOTES



