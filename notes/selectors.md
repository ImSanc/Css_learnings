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
-> this has more specificity , even if we apply a css to all elements and have different class to one , it will override element selector

    .container {
    width: 80%;
    }

### ID Selector (#id) 
→ Selects a specific element with an ID (should be unique , HTML or css won't complain but should be unique for controls)

    #header {
    background-color: black;
    }

### Group selector
- where we select a group p and h1 with , in between

 p , h1 {
    color: blue;
    }


- Use of selectors in React projects:
    🔹 Final Best Practices in React
    ✅ Use id for:

        Anchor links (href="#section").
        Form labels (htmlFor="inputId").
        Interacting with external scripts.
        Rare global styles.

    ❌ Avoid id for:

        Styling (use className).
        Selecting elements (use useRef).
        Handling lists (key prop is better).
        Animations (use Framer Motion or CSS).