[Home](https://pgmorales76.github.io/reading_notes/)

# Class 5 Reading Notes

## What is CSS for?

### CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc

### CSS can be used for very basic document text styling, it can be used to create a layout,it can even be used for effects such as animation

## CSS Syntax

### CSS is a rule-based language — you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page

### For example, you can decide to have the main heading on your page to be shown as large red text

    h1 {
        color: red;
        font-size: 5em;
        }

#### - In the above example, the CSS rule opens with a selector. This selects the HTML element that we are going to style. In this case, we are styling level one headings (`<h1>`)

#### - We then have a set of curly braces { }

#### - Inside the braces will be one or more declarations, which take the form of property and value pairs. We specify the property (color in the above example) before the colon, and we specify the value of the property after the colon (red in this example)

#### - This example contains two declarations, one for color and the other for font-size. Each pair specifies a property of the element(s) we are selecting (`<h1>` in this case), then a value that we'd like to give the property

### A CSS stylesheet will contain many such rules, written one after the other

    h1 {
        color: red;
        font-size: 5em;
        }

    p {
        color: black;
        }


[What is CSS?](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)



[How to add CSS](https://www.w3schools.com/css/css_howto.asp)

[CSS Color](https://www.w3schools.com/cssref/pr_text_color.asp)

[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

[Myers Web Reset Stylesheet](https://meyerweb.com/eric/tools/css/reset/)
