#Reading 10

## Error Handling & Debugging 🐞

 Some things to sort through when beginning the debugging process:
 
 * Order of Execution
  * The Stack - when a line of code requires data from another function, the new function is piled on top of the current task. (Javascript & JQUERY, Jon Duckett, pg. 454)
 * Exectution Context
 * Scope
 * Error Objects
  * Using the console to track down what the type-errors are and where they occured. 
 
 ###Deal With It 🕶️
 
 1. Debug the Script/Fix Errors
 2. Handle Gracefully: Try, Catch, Finally
    * ```try{
      ``` //try to execute this
      ```}
      ```catch{
      ```//If there is a problem, run this
      ```}
      ```finally{
      ```//always execute this
      ```}
      
   Other tips:
   * Try another browser
   * Add numbers to the console
   * Simplify
   * Explain code
   * Stack Overflow
   * www.jslint.com
