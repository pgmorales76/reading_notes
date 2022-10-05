[Home](https://pgmorales76.github.io/reading_notes/)

# Class 4 Reading Notes

## Wireframe and Design

### What is a wireframe?

#### - Wireframing is a practice used by designers which allow them to define and plan the information hierarchy of their design for a website, app, or product

#### - Wireframing is also a great way of getting to know how a user interacts with your interface, through the positioning of buttons and menus on the diagrams

#### - A commonly-used argument for wireframing is that if a user doesn’t know where to go on a plain hand-drawn diagram of your site page, then it is irrelevant what colors or fancy text eventually get used

### Wireframe Examples

#### - Wireframes drawn with paper and pencil have the advantage of being very easy to change

#### - Switching later to software allows you to keep track of more detailed decisions

#### Wireframes from CareerFoundry student Samuel Adaramola

![Wireframe Examples](/images/wireframe_examples.png)

### Things to consider before you start wireframing

#### - The decision to use online tools, or to wireframe by hand, and the process used to get to from wireframe to code, is related to what approach the particular situation requires

### Six steps to make a wireframe

#### 1. Do your research

#### 2. Prepare your research for quick reference

#### 3. Make sure you have your user flow mapped out

#### 4. Draft, don’t draw. Sketch, don’t illustrate

#### 5. Add some detail and get testing

#### 6. Start turning your wireframes into prototypes

### How to make your wireframe good

#### - Clarity

#### - Confidence

#### - Simplicity is key

[How To Create Wireframes For A Website](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)

## Mozilla HTML Basics

### So, what is HTML?

#### - HTML (HyperText Markup Language) is a *markup language* that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way

### Anatomy of an HTML element

#### Below is the anatomy of a paragraph element

![Paragraph element](/images/anatomy_of_an_element.png)

#### Elements can also have attributes that look like the following

![Paragraph element with attribute](/images/html_attribute_anatomy.png)

### Anatomy of an HTML document

    <!DOCTYPE html>
    <html lang="en-US">
        <head>
            <meta charset="utf-8" />
            <meta name="viewport" content="width=device-width" />
            <title>My test page</title>
        </head>
            <body>
                <img src="images/firefox-icon.png" alt="My test image" />
            </body>
    </html>

### Images

#### The image element embeds an image into our page in the position it appears. It does this via the src (source) attribute, which contains the path to our image file. Also included is an alt (alternative) attribute. In the alt attribute, you specify descriptive text for users who cannot see the image

`<img src="images/firefox-icon.png" alt="My test image" />`

## Marking up text

### Headings

#### Heading elements allow you to specify that certain parts of your content are headings — or subheadings. HTML contains 6 heading levels, <h1> - <h6>, although you'll commonly only use 3 to 4 at most

    <!-- 4 heading levels: -->
    <h1>My main title</h1>
    <h2>My top level heading</h2>
    <h3>My subheading</h3>
    <h4>My sub-subheading</h4>

### Paragraphs

#### `<p>` elements are for containing paragraphs of text; you'll use these frequently when marking up regular text content

`<p>This is a single paragraph</p>`

### Lists

#### A lot of the web's content is lists and HTML has special elements for these. Marking up lists always consists of at least 2 elements. The most common list types are ordered (order of the items does matter, such as a recipe) and unordered (order of the items doesn't matter) lists

#### Here is an example of an unordered list

    <p>At Mozilla, we're a global community of</p>
        <ul>
            <li>technologists</li>
            <li>thinkers</li>
            <li>builders</li>
        </ul>
    <p>working together…</p>

## Links

#### Links are very important — they are what makes the web a web! To add a link, we need to use a simple element — `<a>` — "a" being the short form for "anchor". To make text within your paragraph into a link, follow these steps

#### 1. Choose some text

#### 2. Wrap the text in an `<a>` element, as shown below:

`<a>Mozilla Manifesto</a>`

#### 3. Give the `<a>` element an href attribute, as shown below

`<a href="">Mozilla Manifesto</a>`

#### 4. Fill in the value of this attribute with the web address that you want the link to

`<a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>`

[Mozilla HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)

## Semantics

### -

[Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

[Mozilla HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)

[Mozilla HTML Elements Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
