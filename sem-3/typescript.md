◯ Type Script (TypeScript = JavaScript + Types)   

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;It is an extended version of JavaScript that adds types, making the code easier and safer to write.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TypeScript adds types to JavaScript and is converted into JavaScript before running.  

◯ Diffrence between js and ts :- 
| js                                                          | ts                        |
| :-----------------------------------------------------------: | :-------------------------: |
| Dynamically typed                                           | Statically typed          |
| Types are checked at runtime                                | Types are checked at compile time |
| Runs directly in browser                                    | transpiled into js before running |
| simpler for small projects                                  | better for large projects |

◯ Static typing :-  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Static typing means types are checked before the program runs.  

◯ Dynamic typing :-    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dynamic typing means variable types are decided at runtime and can change later.   

◯ Diffrence between compile time and run time :-    
| compile time                       | run time                         |
| :----------------------------------: | :--------------------------------: |
| checks an error before the program runs | checks an error while the program is running |
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

10.  never - never is used for a function that does not return any value normally because it never completes successfully  
11.  void - void is used for a function that does not return any useful value but can complete its task successfully  
12.  object - it represents non-primitive values, such as objects, arrays, and functions  
13.  array - it specifies the type of elements that an array can contain  

| array                     | tupple                          |
| :-------------------------: | :-------------------------------: |
| Elements are generally of the same type | Each position can have a specific type |
| The number of elements can change | The positions and types are defined by its structure |
| Example: number[]         |                                 |

<!-- 2 -->
◯ Function :-  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;parameter types - It specifies what input should be given to a function.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return types - It defines what type of value a function will return.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Optional Parameter (?) - Providing the input is optional.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default Parameter (=) - If no input is provided, the default value is used.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Callback Function - Passing a function as an argument to another function.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rest Parameter (...) - Collecting multiple arguments into a single parameter.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Function Expression - Storing a function in a variable.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Arrow Function (=>) - Short syntax for writing a function.  

◯ Object Types :-
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Object Type - Defines an object's properties and their data types.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Required Property - The property is required.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Optional Property (?) - The property is optional.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Readonly Property - The property cannot be reassigned.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Nested Object - An object inside another object.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Index Signature - Defines the type for dynamic keys.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Method - A function defined within an object.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Function Property - A function is stored as an object property.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this keyword - Refers to the current instance of an object.  

<!-- 3 -->

◯ Type aliases :- Type Alias is a way to give a custom name to a type so you can reuse it.   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; → A type alias is created using the type keyword.   

◯ Interface :-  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;An interface defines the structure and properties that an object should have.  

◯ Diffrence between type and interface :-  
| type                                            | interface                         | 
| :-----------------------------------------------: | :---------------------------------: | 
| it uses type keyword                            | it uses interface keyword         |     
| it can define objects, unions, primitives, etc. | mainly used for object structures |      
| it cannot be reopened or merged                 | it can be extended and merged     |      

<!-- 4 -->

◯ Type composition :-  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Type composition means combining multiple types to create one new type.

1. Union types - A Union Type in TypeScript allows a variable to accept a value of any one of two or more types using the | operator.  
(i) primitive union - it allows a variable to accept values of two or more primitive types, such as string, number, or boolean.  
(ii) multiple union - it allows a variable to accept values of three or more types using the | operator.  
(iii) litral union - it allows a variable to accept only specific, predefined values.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -> it only allows 3 values - pending, success, error (if we assigned failed, an error occurs)  

1. intersection types - In TypeScript, an Intersection Type combines all properties of two or more types using the & operator to create a new &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; type.  
there are four usecases of intersection :   
(i) object intersection - Object Intersection means combining all the properties of two objects into a single type using the & operator.  
(ii) interface intersection - Interface Intersection means combining all the properties of two or more interfaces into one type using the & &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; operator.  
(iii) intersction confilcts - Intersection Conflict occurs when two types have the same property but different data types.  
(iv) combinig types - it means creating a specific type using both Union (|) and Intersection & operators.  

1. litral types - Allow only a specific, exact value instead of a broad type.  
there are main 5 concepts of litral types :  
(i) string litral - Allow only specified string values.  
(ii) Number Literals - Allow only specified numeric values.  
(iii) Boolean Literals - Allow only the exact value true or false.  
(iv) Const Assertions (as const) - Preserve exact literal values and make object properties and arrays readonly.  
(v) Literal Unions - Combine multiple literal values using | to allow only those specified values.  

1. narrowing types - The process of reducing a broad type to a more specific type using checks.  
there are 9 main concepts of narrowing :   
(i) typeof - Checks the type of a value using the typeof operator.   
(ii) instanceof - Checks whether an object belongs to a specific class.   
(iii) in operator - Checks whether an object contains a specific property.   
(iv) Equality Narrowing - Uses === or !== comparisons to narrow a type.   
(v) Truthiness Narrowing - Uses conditions like if (value) to narrow a type based on truthiness.   
(vi) Assignment Narrowing - TypeScript determines the current type of a variable after assigning a value.   
(vii) Control-Flow Analysis - TypeScript determines the current type by analyzing conditions, branches, and assignments.   
(viii) Discriminated Unions - Uses a common property to identify a specific type within a union.   
(ix) Exhaustiveness Checking - Ensures that all possible cases of a union are handled.   

<!-- 5 -->

◯ Advance types :-
1. enums - Enum means grouping predefined options under named constants in one place.
2. generics - it means allowing the same function or code to work with different data types while maintaining type safety.
3. Type Assertions - it tells the compiler to treat a value as a specific type without changing the actual value. 
4. keyof & typeof - keyof Creates a union of all property keys of a type & typeof Gets the type of an existing variable or value.
5. Mapped Types - it creates a new type by transforming the properties of an existing type.

<!-- 6 -->
◯ Utility types :- Utility types are built-in generic types provided by TypeScript for transforming existing types, They allow common type &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; transformations without manually defining a new type each time.

1. partial - it Makes all properties optional in a type.
2. required - it Makes all properties required in a type.
3. readonly - it Prevents all properties from being changed.
4. pick - Selects specific properties from a type.
5. omit - Removes specific properties from a type.
6. record - Creates an object type with specified keys and value types.
7. exclude - Removes specified types from a union.
8. extract - Keeps only specified types from a union.
9. nonnullable - Removes null and undefined from a type.
10. uppercase - Converts a string literal type to uppercase.
11. lower case - Lowercase: Converts a string literal type to lowercase.
12. capitalize - Converts the first character of a string literal type to uppercase.
13. uncapitaliize - Converts the first character of a string literal type to lowercase.

<!-- 7 -->
◯ classes :- Properties + Constructor + Methods + access modifier  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A blueprint for creating objects that contain data and methods.  
1. properties :- Stores data in a class.   
2. constructor :- A special method that initializes an object when it is created.  
3. methods :- A function defined inside a class.  
4. access modifier :- public(by default), private, protected  

◯ oops :-
1. inheritance - Allows one class to reuse and extend another class.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(i) extend - Allows a child class to inherit from a parent class.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(ii) super - Used to access the parent class's constructor and methods.  

2. method overriding - Allows a child class to provide its own implementation of a parent class method.

3. abstaction - Hides implementation details and defines what a class must provide.


<!-- 8 -->
◯ async :- Allows code to handle tasks that take time without blocking other operations.

1. Promise Types - Specifies the type of value a promise will return.
2. Generic Promises - Specifies the type of value a promise resolves to using Promise<T>.
3. Async Functions - Functions that always return a promise.
4. Async Return Types - Specifies the promise type returned by an async function.
5. Promise<T> - Represents a promise that resolves to a value of type T.
6. Promise Arrays - An array that stores multiple promises of a specified type.
7. Async Error Handling - Handles errors in asynchronous operations using try...catch.
   
◯ error handling :-
1. error - An object that represents a runtime error and provides details about it.
2. unknown - Treats caught errors as unknown until their type is checked.
3. custom errors - User-defined errors created by extending the built-in Error class.
4. Error Type Guards - Checks the error type before using its specific properties.
5. Result Types - Represents either a successful result or an error result.
6. Error Unions - Combines different error types into one union type.
   
<!-- 9 -->
