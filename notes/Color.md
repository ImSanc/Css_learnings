## Colors

- CSS offers several ways to specify colors. Here are the main color selection methods:

1. Color Names

    color: red;
    color: blue;
    color: mediumseagreen;

2. Hexadecimal Colors
- First 2 letters are for red , second 2 for green , 3rd 2 for blue

    color: #ff0000; /* red */
    color: #0000ff; /* blue */
    color: #3cb371; /* medium sea green */
    color: #f00;    /* shorthand for #ff0000 */


3. RGB Colors
- Max is 255 , (255,255,255) is black and (0,0,0) is white

    color: rgb(255, 0, 0);      /* red */
    color: rgb(0, 0, 255);      /* blue */
    color: rgb(60, 179, 113);   /* medium sea green */


4. RGBA Colors (RGB with alpha/transparency)
- here aplha is transparency ( it starts from 0 to 1 (where 0 is full transparent and 1 is opaque))


    color: rgba(255, 0, 0, 1);     /* solid red */
    color: rgba(0, 0, 255, 0.5);   /* 50% transparent blue */


5. HSL Colors (Hue, Saturation, Lightness)


        color: hsl(0, 100%, 50%);      /* red */
        color: hsl(240, 100%, 50%);    /* blue */
        color: hsl(147, 50%, 47%);     /* medium sea green */