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