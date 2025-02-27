# CSS (Cascading Styling Sheet)
## Introduction
Purpose: used for webpage make-up
Application: There are 3 types in which we apply CSS styles:
1. inline: i.e., HTML tags with CSS attributes
    * <tag style="attribute1:value1; attribute2=value2; attribute3=value3; ...">
2. internal: HTML tags and CSS styles won't be in same line, rather in the same project
    * <style>
        selector{
            attribute1: value1;
            attribute2: value2;
            ...
        }
    * It helps to define common attribute for whole program. However, 'inline' setting takes up more memory (whose?)
3. external: CSS styles are defined in separate file with .css extension.
    * <link> tag is used to link HTML and CSS files.
    * these styles/settings are for global use

Notes: 
- it has only attributes (and no tags) which are to support HTML
- 'style' defines CSS setting
- if <style> and <link> are to be defined inside the <head> tag, else they won't work.




## CSS Attributes
1. colors:
    * defined in 3 ways:
        1. color name (e.g., red, green, blue, cyan, etc.)
        2. rgb (range 0-255 for each) - e.g., rgb(100,255,150)
        Note: if rgb value for any component is given >255, like 355 => 355%255 = 100 (modulus operation)
        3. hexadecimal colors (range 0-F for all 6 bits of 8 bits each) - #18bb6e
    * color:rgb (and similar) are for global attributes
    * background-color:red (and similar) are for inline
        E.g.: <h1 style="color:red; background-color=yellow;">...text...</h1>
2. border: 
    * defined in pixel (px)
        E.g.: 
        <p style="border:5px solid rgb(12,192,21);">
        <img src="images/squirrel.jpeg" width="400px" height="350px" style="border:10px solid red;">
    * types of border: 
        1. solid
        2. dotted
        3. outset/inset (3D shade)
        4. dashed
        5. ridge (3d type)
3. box-shadow: 
    * to display shadow for HTML element
    * Syntax: 
        box-shadow: Xpx Ypx color;
            where XY are: ++ -+ -- +- (1, 2, 3, 4 quadrants)
        box-shadow: px1 px2 px3 px4 color;
            quad in clockwise dimension of shadow
    * E.g.,
        <p style="background-color:#cfbeab; box-shadow:3px 3px;"></p>
        <p style="background-color:#cfbeab; box-shadow:3px 3px; #ff0000"></p>
4. text-shadow
    * to display shadow on text
    * Syntax:
        text-shadow: Xpx Ypx color;
            where XY are: ++ -+ -- +- (1, 2, 3, 4 quadrants)
        text-shadow: px1 px2 px3 px4 color;
            quad in clockwise dimension of shadow
5. border-radius: 
    * to give curvature to box
    * Syntax: 
        border-radius: Npx;
            i.e., all corners similar curve
        border-radius: Mpx Npx;
            i.e., two diagonal corner pair
    * E.g.,
    <img src="images/Jeep.jpeg" width="400px" height="300px" style="border-radius:150px 50px">
    * We can make circles using this attribute, when N=width/2
6. font-size: used to change size of text
    * Syntax: font-size: Npx;
7. font-family: used to change text writing style
    * Syntax: font-family:<name>;
    * name - tahoma, arial, times new roman, etc.
    Notes: 
    1. We can give multiple font family names separated by space. The browser will choose from left to right whatever is available.
    2. And in case none of the provided is available, then default font of the browser precedes.
    3. And if all/multiple supported then leftmost will be selected.
    4. this helps to fix different browser problem
8. list-style-type: 
    * used to specify the list bullet (same for <ol> and <ul>)
    * Syntax: 
    list-style-type:<type>
    <type>: 
        decimal
        upper-alpha
        lower-alpha
        upper-roman
        lower-roman
        lower-greek
        leading-zero-decimal
        none
        dot
        circle
        square
9. list-style-image:
    * used to specify images for list bullets (all same or all different)
    * Syntax:
        list-style-image:url/filename
        url: source location from anywhere
    * bullet icons need to be small, else the margin gets hampered. 
        