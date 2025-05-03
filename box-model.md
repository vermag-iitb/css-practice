# Box Model in CSS
1. Blue box - content
2. Orange box - margin

## Diagram
![Alt text](../css-practice/resources/box-model.JPG)

### Terminology
1. Height: vertical length of content (in px)
2. Width: horizontal length of content (in px)
3. Border: line enclosing padding and content
4. Padding: space around content
5. Margin: space between boxes of two different contents

## CSS Attributes
#### Box attributes
1. height:
2. width:
3. border: 
    * shorthand for border-style, border-width, and border-color in single line.
        E.g.: 
        <p style="border:5px solid rgb(12,192,21);">
        <img src="../css-practice/resources/mobile.PNG" width="50px" height="50px" style="border:10px solid red;">
    1. border-style: how border will appear
        * types of border: 
            1. solid
            2. dotted
            3. outset/inset (3D shade)
            4. dashed
            5. ridge (3d type)`
    2. border-width: thickness of border
    3. border-color: color of border
4. background-color:rgb(x,y,z)
        - this is for inline
        - this property is for background color (what appears at the back, for text it appears as text highlighter)
    * E.g.: <h1 style="color:red; background-color=yellow;">...text...</h1>
5. box-shadow: 
    * to display shadow for HTML element
    * Syntax: 
        box-shadow: Xpx Ypx color;
            where XY are: ++ -+ -- +- (1, 2, 3, 4 quadrants)
        box-shadow: px1 px2 px3 px4 color;
            quad in clockwise dimension of shadow
    * E.g.,
        <p style="background-color:#cfbeab; box-shadow:3px 3px;"></p>
        <p style="background-color:#cfbeab; box-shadow:3px 3px; #ff0000"></p>
6. border-radius: 
    * to give curvature to box
    * it can be defined in px or %
    * Syntax: 
        border-radius: Npx;
            i.e., all corners similar curve
        border-radius: Mpx Npx;
            i.e., two diagonal corner pair
    * E.g.,
    <img src="../css-practice/resources/laptop.PNG" width="200px" height="150px" style="border-radius:150px 50px">
    * We can make circles using this attribute, when N=width/2
7. padding: 
    * to give space between border and content
    * Syntax: 
        padding: 1px, 2px, 3px, 4px; // applies different px to all sides (top, right, bottom, left)
        padding: 1px; // applies same px to all four sides
        padding-left: 1px; // applies same px to left side
        padding-right: 1px; // applies same px to right side
        padding-top: 1px; // applies same px to top side
        padding-bottom: 1px; // applies same px to bottom side
7. margin: 
    * to give space between two contents (and not border)
    * Syntax: 
        margin: 1px, 2px, 3px, 4px; // applies different px to all sides
        margin: 1px; // applies same px to all four sides
        margin-left: 1px; // applies same px to left side
        margin-right: 1px; // applies same px to right side
        margin-top: 1px; // applies same px to top side
        margin-bottom: 1px; // applies same px to bottom side

