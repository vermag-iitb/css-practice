# Display Attribute

## Theory
1.  Used to change the position of HTML element.
2. Syntax: display: inline/block/inline-block/none;
    ![alt text](resources/display-attribute.PNG)
3. Types:    
* display:inline;
    - takes only the space required by the element (no-margin/padding)
    - to make tags come inline (in one line)
    - Margin and padding are not applied to inline elements. 
    - height and width are also not applicable for inline elements
* display:block;
    - takes full space available in width
    - to make inline tags to go in block (separate lines)
* display:inline-block;
    - to display inline and block level components side-by-side with uniform margin
    - similar to inline, but we can set margin and padding
* display:none;
    - to remove element from document flow
    - used to hide element on the webpage
    - there is another attribute to make an element hidden. However, in case of 'visibility' attribute a space is still allocated while in case of 'display: none' attribute, there is no space allocated for the element: 
        visibility:hidden
* display:grid;
    - to display elements grid-wise
* display:flex;
    - to display elements in column/row (or matrix) -wise (also called containers)
4. Note: 
* heading tags (h1, h2, etc.) are not inline by default. Hence, when we define "display" attribute as inline to make them inline.
* anchor tag is inline by default
* in case of defining display attribute for same tag multiple times, then only first one is considered with its value.
5. Examples:
    1. display: inline-block;
    <style>
        .menus
        {
            background-color:#ee11ff;
            width:150px;
            display:inline-block;
            text-align:center;
            text-declaration:none; // to remove underlying of hyperlink
        }
    </style>

    <a href=".." class="menus">Course</a>
    <a href=".." class="menus">Services</a>
    <a href=".." class="menus">Batches</a>
    <a href=".." class="menus">Contact</a>

    <!-- Output:
    -----------------------------------------
    | Course | Services | Batches | Contact |
    ----------------------------------------- -->

    2. display: inline;
        <h1 style="background-color:red;display:inline;">CSS</h1>
        <h1 style="background-color:red;display:inline;">HTML</h1>
    3. display: flex;
        <style>
            .one {background-color:#ffee00;}
            .two {background-color:#ffee00;}
            .three {background-color:#ffee00;}
            .four {background-color:#ffee00;}
            #main-class{display:flex;}
        </style>
        <body>
            <div class:"main-class">
                <div class="one">
                    <h1>Jan</h1>
                </div>
                <div class="two">
                    <h1>Feb</h1>
                </div>
                <div class="three">
                    <h1>Mar</h1>
                </div>
                <div class="four">
                    <h1>Apr</h1>
                </div>
            </div>
        </body>
    **Note:**
    * The width of the content increases as per the no. of letter.
    * 'Flex' type of 'display' attribute, is defined for outer tag but applied to inner tags.
    * if no. of contents are added further, then the columns will keep on increasing in same line with width addusting by itself.
    * Other attributes related to "display:flex" attribute: 
        - flex-direction: row (default)/column/row-reverse/column-reverse
        - flex-wrap: wrap/nowrap
        - gap:10px (to apply gap of 10pm between each containers)
    * 'display:flex' attribute is good for column-matrix or row-matrix view of data

    4. display:grid;
    - Syntax: grid-template-columns:col1-px col2-px col3-px ... coln-px;
    <style>
        .main-div
        {
            display:grid;
            grid-template-columns:auto auto auto ... auto;
            // grid-template-columns: 300px 500px ... 400px;
            // grid-template-columns: 30% 40% 30%;
            column-gap: 20px;
            row-gap: 20px;
            grid-gap: 20px 30px; //row-gap col-gap
        }
