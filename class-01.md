# Structure
 In order to understand ___**how**___ to build a website, it is important to study the manner in which websites are structured. 
 Different types of documents, such as newspapers, forms, or advertisements, may need different structures.
   
## ***HTML (and specifically, its elements) describes the layout of a page.***

Tags as containers:
   Opening Tag ``` <p> 
                  ipsum here 
                           </p>``` Closing Tag
                           
Attributes give more details about an element and are attached to the opening tag. See the lang attribute here:
  ```<p lang="en-us"> ipsum there </p> ```
  
  
  ### Viewing Source of Webpages 🔍
  For my browser- SHIFT + CTRL + I
  This can be a valuable tool to learn how webpages are made. 
  
  
  # Extra Markup
 There have been several versions of HTML, SO:
 
 > ...each webpage should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using...

...like this: ## ```<!DOCTYPE html> ```

## ```<!-- Comments Go Here -->```

### Block Elements vs Inline
 Block elements, such as ```<h1>,<p>,<ul><li>```, will appear on new line.
 Inline such as ```<em>,<b>``` will appear within the text it is embedded.
 
 # Layout Elements
 
 Traditionally, layout items would be classified as ```<div>```s , such as a ```<div id = "nav">```.  
 ___NOW___ certain layout items have their very own element tags!
 - ```<header> & <footer>```
 - ```<nav> & <section>```
 - and more!
 -___***Please Note! Older browsers will require a line of CSS to render the layout elements correctly!***___
 > ```header, nav, section {display: block;}```

# Process

Use the 5 W's (Who, what, when, where, why) when thinking about how your audience will interact with the page.

Using wireframes can be a powerful tool when organizing the design for your website. Check out [gomockingbird.com](https://gomockingbird.com/home)!
  
 ## Visual Hierarchy and Grouping
 Plan on users skimming your page for bits of information rather than reading top to bottom. Use visual hierarchy to convey info!
 -Size - big stuff seen first
 -Color - bright stuff seen first
 -Style - standout style seen first
 
 Grouping can also convey that information on a page is related. Use this to help guide your users!
