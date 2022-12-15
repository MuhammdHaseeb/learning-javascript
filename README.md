# learning-javascript
///$$$$$$$$$$$$$$$$$$$$$         Static Vs Dynamic websites      $$$$$$$$$$$$$$$$$$$$$$$////
A static website is one with stable content, where every user sees the exact same thing on each individual page.
On the other hand, a dynamic website is one where content is pulled on-the-fly, allowing its content to change with the user.

///$$$$$$$$$$$$$$$$$$$$$         Static Vs Dynamic language      $$$$$$$$$$$$$$$$$$$$$$$///
 Dynamically-typed languages perform type checking at runtime, while statically typed languages perform type checking at compile time.
 statically-typed languages require you to declare the data types of your variables before you use them, while dynamically-typed languages do not.
 Dynamically-typed languages are more flexible and can save you time and space when writing scripts. However, this can lead to issues at runtime .
 
 
 
 
 
 
 
 //Errata:  خرابی
 // all modern browsers understand JavaScript—and soon you will understand it too.




https://dev.to/this_mkhy/do-you-know-es6-part-3-advanced-3fcl#IIFE-1   (important link for promises, async, await concept)









https://dev.to/dailydevtips1/10-games-to-learn-javascript-155j
















function print(callback) {  
    callback();
}

The print( ) function takes another function as a parameter and calls it inside. This is valid in JavaScript and we call it a “callback”. So a function that is passed to another function as a parameter is a callback function. But that’s not all.


Callbacks make sure that a function is not going to run before a task is completed but will run right after the task has completed. It helps us develop asynchronous JavaScript code and keeps us safe from problems and errors.

In JavaScript, the way to create a callback function is to pass it as a parameter to another function, and then to call it back right after something has happened or some task is completed. Let’s see how…


const message = function() {  
    console.log("This message is shown after 3 seconds");
}
 
setTimeout(message, 3000);



In other words, the message function is being called after something happened (after 3 seconds passed for this example), but not before. So the message function is an example of a callback function.


Callback as an Arrow Function
If you prefer, you can also write the same callback function as an ES6 arrow function, which is a newer type of function in JavaScript:

setTimeout(() => { 
    console.log("This message is shown after 3 seconds");
}, 3000);


Note: The callback function is helpful when you have to wait for a result that takes time. For example, the data coming from a server because it takes time for data to arrive.


// callback function

function greet(ab, cb){
       console.log("haseeb"+" "+ ab);
       cb();
}

function callme(){
       console.log(" I am a callback function");
}

greet("Salam", callme);

]





// callback function

function morning(name, callbackfunction){
       console.log("Hello world");
       callbackfunction(name)
}

function morninggreet(name){
       console.log("Hello" +" "+ name)

}
setTimeout(morning,2000, "John", morninggreet)







Symbol is a brand new data type introduced in ES6 (we mentioned ECMA Script 6,
or ES6, in Chapter 1, Getting Started with JavaScript). Symbol can be used when it is
important that variables are not equal, even though their value and type are the same
(in this case, they would both be of the symbol type). Compare the following string

declarations to the symbol declarations, all of equal value:
let str1 = "JavaScript is fun!";
let str2 = "JavaScript is fun!";
console.log("These two strings are the same:", str1 === str2);
let sym1 = Symbol("JavaScript is fun!");
let sym2 = Symbol("JavaScript is fun!");
console.log("These two Symbols are the same:", sym1 === sym2);
And the output:
These two strings are the same: true
These two Symbols are the same: false




There is an odd one out, and that is the null type. In the output you can see that
typeof null returns object, while in fact, null truly is a primitive and not an object.
This is a bug that has been there since forever and now cannot be removed due to
backward compatibility problems. Don't worry about this bug, as it won't affect our
programs—just be aware of it, since it will go nowhere anytime soon, and it has the
potential to break applications.




String(), Number(), and Boolean()

let nullToNr = null;
nullToNr = Number(nullToNr);
console.log("null", nullToNr, typeof nullToNr);
let strToNr = "";
strToNr = Number(strToNr);
console.log("empty string", strToNr, typeof strToNr);
The preceding code snippet will log the following to the console:
null 0 number
empty string 0 number



let strToBool2 = "false";
strToBool2 = Boolean(strToBool2);
console.log(strToBool2, typeof strToBool2);
let strToBool = "";
strToBool = Boolean(strToBool);
console.log(strToBool, typeof strToBool);
Finally, this one will log the following:
true boolean
false boolean
This output shows that any string will return true when converted to a Boolean,
even the string "false"! Only an empty string, null, and undefined will lead to a
Boolean value of false.
