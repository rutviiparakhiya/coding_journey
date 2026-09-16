 							JS(High-level-language)

#_Diffrence between var, let and const :-
 	1. var : i) Function scoped ii) Can be redeclared and updated iii) Hoisted(can cause bugs).
 	2. let : i) Block scoped ii) Can be updated, not be redeclared iii) safer than var.
 	3. const : i) Block scoped ii) can not be redeclare or updated iii) value must stay the same.

#_What is scope :-
 	i)  Scope refers to the accessibility (visibility) of variables and functions in different parts of a program.
ii) It determines where a variable or function can be used.
 	Types :-

 			1. global scope   : variables that can be accessed from anywhere in the program.
 			2. function scope : Variables that can be accessed only inside that function.
 			3. block scope    : Variables that are accessible only inside { } block (like if, loop).
 			4. lexical scope  : Inner functions can access variables from their outer parent scopes.
 			5. scope chain    : Looking for a variable step by step, from inside to outside until found.

#_what is hoisting?:- (var only)
 	we can access variables and functions before declaring them.
 	In simple words : js no code run thay e pehla js na varibles ane function na declartion ne temna scope na top pr ly jay.
 		e.g. - console.log(x); // undefined
 		       var x = 5;
 				it's treated like this : var x;
 							 console.log(x); // undefined
 							 x = 5;


#_Temporal dead zone :- a time between we run the programme and the value is assigned.


class:- blueprint of object
object:- instance of class
constructer:- to allocate the memory
deconstructor:- to recover the memory
static:- must use in the class (method)
extends:- to access element of parent class into the child class(inheritance)
super:- call the parent class’s constructor


stack: lifo-> last in first out

queue: fifo-> first in first out

linked-list->   singly
 		doubly
 		singly circular
 		doubly circular



Hash_map :->    o(2^n) // exponential		!!worst
 		o(n^2) // n rasto 2
 		o(n log n) // array
 		o(n)
 		o(1) // hashmap 		!!best

#_Clouser :
A function that remembers and can use variables from its outer scope, even after the outer function has finished.


Asynchronous execution allows a program to perform multiple tasks at the same time without stopping the execution of other code.
Synchronous execution means a program waits for a task to complete before moving on to the next task.

set time out : setTimeout() is used to execute a function once after a specified time delay.
set interval : setInterval() is used to execute a function repeatedly at fixed time intervals.
set immidiate : setImmediate() is used to execute a function immediately after the current execution is completed.

promise : A Promise is a way to handle asynchronous work without using many callbacks.
 	.all - All Must Succeed
 	.allsetlled - Wait for All (Success or Fail)
 	.race - First One Wins
 	.any - First Successful Promise
 	.finally - Always Executes

rest -
 	get: read only
 	post: create a new resourse
 	put: Replace an Entire Resource
 	patch: Update Part of a Resource
 	delete: remove a resoure

call back : a callback is a function, it is used to passed the argument to another function, which is executed later, usally after same task is completed
 	e.g. - function first (callback)
 	       {
 			callback();
 	       }
 		function second()
 		{
 			console.log("hello");
 		}
 		first (second);

callback hell : call back hell happens when multiple calbacks are nested inside each other.
 		- hard to read
 		- hard to debug
 		- hard to resuse

#_app.jsx
what is jsx?
java script XML : java script extensible markup language
jsx: it provides the feature through

#_props:
component's skeleton is same but their if we change inner data then we use pops.(property)

HIGH (Micro task queue) :-
promise, async/await, callbacks

Low(Macro task queue) :-
set Timeout, interval, immediate

micro:-

promise
2. async/ await
3. callbacks

macro:-

4. Immediate
5. interval
6. set Timeout





















 