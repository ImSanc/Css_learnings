# Elements 
In CSS, elements can be categorized into different types based on their behavior and usage. Here are the main types:

###  Block Elements
- These elements take up the full width of their parent container and start on a new line.
Example : div, p, h1-h6, section, article, aside, header, footer, nav, main

### Inline Elements
- These elements only take up as much width as needed and do not start on a new line.
Example : span, a, strong, em, b, i, img, label, small

### Inline-Block Elements
- These elements behave like inline elements but allow setting width and height like block elements.
Example : input, button, img, select, textarea

### Flex Elements
Used within a flex container (display: flex;) to create flexible layouts.


        Parent container:
        display: flex;


Child items follow flex properties like flex-grow, flex-shrink, and align-self.

### Grid Elements
- Used within a grid container (display: grid;) for advanced layouts.


        Parent container:
        display: grid;


- Child items follow grid properties like grid-column, grid-row, and align-self.

### Floating Elements
Elements that use float: left; or float: right; to move within the layout.
Example:

            img {
            float: left;
            }


###  Positioned Elements
These elements are controlled using the position property.

Types:
- static (default)
- relative
- absolute
- fixed
- sticky

### Pseudo-Elements
These are virtual elements used to style parts of an element.

Examples:

        p::first-letter { font-size: 2em; }
        a::before { content: "🔗 "; }


###  Form Elements
Special elements used in forms.

Examples:
input, textarea, select, button, label, option, fieldset

