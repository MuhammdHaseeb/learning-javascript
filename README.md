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
