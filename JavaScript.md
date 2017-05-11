# JavaScript
## Complete Beginners

### JavaScript Basics 
JavaScript ("JS" for short) is dynamic programming language that adds interactivity to your website(for example: games, responses when buttons are pressed or data entered in forms)<br>


#### How the web works 

> ***How the Web works*** provides a simplified view of what happens when you view a webpage in a web browser on your computer or phone.


##### So what happens, exactly 
When you type a web address into your browser(for our analogy that's like walking into the shop) <br>

>1. The browser goes to the DNS Server and finds the real address of the server that the website lives on(find the address of the shop)   
2. The browser sends the HTTP request to the server, asking it to send a copy of the website to the client(you go to shop and order your goods). This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP. 
3. Provided the server approves the client's request, the server sends message "200 OK", which means "of course you can look at the website!, here it is", and then starts sending responses back to browsers as a series of small chunks called data package( the shop gives you the good you have ordered, and you bring them back to your home) 
4. The browser assembles the small chunks into a complete website and displays it to you(the good arrives at your door) 



### JavaScript Learning Steps  
- Learn basic grammar of Javascript 
- Learn how to debug html elements and write JS code using browsers (Chrome, Firefox)  
- Learn even-driven pattern in JS (click, focus, keyup, keydown ...)   
- built-in objects and functions in JS 
- Closure & Prototype use in JS


#### JavaScript Grammar

##### Basics 
- case-sensitive 
- Grammar is similar to JAVA
##### Comments 

Comments is sthe same as in C++ and in many other languages 
##### Declarations 
`var` `let` `const`<br>
**var** : Declares a variable, optionally initializing it to variable. `var a = 1;` <br>
**let** : Declares a block scoped, local variable, optionally initially it to a value. (Let,to some extent, can replace closure.)<br>

```JavaScript 
var nodes = document.getElementsByTagName('li');
    var node = undefined;
    //Use Let to create a block scope
    for(let i = 0 ; i < nodes.length; i++){
        node = nodes[i];
        node.onclick = function(){
            console.log(i);
        }
    }
    //Use closure to cache i in memory
    for(var i = 0 ; i < nodes.length; i++){
        node = nodes[i];
        node.onclick = (function(i){
            return function(){
                console.log(i);
            }
        })(i);
    }
```
<br>**const**: Declares a constant variable (block scoped) that can't be changed. 
`const a = 1; a = 3;`
in above code, it throws an exception saying ***Uncaught TypeError: Assignment to constant variable.***

  
##### Data Structures and types 

#####Data Structures 
Array,Object, 

#####Data Types 
`object`,`number`,`function`,`string`,`undefined`, `boolean` <br>


##### Literals 


##### JavaScript Building blocks 

- Making decisions in your code - conditionals 
- Looping code 
- Functions - reusable blocks of code 
- Build your own function 
- Function return values 



 