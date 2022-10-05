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

## How to add CSS

### Three Ways to add CSS

#### 1. External CSS

#### With an external style sheet, you can change the look of an entire website by changing just one file

#### Each HTML page must include a reference to the external style sheet file inside the `<link>` element, inside the head section

    <!DOCTYPE html>
    <html>
    <head>
    <link rel="stylesheet" href="mystyle.css">
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>

#### An external style sheet can be written in any text editor, and must be saved with a .css extension

#### The external .css file should not contain any HTML tags

#### Here is how the "mystyle.css" file looks

    body {
        background-color: lightblue;
        }

    h1 {
        color: navy;
        margin-left: 20px;
        }

#### 2. Internal CSS

#### An internal style sheet may be used if one single HTML page has a unique style

#### The internal style is defined inside the `<style>` element, inside the head section

    <!DOCTYPE html>
    <html>
    <head>
    <style>
    body {
        background-color: linen;
        }

    h1 {
        color: maroon;
        margin-left: 40px;
        }
    </style>
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>

#### 3. Inline CSS

#### An inline style may be used to apply a unique style for a single element

#### To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property

    <!DOCTYPE html>
    <html>
    <body>

    <h1 style="color:blue;text-align:center;">This is a heading</h1>
    <p style="color:red;">This is a paragraph.</p>

    </body>
    </html>

### Multiple Style Sheets

#### If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used

#### If the internal style is defined **after** the link to the external style sheet, the `<h1>` elements will be will styled according to the internal style sheet

    <head>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
    <style>
    h1 {
        color: orange;
        }
    </style>
    </head>

#### However, if the internal style is defined **before** the link to the external style sheet, the `<h1>` elements will be styled according to the external style sheet

    <head>
    <style>
    h1 {
        color: orange;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
    </head>

### Cascading Order

#### What style will be used when there is more than one style specified for an HTML element?

#### All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority

#### 1. Inline style (inside an HTML element)

#### 2. External and internal style sheets (in the head section)

#### 3. Browser default

#### So, an inline style has the highest priority, and will override external and internal styles and browser defaults

[How to add CSS](https://www.w3schools.com/css/css_howto.asp)

## CSS Color Property

### Definition and Usage

#### The color property specifies the color of text

#### Tip: Use a background color combined with a text color that makes the text easy to read

### Text-color property for different elements

    body {
        color: red;
        }

    h1 {
        color: #00ff00;
        }

    p.ex {
        color: rgb(0,0,255);
        }

[CSS Color](https://www.w3schools.com/cssref/pr_text_color.asp)

[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

[Myers Web Reset Stylesheet](https://meyerweb.com/eric/tools/css/reset/)
