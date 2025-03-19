## Box-Sizing
- The box-sizing property in CSS controls how the total width and height of an element is calculated — especially whether padding and border are included in that calculation.

- Syntax:

         box-sizing: content-box | border-box | inherit;


- Values:
1. content-box (default):
- Width/height only include the content.
- Padding and border are added on top.

            box-sizing: content-box;

📦 Total size = width + padding + border

2. border-box:
 - Width/height include content + padding + border.

The content box shrinks to make room

        box-sizing: border-box;

📦 Total size = exactly width (includes padding & border)


Many developers apply this globally for easier layout control:

        * {
        box-sizing: border-box;
        }