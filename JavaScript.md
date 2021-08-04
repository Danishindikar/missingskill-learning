# JAVASCRIPT

### History of JavaScript

* JavaScript was Created  by **Brendan Eich** in 1995.
* Basically JavaScript is a **Kernel**.
* Javascript language is created in just 10 days.
* First it was named as **Mocha** then named as **liveScript** and then  later **JavaScript**.
* JavaScript is also known as **EcmaScript**.
* While creating Js Brendon did not add many things at that time because of such less duration was given to him.
* so these things are called as **Tech Debts**
* Now these Tech Debts cannot be updated because JavaScript is 
used by millions of Developers and to update these things will crash it.
* JavaScript is very popular and can be used both in Front End as well as Back End Development.
* As per the Surveys done majority of the Developers has chosen JavaScript as their First Choice for Development.


### Control Structure

1. ##### if-else
If the Value is True the if Condition will Execute otherwise Else condition get executed.
 
 **Syntax**:- ```if(condition)[//execute if condition is true]```
                 
                else[//execute this if condition is false]```
   
   2. #### For loop
   it will execute codes number of times till the given value reaches to its limit
   
   **Syntax**:-
   	```for(initialization;Condition;Increment/decrement){}```
   	
   3. #### Switch Case 
   
   It is used to choose the option provided
   
   **Syntax**:-   ```switch(expression){case n: break}```
   
   4. #### While loop 
   
   code execute till specific condition is true
   
   **syntax**:-  ```while(condition){//code to be execute}```
   
   5. #### do-while 
   
   code execute once then if the condition is true it will execute again
   
   **syntax**:- ```do{//code to be execute}while(condition);```
   
   ### Operators
   
   *  #### Arithematic operator
   
   1. ( + )  Add if both operands are numbers
   e.g:- (a+b)
   2. ( - )  Substract if both operands are numbers
   e.g:- (a-b)
   3. ( * ) Multiplication
   e.g:- (a*b)
   4. ( / ) Division
   e.g:- (a/b)
   5. ( + ) Concatination if one of the operand is of type string
   e.g:-(a+"b")
   6. ( % ) Modulus gives remainder as Output
   e.g:- (a%b)
   7. ( == ) Equal To
   e.g:- (a == b)
   8. ( === ) First check type of variable and the gives output as boolean value
   e.g:- (a === b)
   9. ( != ) Not Equal to
   e.g:- (a != b)
   10. ( > ) Greater than
   e.g:- (a > b)
   11. ( < ) less than
   e.g:- (a < b)
   12. ( >= ) Greater than and equal to
   e.g:- ( a>=b )
   13. ( <= ) Less than and equal to
   e.g:- ( a<= )
   
   ### Logical operator
    
   1. ( && ) AND operator
   e.g:- (True && False = False)
   
         
         (False && False = False)
         
         (False && True = False)
         
         (True && True = True)
   
   2. ( || ) OR operator
   e.g:- (False || True = True)
   
         
         (True || False = True)
         
         (True || True = True)
         
         (False || True = False)
   3. ( ! ) NOT operator
   e.g:- (a != b) or !( a == b )
   
   #### Bitwise Operator
   1. ( & ) bitwise AND
   e.g:- (a & b)
   2. ( | ) Bitwise OR
   e.g:- (a | b)
   3. ( ~ ) Bitwise NOT
   e.g:- ( ~ a)
   
   #### Ternary Operator
   
   1. (? : ) Ternary operator
   e.g:- ( a?b:c )
   
   
   #### Tech Debts
   1. (concat & addition) => a+a = aa
   2. ( = = = ) => Equality Check
   3. Typeof Null is given as object.
   
   
   ### JavaScript Variables
   
   * JavaScript is of Dynamic Type
   * Variable acts like a container which can hold any type of data
   * There are 3 types of variables is JavaScript
   1. **var**
   2. **let**
   3. **const**
   
   
   
<table>
<thead>
	<tr>
		<th>var</th>
		<th>let</th>
		<th>const</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>can be redeclared</td>
		<td>as per (es6) let can't be redeclared</td>
		<td>as per (es6) const can't be redeclared</td>
	</tr>
	<tr>
		<td>can be re-initialize</td>
		<td>can be re-initialize</td>
		<td>can be re-initialize but non-primitive value can be updated</td>
	</tr>
	<tr>
		<td>functional scope</td>
		<td>lexical scope</td>
		<td>lexical scope</td>
	</tr>
	<tr>
		<td>hoisted</td>
		<td>doesn't get hoisted</td>
		<td>doesn't get hoisted</td>
	</tr>
</tbody>
</table>


![](WhatsApp%20Image%202021-08-04%20at%202.10.13%20PM.jpeg)


#### Categories of Variables

Mainly there are 2 Categories of Variables
1. ##### Primitive (Copy By Value)
2. ##### Non-Primitive (Copy by reference) 




#### Primitive
primitive are further classified as
* **string**  :- Every value you write inside " " will consider as String in JavaScript.
e.g:- "My name is Danish"
    
    syntax :- ```var name="Danish" ```


* **Number** :- All the numbers including decimal numbers are consider as Number in JavaScript

     syntax:- ```var number = 5; ```

* **Boolean** :- The Values **True** and **False** in JavaScript are considered as Boolean.

     Syntax :- ```var Bool = True;```

* **Undefined** :- The variables without any value or given value as undefined are Undefined in JavaScript

     syntax:- ```var name = undefined;```
* **Null** :- Null means empty . the type of null falls under Non-primitive object type.

* **Symbol(ES6)** They are given under ES6

#### Non primitive
Non primitive are further classified as


* **Object** :- Everything in JavaScript is an Object.
They are defined using {}
          ```var person ={name:"Danish",age:"23"};```

            typeof person object

* **Array** :- In JavaScript the is nothing like array Every thing is object
but array are written as []

    var array =["hello"]; 

    typeof array "string"

#### Falsy Values
* The values which shows boolean False on executing are all falsy Values
   * Null
   * NaN
   * " " => Empty string
   * undefined
   * 0
   * false
   
#### Truthy Values
* The values which shows boolean True on executing are all Truthy Values
   * []
   * {}
   * Number
   * string
   #### Functional Scope of Variable
* **Local scope** 

The Variables declared inside the function can only be accessed by the function.This is local scope

 
    function createUserName() {
        var userName = "Danish";
    }

    function showUserName() {
        alert(userName);
    }

    createUserName();
    showUserName(); // throws error: userName is not defined
* **Global Scope**

The Variables Declared outside the function and can be accessed by any function are called global scope


    function createUserName() {
        userName = "Danish";
    }

    function modifyUserName() {
        if(userName)
            userName = "Zaid";
    };

    function showUserName() {
        alert(userName);  
    }
    
    createUserName();
    showUserName(); // Danish 

    modifyUserName();
    showUserName(); // Zaid 

* **Lexical Scope**

The variable which is declared inside any {} are called as Lexical functions.

    function createUserName() {
        var userName = "Danish";      //lexical scope
    }

    function showUserName() {
        alert(userName);
    }



### Copy by value and copy by reference


* **Copy By Value**

In JavaScript every thing is copied by value


    var a= 10;  // primitive 
    var b=20;   // primitive    
    b=a+30; 
    console.log(b); 
    console.log(a);



* **Copy by Reference**

 When an object variable is copied, the reference is copied, but the object itself is not copied this is called as copy by reference
 
     function update(ref) {
      ref.key = 'newvalue';
    }
       var a = { key: 'value' };
      console.log(a);



## JavaScript FUNCTIONS

* JavaScript a function allows you to define a block of code, give it a name and then execute it as many times as you want.
* A function can include one or more parameters. It is optional to specify function parameter values while executing it.

#### **Function Structure**

    function fn_name(); {
    
    }
      fn_name();
 
  * functions behaves exactly like variables behave
  * if you redeclare the same function then it will override that function
  
         function fn_name() {
          console.log("print fn");
      
        }
        function fn_name() {
          console.log("print fn 2");
        }
        fn_name();
        output: Print fn 2


Because the function is declared by the same name fn_name so it will override the function and print fn 2

#### Properties of Function

* Hoisting

* Overwrite

* Scope

* Act as a container

* objects

* Normal declaration using the function name
* Function can be assigned to a variable.
* function can be return from another function
* function returns a function


#### First Class Function

First class function can be assigned to a variable and passed and returned to a function converted into a prototype constructor. It has access to everything under it

    function helloDouble(somevalue){
    console.log("print"+ somevalue);
    return somevalue*2;
    }
    var val=20;
    var result=helloDouble(val);
    console.log(result);
    output : print 20
                40
                
                
                
   #### Assignment Function
   
    var logicBoard=function(param){
       console.log("logicBoard" ,param);
       
     }
     var board= "i386";
     logicBoard(board);
     var board="i586";
     logicBoard(board);
   
    var newlogicBoard = logicBoard;
   
    var board = "8core";
    newlogicBoard(board);
   
     var newB = "nvidia";
    var gaeboard = newlogicBoard;
    gameBoard(newB)'
   
    output:
    logic Board i386
    logic Board i586
     logic Board 8core
     logic Board nvidia
   
   
   #### Cascading of a Function
   
   #### fn()()()()()();
   
   Here the innermost values are cascaded and they are displayed at the output this is called as cascading of function
   
   
   
   #### Higher Order function
   
   Function can receive a function from parameter and function can return a function.then it is called as Higher order function.
   
   #### Pure Function
   It is a function when we pass a value then it will return the same value that means the values are not overwrite or changed.
   
   #### IIFE - Immediate Invoked Function Expression
   

     (function() {
         console.log("Initialisation...");

     }
     ) ();
   
   Here we can call function only once because there is no initialisation to function so this is called as IIFE.
   
   #### Inline Function 
   
     var outside= (function(next){    //function assignment
      console.log("print.....");

     function hello(value){
              console.log("called....");
              next && (typeof next === "function")&& next(value);
    }

     return hello;
    })(function (value){
        console.log("printing value :",value)
    });

    outside(10);     // inline parameter

   
   #### Arrow Function 
     var h = (param) => {
         console.log("Arrow",param);
         param();

     }
    h(c)=> {
        console.log("called from inside arrow function to arrow function");

    } ) ;
  
  
  
  ## Builtin Object and Prototype
  
  #### Constructor
  * **typeof** a refers to **string**
  * if we add a ( . ) dot then it will become constructor
  * **typeof** a.object becomes **constructor**
  
  

        Function Person(name,exp){
          this.name = name;                           //this kewyword refers to object of class
          this.exp = exp;
        }

        var samal = new Person("Samal",12);                //created constructor
        console.log(samal);

        output : person{name: "samal",exp: 4}

#### Builtin Object/constructor

* **function** - not generally used

    ```var fun = new Function();```
* **String** - Heavily used by shadow object creator.

  ```var name = new string();```
* **Number** - It is used
             
     ```var num = new Number();```
* **Boolean** - Deprecated/don't use instead use Boolean function

   ```var yes = new Boolean();```
* **Array** - Very heavily used by shadow object creator
 
  ```var arr = new Array();```
* **Object** - Very heavily used by shadow object creation

     ```var bat = new Object();```
* **RegEx** - Not much used but good to know

  ```var exp = new RregExp();```
 * **Date** - Shows the current date
 
    ``` var val = new Date();```
 * **Math** - Mathematical expressions can be done
 
    ```Math.floor();```
  
  
  #### Declaration
  * Gets Hoisted
  * Overwrite
  
  #### Expression
  * Assignment
  * not hoisted
  * Anonymous function/un-named function



 ## JavaScript Array
  
  * Basically Array is a special type of variable that can store multiple values in it using a special syntax
  * Array can be created using array literals or array constructor syntax
  
  Example 1.
  
  
   ```var StringArray= ["one","two","three","four"];```
    
 
  This is used for writing literal syntax

Example 2.

```var numArray=newArray(3);```

This is used for writing constructor syntax

* Array can store value of different data types

### Builtin Methods in Array

* **Length()** :- 
  It is used to determine the length of a string.
  
    
      var str = "Hello World!";
    
      var n = str.length;
    
      output : 12
    
* **concat()** :- It is used to merge two or more arrays. This method does not change the existing arrays, but         instead returns a new array 

    
      const letters = ['a', 'b', 'c'];
    
      const numbers = [1, 2, 3];

   
      letters.concat(numbers);
   
      // result in ['a', 'b', 'c', 1, 2, 3]
    
* **Push()** :- It is used to add element at the end of the array and return new lenght of the array


      // Add a new item to an array

       var fruits = ["Banana", "Orange", "Apple", "Mango"];

      fruits.push("Watermelon");

       // OUTPUT: Banana,Orange,Apple,Mango,Watermelon

* **pop()** :- It is used to remove the last element of the array and returns that element

      var students = ['Danish', 'Sufiyan', 'Fahim', 'Sadik'];
    
      var popped = students.pop();
    
       console.log(students);
    
      console.log(popped);

      Output : Sadik
  
* **shift()** :- shift method removes the first element from an array and returns that removed element. This method changes the length of the array.

      const Students = ["Danish", "Sufiyan", "Fahim", "Sadik"];
    
      Students.shift();   // Returns "Danish"
  
 * **unshift()** :- Unshift method adds the element at the beginning of the array
 
        var Students = ["Danish", "Sufiyan", "Fahim", "Sadik"];
    
        Students.unshift("Aquib", "Sohail"); 
    
        //Returns ["Aquib","Sohail", "Danish", "Sufiyan", "Fahim", "Sadik"];
    
  * **ForEach()** :- The ForEach method executes a provided function once for each array element.
  
        const Students = ["Danish", "Sufiyan", "Aquib"];
    
        Students.forEach(myclassroom);
    
  * **map()** :- It creates a new array with the result of calling a function for every array element
  
        var numbers = [1, 4, 9];
    
        var roots = numbers.map(function(num) {
    
        return Math.sqrt(num)
    
 * **Filter()** :- It creates an array filled with all array elements that pass a test
 
        function Bigger(value) {
    
        return value >= 10;
        }

        var filtered = [12, 5, 8, 130, 44].filter(Bigger);
    
        });
    
 * **indexOf()** :- It is used to find the index of the element
 
        var array = [2, 9, 9];
    
        array.indexOf(2);     // 0
    
        array.indexOf(7);     // -1
    
        array.indexOf(9, 2);     // 2
    
        array.indexOf(2, -1);    // -1
    
        array.indexOf(2, -3);    // 0
  
* **includes()** :- To check whether elements is present in array or not.

      // Check if a string includes with "world"
    
    
       var str = "Hello world, welcome to the universe.";
    
      var n = str.includes("world");
    
      // OUTPUT: true
    
 * **slice()** :- It splits an array
 
       var Students = ['Danish', 'Sufiyan', 'Aquib', 'Sohail', 'Sadik'];

        var Classroom = Students.slice(1, 3);

       // Students contains ['Danish', 'Sufiyan', 'Aquib', 'Sohail', 'Sadik']

       // Classroom contains ['Sufiyan','Aquib']

* **splice()** :- To remove elements from array


       const Students = ['Danish', 'Sufiyan', 'Aquib', 'Sadik'];

       // At position 2, add 2 elements:

       Students.splice(2, 0, "Sohail", "Zaid");

       // returns ['Danish', 'Sufiyan','Sohail','Zaid', 'Aquib', 'Sadik']

* **IsArray()** :- To check Whether it is an array or not

      function Classroom() {

       var Students = ['Danish', 'Sufiyan', 'Aquib', 'Sadik'];

       var x = document.getElementById("demo");

       x.inner = Array.isArray(Students);
    
        
      }

      // OUTPUT: true...
  
  
      
### Es6 Builtin Functions
    
  * **SetTimeOut()** :- The code will run after some time which is provided
  
        const timerfn= function(){

        console.log("Printing after 2 seconds");

        }
          console.log("Running 1");

        setTimeout(timerfn,2000);

        console.log("Running 2")
        );

         //It will print first outputand After 2 seconds it will print 2nd output

     
* **SetInterval()** :- It is same like  SetTimeOut but it will keep running continously

       SetInterval(function(){

       console.log("Printing after 5 sec");

       },5000);

       console.log("Running 2");
     
//In output it will first print Running 2 then it will print "Printing after 5 sec" continously after every 5 secs

* **ClearInterval()** :- It will stop the continue execution of SetInterval

      console.log("Running 1");

      let counter = 0;

      const timer = SetInterval(function(){

      console.log("Printing after 5 sec");

      if(counter>5){

       ClearInterval(timer);

      }
      counter ++;

      }.3000);

* **ParseInt()** :- It converts anyting into an integer.

       const num = 10.18;

      let intNum = parseInt(num);

      console.log(intNum)
      //Output : 10

* **JSON()** :- It is a builtin object . JSON is often used to send data over the network

     
       var Student = {"FirstName"="Danish","LastName"="Indikar","age"=23};

# TRIVIA
### Function Short circuit and Function Chaining

#### a()()()()()()()().z

     let a= () => {
        return() => {
            return() {
                return() {
                    return() {
                        return() {
                            return() {
                                return() {
                                    return() {
                                        z: "Final value"
                                    }
                                }

                            }
                        }
                    }
                }
            }
        }
    }
    let result = a()()()()()()()().z;
    console.log(result);
    //Output: Final Value
    
    
### Function Chaining
#### a().b().c().d().e().z();

    function a() {
        return {
            b: function() {
                return {
                    c: function() {
                        return {
                            d: function() {
                                return {
                                    e: function() {
                                        return {
                                            z: function() {
                                                console.log("final");
                                            }
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
    a().b().c().d().e().z();
    
    
  #### a(1).b(2).c(3)(4).d(5).final;

    function a(p1) {
        return {
            b: function(p2) {
                return {
                    c: function(p3) {
                        return function(p4) {
                            return {
                                d: function(p5) {
                                    let total = p5+p4+p3+p2+p1;
                                    return {
                                    final:total;
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
    let result = a(1).b(2).c(3)(4).d(5).final;
    console.log(result);

