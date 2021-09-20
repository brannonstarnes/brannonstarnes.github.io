# Reading Notes

## Images

## ```<img>```

Images are a powerful resource which can deliver a large amount of a variety of information instantly.

Keeping images in a folder seperate from your index.html is a preferred organizational standard. Folders within those folders can further provide a simple method for finding images of different categories, such as images that contain buttons, or photos, or cat pictures 🐈 .

### src -

   This tells the browser where it can find the image you want to use.

### alt -

   When you are unable to see the image, such as while it is loading, this attribute will give a text description of the image.

### title -

   Hovering over an image often brings up a small description which is created using the title attribute.

### ```<fig> and <figcaption>```

   Used when a figure contains an image and uses a caption as a short descriptor.

### Saving and Deploying Images

   Use the correct format! .jpeg, .gif. and .png are the most common.
   Use the appropriate dimensions! This is a measurement using pixels ie, 300x400.

## Color

### RGB

   All colors are created from three primary colors. Red, green, and blue.
   The RGB values range between 0 -255. RGB = 102,205,170

### Hex Codes

   RGB is represented in a hexidecimal code. RGB = #66cdaa.

### Opacity

   In CSS3, opactiy can be specified on any element and its children. Values between 0.0 - 1.0 represent 0-100% opactiy.
   This can also be defined in RGB values as a fourth value known as * *alpha* *.

## Text

   Choosing a typeface is an important decision when designing a web application or program. Some fonts will not be displayed if it isn't on the user's computer. However, it is possible to point the page to an external source of the desired font.

### Font-face

   The user will have to download the file, but this may slow the process of loading the webpage. (HTML and CSS: Design and Build Webpages, pg. 271). A src attribute is required to point to where the font file can be foound.

### Serif vs Sans-Serif

   Serif fonts have small details at the end of each letter stroke. Sans-serif removes these details.

## Units of Size

   Type sizes vary by the units they are measured by. Twelve pixel scale, percentage (ex. h1 is 200%) or ems, which allows you to change the size relative to a parent element.

## ```:link``` & ```:visited```

   These two "pseudo-classes allow you to style links before and after they have been visited.

## ```:first-letter``` & ```first-line```

   You may apply an independant set of values to the letter at the beginning of an element, or the whole first line.
