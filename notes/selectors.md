# Selector
- CSS has several types of selectors that help target HTML elements effectively. Here’s a breakdown of the main types:

### Basic Selectors
These are the most common and simple selectors.

##### Universal Selector (*) 
→ Selects all elements

        * {
        margin: 0;
        padding: 0;
        }

### Type Selector (element)

→ Selects all elements of a specific type

    p {
    color: blue;
    }


### Class Selector (.class) 
→ Selects elements with a specific class

    .container {
    width: 80%;
    }

### ID Selector (#id) 
→ Selects a specific element with an ID (should be unique , HTML or css won't complain but should be unique for controls)

    #header {
    background-color: black;
    }