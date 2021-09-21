# Reading Notes

## Tables 📊

```<table>, <tr>, <td>, <th>```

Tables are used to depict information on x and y axes. We use tables to compare high scores, stocks, avg temperature readings, daily prices, and more.
To create a table, use ```<table>```. Indicate each row with ```<tr>```, and give that row a title, or heading, with ```<th>```. Lastly, the 
data is inserted into the row using ```<td>```.

```<colspan=""> ``` and ```<rowspan="">```
Whenever your entries need to reach across multiple columns, use the colspan attribute. For example, if you need to stretch across two rows, you would use 
```<td colspan="2">```. You would use a similar attribute to reach across multiple rows, such as ```<td rowspan="3">``` to cross three rows. 

```<thead>, <tbody>, <tfoot>```
Long tables can be difficult to decipher if there isn't a visual separation between the main content and the header and footer of the table. Wrapping the 
```<th>``` elements will underline the headings, giving them an easy to read, visual delineation. Wrap body and footer elements in the corresponding tags. 

```<table width=" " cellpadding=" " cellspacing=" ">```
Adjusting the size and spacing of the table cells is simple. Using the attributes listed above, you are able to customize the look of your tables and 
organize the data held in them. 

## Functions, Methods and Objects

##### * *...continued from reading 6* * 

### this

"This" is a keyword used inside an object or function to point to the object or function itself. Using * *this* * in an object will allow you to point to 
the object's own properties. For example, ```this.model``` used on an object called 'companyCar' may result in the value "F-150". Here, "this" replaces
"companyCar" (instead of companyCar.model => "F-150").

### Built-in Objects

Three types of built-in objects are used in the creation of interactive webpages: Browser Object Models, Document Object Models, and Global Javascript Objects.

These objects come with their own methods and are used to mainpulate the various types of data you will encounter in web development. For example ```math.random``` uses 
the global object math and its method .random.

