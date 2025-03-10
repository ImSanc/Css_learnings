## Inheritance in CSS Properties
- In CSS, some properties are inherited by default, while others are not. This concept helps maintain consistent styling across child elements without explicitly defining properties for each element.

✅ Inherited Properties (Text-Related)
Some properties naturally inherit values from their parent element:

- color
- font (including font-size, font-family, font-style, font-weight)
- letter-spacing
- line-height
- visibility
- direction
- cursor


❌ Non-Inherited Properties (Box Model & Layout)
Most properties do NOT inherit because inheritance would break layouts:

- margin, padding, border
- width, height, max-width, max-height
- display, position, z-index
- background, box-shadow
- overflow, clip-path
- grid, flex, align-items, justify-content


### Setting something use all selector is not inheritance


## Universal selector
eg: 
    * {
        border: 1px solid red;
    }

This will apply this to every element in the DOM tree.

But if we want things to be inhertied then we can do is:
eg:
button , input, textarea, select {
    font : inherit;
} 

- We can use HTML selector for the default case : 
html {
}

we can either use body or html , but can use html if we want want to have some other settings then html.


### Other selector is main selector
In CSS, the main selector targets the <main> HTML element. The <main> element is a semantic tag introduced in HTML5 that represents the main content of a document. It should contain content that is unique to the page and not repeated across multiple pages, such as headers, footers, or navigation menus.


    <main>
    <h1>Welcome to My Website</h1>
    <p>This is the main content of the page.</p>
    </main>

we can apply this to the main selector : 

    main {
    background-color: #f4f4f4;
    padding: 20px;
    font-size: 18px;
    }


### Ranking of selectors
- Inline styles → 1000

- ID selectors (#id) → 100

- Class, Attribute, and Pseudo-class selectors (.class, [attr], :hover) → 10

- Element and Pseudo-element selectors (div, h1, ::before) → 1

- Universal selector (*) → 0 (No specificity)

🚀 <b>!important</b> overrides all but follows specificity rules when multiple !important styles exist.
it gives 

### !Important 
The !important declaration in CSS is used to override all other style rules, regardless of specificity. When a rule has !important, it takes priority over conflicting styles—even those with higher specificity.

    p {
    color: blue !important;
    }

    p {
    color: red;
    }
    
🔹 The paragraph will be blue because !important overrides the second rule.