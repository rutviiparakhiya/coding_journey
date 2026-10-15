◯ Type Script (TypeScript = JavaScript + Types)   

It is an extended version of JavaScript that adds types, making the code easier and safer to write.  
TypeScript adds types to JavaScript and is converted into JavaScript before running.  

◯ Diffrence between js and ts :-   

| js                                                          | ts                        |
| :-----------------------------------------------------------: | :-------------------------: |
| Dynamically typed                                           | Statically typed          |
| Types are checked at runtime during development/compilation | Types are checked         |
| Runs directly in browser/Node.js into js first              | Compiled/transpiled       |
| simpler for small projects                                  | better for large projects |

◯ Static typing :-  
Static typing means types are checked before the program runs.  

◯ Dynamic typing :-    
Dynamic typing means variable types are decided at runtime and can change later.   

◯ Diffrence between complie time and run time :-    
| compile time                       | run time                         |
| :----------------------------------: | :--------------------------------: |
| before the program runs            | while the program is running     |
| errors are found beforee execution | error happing during executation |
| e.g. - typescript type error       | e.g. - undefined error           |


◯ Diffrence between parameter and return type :-  
| parameter                 | return type                     |     
| :-------------------------: | :-------------------------------: | 
| input given to a function | output given by a function      |     
| used inside the function  | tells what the function returns |     
| e.g. - name : string      | e.g. - string                   |     

◯ Basic types of typescript :-

1. string - it represents textual values
2. number - represents numeric values
3. boolean - it represents true or false
4. null - it represents the intentional absence of a value
5. undefined - it represents an undefined value
6. bigint - it represents integers larger than the range safely represented by the number type
7. symbol - it represents unique values created using Symbol
| any                       | unknown                         |
| :-------------------------: | :-------------------------------: |
| we can store the value by string, number, boolean, array | we can store the value by string, number, boolean, array |
| we can use it without checking it | we must check the type before we use |
| it has less saftey        |                                 |
10. never - never is used for a function that does not return any value normally because it never completes successfully
11. void - void is used for a function that does not return any useful value but can complete its task successfully
12. object - it represents non-primitive values, such as objects, arrays, and functions
13. array - it specifies the type of elements that an array can contain
| array                     | tupple                          |
| :-------------------------: | :-------------------------------: |
| Elements are generally of the same type | Each position can have a specific type |
| The number of elements can change | The positions and types are defined by its structure |
| Example: number[]         |                                 |

<!-- 2 -->
◯ Function :-
parameter types - It specifies what input should be given to a function.
return types - It defines what type of value a function will return.
Optional Parameter (?) - Providing the input is optional.
Default Parameter (=) - If no input is provided, the default value is used.
Callback Function - Passing a function as an argument to another function.
Rest Parameter (...) - Collecting multiple arguments into a single parameter.
Function Expression - Storing a function in a variable.
Arrow Function (=>) - Short syntax for writing a function.

◯ Object Types :-
Object Type - Defines an object's properties and their data types.
Required Property - The property is required.
Optional Property (?) - The property is optional.
Readonly Property - The property cannot be reassigned.
Nested Object - An object inside another object.
Index Signature - Defines the type for dynamic keys.
Method - A function defined within an object.
Function Property - A function is stored as an object property.
this keyword - Refers to the current instance of an object.

<!-- 3 -->

◯ Type aliases :-
Type Alias is a way to give a custom name to a type so you can reuse it.  
A type alias is created using the type keyword.  

◯ Interface :-  
An interface defines the structure and properties that an object should have.  

◯ Diffrence between type and interface :-  
| type                                            | interface                         | 
| :-----------------------------------------------: | :---------------------------------: | 
| it uses type keyword                            | it uses interface keyword         |     
| it can define objects, unions, primitives, etc. | mainly used for object structures |      
| it cannot be reopened or merged                 | it can be extended and merged     |      

<!-- 4 -->

◯ Type composition :-  
&nbsp;&nbsp;&nbsp; Type composition means combining multiple types to create one new type.

1. Union types - 
   A Union Type in TypeScript allows a variable to accept a value of any one of two or more types using the `|` operator.
2. intersection types - 
3. litral types - 
4. narrowing types - 

<!-- 5 -->

◯ Advance types :-
1. enums - 
2. generics - 
3. Type Assertions - 
4. keyof & typeof - 
5. Mapped Types - 
   
<!-- 6 -->
◯ Utility types :-
1. partial - 
2. required - 
3. readonly - 
4. pick - 
5. omit - 
6. record - 
7. exclude - 
8. extract - 
9. nonnullable - 
10. uppercase - 
11. lower case - 
12. capitalize - 
13. uncapitaliize - 

<!-- 7 -->
classes = Properties + Constructor + Methods + access modifier

◯ properties :-

◯ construcutor :-

◯ methods :- 

◯ access modifier :-
1. public - 
2. private - 
3. protected - 

oops :-

1. inheritance - 
(i) extend - 
(ii) super - 

2. method overriding - 

3. abstaction - 


<!-- 8 -->
◯ async :-
1. Promise Types - 
2. Generic Promises - 
3. Async Functions - 
4. Async Return Types - 
5. Promise<T> - 
6. Promise Arrays - 
7. Async Error Handling - 
   
◯ error handling :-
1. error - 
2. unknown - 
3. custom errors - 
4. Error Type Guards - 
5. Result Types - 
6. Error Unions - 
   
<!-- 9    -->
