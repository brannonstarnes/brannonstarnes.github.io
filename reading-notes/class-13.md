# Reading 13

## Key/Value Pairs in Storage 🔑

Local Storage, or as the article calls it, HTML5 storage, is all based around key/value pairs. You will designate a keyword, 
which is a string, by which you will store and retrieve data of any type.

The big HOWEVER, in this case, is that if you are storing anything * *other than* * strings, you will need to stringify that 
data to store it, then parse it to return it to its original format when you pull it from storage.

## Set it, don't forget it!

Data is initally set, updated, or retrieved using the following commands:

```localData.setItem('foo')``` This will set the data to a keyword and place in local storage.
```localData.getItem('bar')``` This will * *get* * the data, or retrieve it form storage. 
```localData.setItem('newFoo')``` Reusing 'setItem' will update the key/value pair with new data. 
```localStorage.removeItem('byebyeFooBar')``` This will remove the data from local storage altogether.
