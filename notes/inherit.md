# Inherit
- The inherit keyword makes a CSS property explicitly inherit its value from its parent element.

        child {
        color: inherit;
        }

- This means the child element will use the same color as its parent, even if that property doesn’t normally inherit by default.

🔍 What normally gets inherited in CSS?
- Some properties automatically inherit, like:

- color
- font-family
- line-height
- visibility

But many do not inherit by default, like:

- margin
- padding  
- border
- background

That’s where inherit becomes useful — to force inheritance for properties that don't do it on their own.


🛑 Limitations of inherit
- It only inherits from the direct parent — not grandparents or other ancestors.
- If the parent doesn’t have a set value for that property, the browser uses the initial value (default).
- Doesn’t work well in isolation — can be unpredictable if you're not sure what the parent value is.
- Doesn't always make sense — for example, inheriting margin or position might break layout.

✅ When to use inherit
- To maintain consistent styling (e.g., forcing a button inside a div to inherit font styles).
- When customizing components that override default behavior.
- For theming systems (inherit a variable-based color or spacing rule).

