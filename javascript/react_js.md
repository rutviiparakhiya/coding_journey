REACT JS

#_Real DOM :-
it is the actual browser document object model that represents the ui structure
(updates are slow and expensive)

#_Virtual DOM :-
it is a light weight js representation of the real dom maintain by REACT
(updates are fast and efficient)

#_Real DOM vs Virtual DOM :-

    aspect  +            real dom             +         virtual dom 
------------|---------------------------------|-------------------------------
  updates   |slow(direct browser manipulation)|fast(in-memory operations)
  memory    |creates new dom nodes            |reuses existing objects
manipulation|direct manipulation              | it updates
rerendering |full rerendering                 |selective updates via diffing
 perfomance |expensive operations             |optimizing batching

-> when to use better :

            building static pages             |building complex, dynamic ui's 
            working non-react projects        |working large scale applications

#_map :-
it takes each item from an (old) array, does somthing to it and returns a new array with the results

#_Components :-
it is reusable piecies used to build the ui

#_Props :- (data passed from parent to child)
props are inputs that control how a component looks or behaves

- it is read-only (cannot be changed)
- it helps to send data or functions
- data flows one way : parent -> child

#_props drilling :-
passing data through many components

parent - child - grandchild - greatgrand child

#_Use State :-
it is used to store data in component and to be update the data

#_Use Effect :-
it runs extra code after component renders
it is used for : - Fetching data (API)
                 - Changing page title
                 - Adding event listeners
                 - Running animations           

#_react-lifecycle :-
React Lifecycle = stages of a component’s life
    1. Mounting → Component is created and shown on screen

    2. Updating → Component updates when data (state/props) changes

    3. Unmounting → Component is removed from screen

#_Class based components :-
Class Component = component made using a class (It uses render() method to show UI)

#_Function Components :-
A function component is a JavaScript function that returns JSX to show UI and can take data using props.

#_What is react context :-
Context API = global data share karva mate

#_Use Context :-
useContext = get global data in any component without prop drilling

#_Use Memo :-
it saves a calculated value and only recalculate if needed (optimize performance by remembering values)

    Why we use :
    - Re-run any calculations inside the component

#_Use CallBack :- (React hook)
it saves a function so it doesn’t change on every render

    Why we use :
    - Re-create functions inside the component

#_Use Ref :-
it stores a value or DOM element without re-render

    Why we use :
    1. Accessing the DOM directly
    2. Storing a mutable value that persists across renders
    3. Avoiding unnecessary re-renders by not storing frequently updated values in the state

#_Use Reducer :-
it manage complex state like useState

    Why we use :
    1. Handles Complex State
    2. Improves Readability
    3. Predictable State Updates

#_Custom Hooks :-
it is a reusable function using React hooks

    Why we use :
    1. reusability
    2. Separation of Concerns (it helps organize code by separating logic from UI)
    3. Simplifying Complex Components (it simplifies components by handling logic separately)
    4. Abstraction of Reusable Logic (it hides complexity and make components simple)

#_React router dom :-

#_Event loop :-
it decides the order of running code, including async tasks
- JavaScript is single-threaded, so the event loop lets it run async tasks without blocking other code

#_Async await :-
it is easier, readable way to handle asynchronous tasks

#_Promises :-
it manages async code in an organized way

    it has three stages :
    1. Pending: The operation is still ongoing
    2. Resolved: The operation completed successfully
    3. Rejected: The operation failed

#_CallBack :-
function passed to run after a task finishes

#_Redux :-
it was centralized state manager for JavaScript apps

    Why we use : 
    1. Prop drilling: no need to pass state through many components
    2. Complex state: easy to manage multiple states
    3. Debugging: track state changes easily

    When to use :
    1. Large app with shared state
    2. Need state persistence
    3. Want predictable state updates

    Principles :
    1. Single Source of Truth → All app state is in one store
    2. State is Read-Only → Change state only via actions
    3. Changes with Pure Functions → Reducers define how state updates

    Core concepts :
    1. Store → Holds the entire app state in one place
    2. Actions → Objects that describe what to do 
    3. Reducers → Pure functions that define how state changes
    4. Dispatch → Sends an action to the reducer

    middleware :
    it manages async operations in Redux easily              
    - Lets you do API calls or async work before reaching reducers
    - Examples: Redux Thunk, Redux Toolkit

#_Redux Toolkit :-
it is Redux Toolkit (RTK)
Redux Toolkit simplifies Redux setup

    Why we use : 
    1. Less boilerplate: no separate action creators/reducers
    2. Better performance: uses Immer.js for state updates
    3. Async handling: createAsyncThunk for API calls
    4. Middleware integration: works well with redux-thunk

    createAsyncThunk : 
    it handles API calls in Redux easily

    RTK Query :
    it makes easy to data fetching and caching in Redux Toolkit
    - it makes API calls, caching, and updates automatic in Redux 

#_Template :-
it is a keyword to reuse the piece of code for a several data types

#_routing : 
it is a process of navigating between different pages in a web application
static route - users-> named folder
dynamic route - user/[id] -> dynamic folder inside pages folder