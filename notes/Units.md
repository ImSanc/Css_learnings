# Units 
In CSS there are many units like cm ,pixels , mm , in etc/
- We more commonly only use <b>pixel (px) </b>

- We shouldn't hard code things which user can set on browsers default as well. eg: font sizes etc.



## Absolute Lengths
- The absolute length units are fixed and a length expressed in any of these will appear as exactly that size.

- Absolute length units are not recommended for use on screen, because screen sizes vary so much. However, they can be used if the output medium is known, such as for print layout.

* Pixels (px) are relative to the viewing device. For low-dpi devices, 1px is one device pixel (dot) of the display. For printers and high resolution screens 1px implies multiple device pixels.

Unit	        Description
cm	            centimeters
mm	            millimeters
in	            inches (1in = 96px = 2.54cm)
px *	        pixels (1px = 1/96th of 1in)
pt	            points (1pt = 1/72 of 1in)
pc	            picas (1pc = 12 pt)


## Relative Lengths
Relative length units specify a length relative to another length property. Relative length units scale better between different rendering medium.

Unit            	Description	
em	                Relative to the font-size of the element (2em means 2 times the size of the current font)	
ex	                Relative to the x-height of the current font (rarely used)	
ch	                Relative to the width of the "0" (zero)	( we can use it like if we want only 40 characters on a line etcs)
rem	                Relative to font-size of the root element	
vw	                Relative to 1% of the width of the viewport*	
vh	                Relative to 1% of the height of the viewport*	
vmin	            Relative to 1% of viewport's* smaller dimension	
vmax	            Relative to 1% of viewport's* larger dimension	
%	                Relative to the parent element


#### Difference Between % and Viewport Units (vw, vh)

1. Percentage (%)
 - % is relative to the parent element.
 - If the parent element has no defined size, the % value might not work as expected.

2. Viewport Units (vw, vh)
 - vw and vh are relative to the entire viewport (browser window), not the parent.
 - They always take a percentage of the viewport size, even if inside a smaller parent.


### Which One is More Used?
 - Use % when you want sizes relative to a parent container (e.g., for layouts inside a div).
 - Use vw/vh when you want sizes relative to the screen (e.g., full-page sections, fullscreen backgrounds).

### When to Use Which?
    Use Case	                                       Best Choice
    Responsive grids, divs inside a container	        %
    Full-screen sections, modals, hero banners	        vw, vh
    Text that scales with screen size	                vw
    Child elements inside a fixed-size parent       	%


#### Note : body is not always fully 100% it grows with the content. But there might be cases where we want the content to be 100 height
- We can use 


        body {
            min-height : 100vh;
        }