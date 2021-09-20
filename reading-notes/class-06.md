# Reading 06

## Objects

  Objects take a set of variables or functions and "create a modelof something you would recognize from teh real world". (Javascipt and JQUERY, Jon Duckett, p.100)
  
   > Example: ```var car = {
   >             make: "Volkswagen",
   >             model: "Golf",
   >             year: 2003,
   >             turbo: true,
   >             checkMaintenance: function(){
   >             code here; }
   >             }; ``` 
 Note that the function, above, when inside an object is known as a * *method* *. 
 
 ### Object-literal Notation
 
  The example above, using a declared variable and listing it's properties, is known as object literal notation. However, objects can be created in other ways.
   
 ### Constructor Notation 🏗️
 
  > Example: ```var car = new Object();
  >             car.make = "Volksawagen";
  >             car.model = "Golf";
  >             car.year = 2003;
  >             car.turbo = true;
  >             car.checkMaintenance = function(){
  >               code here;
  >             }; ```

  The constructor method, above, is not as popular, but is a useful way to add properties to an object you created regardless of the method used to initially creat the object. 
  
  
 ##### * *Below is beyond the scope of the current assigned reading, but useful* * 
 ### Accessing Objects and Using Dot Notation
 
 In order to get the stored property of an object, we use dot notation. 
 
 ``` var carName = car.name;```
 ``` var needMechanic = car.checkMaintenance(); ```

The dot is known as a member operator. You also have the option of replacing the dot with an open square bracket which wraps the property or method name. These notation methods are also used to update the properties.  
  
## The DOM

### Document Object Model

  This concept refers to the manner in which a web browser will create a model of the HTML page and allow Javascipt to access  and manipulate its contents. For example, a clicked button may change the title of the page via the actual HTML code. 
  
### DOM Tree 🌳

Think of the DOM tree as the actual model of the webpage, made up of nodes. These vary from document nodes, element nodes, attribute nodes, and text nodes. 
