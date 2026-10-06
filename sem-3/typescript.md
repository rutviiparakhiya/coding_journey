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

◯ Type composition :-  
&nbsp;&nbsp;&nbsp; Type composition means combining multiple types to create one new type.

&nbsp;&nbsp;&nbsp; 1. Union types : Union type allows a value to have one of multiple types using the | operator.  

&nbsp;&nbsp;&nbsp; 2. Intersection type : Intersection type combines all properties of multiple types using the & operator.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (i) object intersection - it combines the properties of two or more object types using &.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (ii) interface intersection - it combines two or more interfaces using &.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (iii) intersection conflicts - it happens when two types have the same property with different types.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (iv) combining types - it means joining two or more types using & or |.

&nbsp;&nbsp;&nbsp; 3. Literal types : it allows a variable to have a specific fixed value.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (i) string literals - it means a type that allows only specific string values.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (ii) 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 