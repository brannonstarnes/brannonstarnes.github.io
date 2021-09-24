# Reading 09

## Forms and Events

  > "Ma'am, could you please fill out this form and then we will be right with you". 

Filling out forms may remind you of a number of situations we might face in everyday life: filling out patient notes at the 
doctor's office, getting permission slips signed for that awesome field trip to the fidget-spinner factory, or signing your 
life over to the devil for some amazing fiddling skills. Forms require some input from us * *before* * a desired output can 
be made into a reality. This is no different in the realm of web pages. HTML presents us with the pen and paper, and Javascript 
is the devil playing the fiddle and fulfilling the deal. 

Let's see some examples:

```<form>``` starts us off, just like the clerk behind the desk handing us a clipboard.
```<input>``` is like the paper on the clipboard, and its attributes ```name= ``` and ```type= ``` 
    tells us what needs to be written on each line.  
      For example: ```<input name="Your Name" type="text"> ```
        This would display a box titled **Your Name** ____________ and expects a text input.

Just like paper forms, there are many options for taking inputs:
  * Checking boxes ```<type='checkbox'>```
  * Multiple choice ```<type='multiple'>```
  * Fill in the circle ``<type='radio'>```
  * Enter a Date ```<type='date'>```
  * And More!

## Now on to the Event! 🚌

Once you've turned in your permission form its time for that fieldtrip! Let's take a look at the Javascript schoolbus that will
take us there.

### Event Listeners
```element.addEventListener('event', functionName);```

The event listenter is essentially the person (or underworld overlord) waiting for you to turn in your form.Beautiful ain't she? 
This essentially means when * *some predetermined event* * happens to the element in question, a function fires off.

Look at is like this:
```permissionSlip.addEventListener('turnInSlip', headToFidgetSpinnerFactory);```

Now that you've '*(event:)* turned in' your '*(element:)* permission slip', you get to '*(functionName:)* head to the Fidget Spinner Factory
with your classmates! 
