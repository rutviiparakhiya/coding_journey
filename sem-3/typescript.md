Type Script (TypeScript = JavaScript + Types)
It is an extended version of JavaScript that adds types, making the code easier and safer to write.
TypeScript adds types to JavaScript and is converted into JavaScript before running.

diffrence between js and ts :-

| js                                                          | ts                        |
| :-----------------------------------------------------------: | :-------------------------: |
| Dynamically typed                                           | Statically typed          |
| Types are checked at runtime during development/compilation | Types are checked         |
| Runs directly in browser/Node.js into js first              | Compiled/transpiled       |
| simpler for small projects                                  | better for large projects |




js                                 |ts
------------------------------------------------------------------------------------
Dynamically typed                  |Statically typed
Types are checked at runtime       |Types are checked during development/compilation
Runs directly in browser/Node.js   |Compiled/transpiled into JavaScript first
Simpler for small projects         |Better for large projects

static typing :-
Static typing means types are checked before the program runs.

dynamic typing :-
Dynamic typing means variable types are decided at runtime and can change later.

diffrence between complie time and run time :-

compile time                        |Run Time
-------------------------------------------------------------------
Before the program runs             |While the program is running
Errors are found before execution   |Errors happen during execution
Example: TypeScript type errors     |Example: undefined error

diffrence between parameter and return type :-

Parameter                     |Return Type
----------------------------------------------------------------
Input given to a function     |Output given by a function
Used inside the function      |Tells what the function returns
Example: name: string         |Example: : string

type aliases :-
Type Alias is a way to give a custom name to a type so you can reuse it.
A type alias is created using the type keyword.

interface :-
An interface defines the structure and properties that an object should have.

diffrence type and interface :-

type                                           |interface
---------------------------------------------------------------------------------
Uses type keyword                              |Uses interface keyword
Can define objects, unions, primitives, etc.   |Mainly used for object structures
Cannot be reopened/merged                      |Can be extended and merged

