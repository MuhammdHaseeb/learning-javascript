Dude mean man/friend
relax ===chill
to study hard === to cram
to do well == to ace e.g: I aced my math exam mean I did very well.

amazing/good//enjoyable === lit/Dope
crazy === nuts
# learning-js is an excellent choice.

Q:Usage of js?
A:it is used in both side server side and client side.

Q:Difference between server side and client side?
A:Server side mean itt runs on computer in data center and interact with database.
Client side mean it runs on the device of the user.

Q:When js originate?
A: It originate in 1995.

Q:Why should you learn JavaScript?
A:JavaScript is the language that web browsers support and understand. It is a great programming language for beginners and a great choice for beginners. JavaScript can be used for (semi) object-oriented, functional, and procedural programming, which are just different programming paradigms.  Examples of these great libraries and frameworks include React, Vue.js, jQuery, Angular, and Node.js.

Q:What is stack overflow?
Stack Overflow is a question and answer website for professional and enthusiast programmers. It is the flagship site of the Stack Exchange Network. It was created in 2008 by Jeff Atwood and Joel Spolsky. It features questions and answers on a wide range of topics in computer programming.

Q: How to Setting up your environment for js?
A: You need IDE, Web browser(it's better not to use Internet Explorer, which doesn't support the latest JavaScript features. Two good options would be Chrome and Firefox. They support the latest JavaScript features and helpful plugins are available),

Q: What is Integrated Development Environment (IDE)
A: An Integrated Development Environment (IDE) is a special application that is used to write, run, and debug code. You can just open it like you would any program. For example, to write a text document, you need to open the program, select the right file, and start to write. Coding is similar. You open the IDE and write the code. If you want to execute the code, the IDE often has a special button for this. Pressing this button will run the code from inside the IDE.

Q: Write the names of different types of IDE.
A: VS Code, Atom, Sublime Text, and WebStorm.

Q:How does the browser understand JavaScript?
A:Js is an interpereted language which mean that the computer understands it while running it. Some languages get processed before running, this is called compiling, but not JavaScript. The computer can just interpret JavaScript on the fly. The "engine" that understands JavaScript will be called the interpreter here.

Q: Web page consist of how many languages?
A: Web pages are written in three languages: HTML(HTML determines what is on the page; the content of the page), CSS(CSS is the layout(he way in which the parts of something are arranged or laid out."the road layout") of the web page), and JavaScript( defines what the web page can do and how it can interact with the user or the backend. ).

Q:What is ECMAScript?
A:This is the specification or standardization for the JavaScript language. The current standard is ECMAScript 6 (also referred to as ES6). Browsers use this specification to support JavaScript, ECMAScript can be considered the basic specification that the JavaScript implementation will definitely include.


Q: How to link JavaScript to a web page?
A: There are two ways to link JavaScript to a web page. The first way is to type the JavaScript directly in the HTML between two <script> tags. In HTML, the first tag is <script>, is to declare that the following script will be executed. Then we have the content that should be inside this element.
<html>
 <script type="text/javascript">
 alert("Hi there!");
 </script>
</html>
If you store this as a .html file, and open the file in your browser. We will be storing this one as Hi.html.
The alert command will create a popup that provides a message. 

Next, we close the script with the same tag, but preceded by a forward slash, </script>. Or you can link a JavaScript file to the HTML file using the script tag at the head of the HTML page. Linking an external file to our web page: You could also link an external file to the HTML file. This is considered a better
practice, as it organizes code better and you can avoid very lengthy HTML pages due to the JavaScript. First, we are going to create a separate JavaScript file. These files have the postfix .js. I'm going to call it ch1_alert.js.

 <script type="text/javascript" src="ch1_alert.js">     </script>

Q:What is the shortcut key for opening the console on browser?
A: F12

Q: What is console nad debuging?
A: The console is used by developers to log what is going on and do any debugging. Debugging is finding the problem when an application is not displaying the desired
behavior. The console gives some insights as to what is happening if you logsensible messages.

Q: What is the use of console.log(); in js?
A: The console.log() is a function in JavaScript that is used to print any kind of variables defined before in it or to just print any message that needs to be displayed to the user.
 
 Q: What is the syntax to write console.log()
 A: There are two two different syntaxes for different purposes. One syntax for printing variable/object/function etc. syntax: console.log(name of variable/object/function write here in parenthesis); 
 the other syntax is for printing any message that need to be displayed on the user, that synax is following
console.log("");



Q: What is the use of alert function in js?
A: The alert() function. This function will display text in a dialog box that pops up on the screen.

Q:What is the syntax to write alert?
A: here are two two different syntaxes for different purposes. One syntax is for printing variable/object/function etc. syntax: alert(name of variable/object/function write here in parenthesis); 
 the other syntax is for printing any message that need to be displayed on the user, that synax is following
alert("");

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
