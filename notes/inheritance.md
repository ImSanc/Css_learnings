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

eg: 
    * {
        border: 1px solid red;
    }

This will apply this to every element in the DOM tree