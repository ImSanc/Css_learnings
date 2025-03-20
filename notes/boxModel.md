# Box Model 
- In CSS, every HTML element is considered as a box. The box model describes how the size of these elements is calculated and how elements interact with each other.

        +---------------------------+
        |       Margin (outside)    |
        |  +---------------------+  |
        |  |   Border (edge)     |  |
        |  |  +---------------+  |  |
        |  |  | Padding        |  |  |
        |  |  | +-----------+  |  |  |
        |  |  | | Content   |  |  |  |
        |  |  | +-----------+  |  |  |
        |  |  +---------------+  |  |
        |  +---------------------+  |
        +---------------------------+

- Content – The actual text/image/element.

- Padding – Space between the content and border.

- Border – The visible edge around the element.

- Margin – Space outside the border, pushing the element away from others.


#### What is an Outline?
- The outline is similar to a border, but:
- It doesn’t take up space in the layout (doesn't affect element size).
- It is drawn outside the border.
- It's mostly used for accessibility (e.g., focus rings).

            outline: 2px solid red;

#### How to Round a Div?
Use the border-radius property:

            div {
                border-radius: 10px;
            }

More examples:
- border-radius: 50%; makes a perfect circle (if the div is square).
- border-radius: 0 10px 10px 0; gives rounded corners selectively (top-right, bottom-right in this case).