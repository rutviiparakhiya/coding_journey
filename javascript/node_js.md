NODE JS

Node_js is not a framework.
it is a JavaScript runtime environment that allows JavaScript to run outside the browser
Every Node.js file is a module
Modules prevent global scope pollution
npm manages third-party libraries
Every request triggers a callback
Requests and responses are event-driven
Node.js handles concurrency using non-blocking I/O
Frameworks exist to simplify routing and structure
REST is an architectural style, not a framework
HTTP methods define actions
Statelessness enables scalability
Express is built on Node’s HTTP module
express simplifies routing and responses
Middleware runs in order
next() is mandatory to continue
Middleware can end requests
express.json() must come before routes






#_what is module ?
Every file is a module
Each module has its own scope
Variables are not global by default

#_types of modules in node_js ?
1. core module : it builds directly into nodejs
2. local module : it is create inside your project
3. third party module : Modules created by others and shared via npm

dependencies : Required for the app to run
devDependencies : Required during development

#_what rest defines and what not?
defines :  how APIs should behave, not how they are built internally

not define :    How authentication is implemented
                How data is stored
                Which programming language to use
                Which framework to use


#_express_js : it is a web framework built on top of Node.js
    when we use it : building rest api, want middleware support, need scalable backend strucutre

#_middleware : it is a function that runs before the final route handler 
Middleware uses a function called next() -> to move to the next middleware or route or request stops