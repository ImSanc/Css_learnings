# What is CSS?
Cascading Style Sheets (CSS) is used to format the layout of a webpage.

With CSS, you can control the color, font, the size of text, the spacing between elements, how elements are positioned and laid out, what background images or background colors are to be used, different displays for different devices and screen sizes, and much more!


####  There are 3 ways of adding css to your HTML :

- Inline - by using the style attribute inside HTML elements
- Internal - by using a <style> element in the <head> section
- External - by using a <link> element to link to an external CSS file

## Inline CSS
- An inline CSS is used to apply a unique style to a single HTML element.

- An inline CSS uses the style attribute of an HTML element.

- The following example

Example

    <h1 style="color:blue;">A Blue Heading</h1>
    <p style="color:red;">A red paragraph.</p>


## Internal CSS
- An internal CSS is used to define a style for a single HTML page.

- An internal CSS is defined in the <head> section of an HTML page, within a <style> element.

- The following example 

Example

        <!DOCTYPE html>
            <html>
                <head>
                <style>
                    body {background-color: powderblue;}
                    h1   {color: blue;}
                    p    {color: red;}
                </style>
                </head>
                <body>

                    <h1>This is a heading</h1>
                    <p>This is a paragraph.</p>

                </body>
            </html>



## External CSS
- An external style sheet is used to define the style for many HTML pages.
- To use an external style sheet, add a link to it in the <head> section of each HTML page:

Example

    <!DOCTYPE html>
        <html>
            <head>
                <link rel="stylesheet" href="styles.css">
            </head>
        <body>

            <h1>This is a heading</h1>
            <p>This is a paragraph.</p>

        </body>
        </html>

