# background Attribute

## Theory
1.  To set background of elements with images, etc.
2. Attributes: 
    a. background-image: to set an image for an element (like box, etc.)
        Syntax: background-image: url("image-path");

    b. background-size: to set the dimensions of the background image inside the element
        - Values: 
            cover: complete area is covered by image inside the element
            contain: fit into the area, but with same dimension as original. Hence, it'll start repeating the image beside the smaller dimension
            auto: it'll give image as usual photo without modifying dimensions (default view)
    c. background-repeat: to set if we need the image to repeat in the background.
        - Values: no-repeat