# Reading Notes

## Layout

Designing the layout of a web page is like working with blocks of many sizes in a rectangular frame. Some blocks are very large and will not allow others to 
sit next to them ```display:block```, some are small and can have neighbors ```display: inline```. Some blocks can open to reveal something inside of them. 
Arranging your blocks in a way that is pleasing can be challenging if you don't know what each block's characteristics are. 

### Positioning

Below is a list of a few characteristics that can change the behaviors of your "blocks", or elements, as they are called:

  * ```relative-positioning: ``` - can shift an element's position within its parent * *relative* * to that parent.
  * ```absolute-positioning: ``` - causes elements to essentially leave the flow within the parent element, placing the item in a fixed,forward position.
  * ```fixed-positioning: ```    - is similar to absolute, but * *fixes* * the element to a position on the browser window.
  * ```float: ```                - allows an element to be buoyed up to the top left or right of its containing element.
  * ```z-index: ```              - allows you to decide which element would "sit on top" by giving each element a z-index value. The higher value sits on top.

### Screen Sizes

**Resolution** is "the number of dots a screen shows per inch" (*HTML & CSS*, Jon Duckett, p. 378). Screens come in many sizes and, therefore, will vary widely in 
what resolution they will display. 

To address this problem, designers typically create pages between 960-1000 pixels wide. This will allow most users to see the designs of the web page, with perhaps
only a few outliers. 

Understanding what a user will see initially is also very important. If the majority of important information is hidden from view upon loading the page, a user may
miss what it is they are looking for. 
