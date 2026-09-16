oops(object orianeted programing) :-

where object is entity(real world problem)
entity :- exstis, space occupy, character, functioanlity

-> opps is a platfrom independent laungage.

#_keywords :-
1.this : It refers to the current execution context.

2.static: It is a variable that stays in memory until the program terminates and remembers its previous value.

3.friend : It is use specially when we want to access the private or a protced member of a particular class via through a function which is define outside that class.

4.virtual : It is a function in a base class that can be changed (overridden) in a derived class and is called at runtime using the virtual keyword.

#_class :- 
It is a blueprint/skeleton of object(object -> particular entity)
-> and it is a "keyword" to define a members(data members, function members)
-> it not consume any space(memory)

#_object :-
An object is an instance of a class that represents a real-world entity and stores its own data.

#_constructure :- 
It is used to initialize of the value to a particular object members during object creation
->there are 2 types : 1.default, 2. parametarized 

1. default - It is a special function that automatically initializes an object when it is created.

2. parametarized - If the base class has a parameterized constructor, the derived class must call it and pass the required parameters

#_Destructre :-
It is a kind of function but get call automatically by c++ compiler when a particular object is about to get destroy because of the block scope.

#_inheritance :- 
It is used to create a child class from a parent class, where common properties are in the parent class and distinct properties are in the child class.
    
    1. single_inheritance : It is used to make a clidren class.

    2. multilevel_inheritance : It is when a class inherits from another derived (child) class.

    3. multiple_inheritance : It is when a class inherits properties from more than one base (parent) class

        (i)same-method : Same method means two or more functions have the same name but different parameters
        (ii)constructre : A constructor is a special function of a class that runs automatically when an object is created.

    4. hirarical_inheritance : It means multiple derived (child) classes inherit from a single base (parent) class.

    5. hybrid_inheritance : It combines two or more types of inheritance in one program.

#Pass by value :-
It the function gets a copy of the variable, not the original one.
-> So if the function changes the value, it only changes the copy, and the original variable stays the same

#Pass by refrence :-
It means the function gets the actual variable’s address, not a copy
-> So when the function changes the value, it changes the original variable directly

#Static-members :-
Static Members are variables or functions that belong to the class, not to individual objects.
-> This means all objects of the class share the same static member

    there are 2 types of static members : 1.static-variable, 2.static-function

        1.static-variable  - A static variable is a variable that is shared by all objects of a class and belongs to the class, not to a single object

        2.static-function - A static function is a function that belongs to the class, not to an object. It can only use static variables and static functions and can be called using the class name without creating an object

#_virtual :-
It is a function in a base class that can be changed (overridden) in a derived class and is called at runtime using the virtual keyword

#Access-modifire :-
It is a way through which you can provide the level of accessibilty for a security concerns to a particular class members upto which level it can be accessed.

types : 1.public, 2.private, 3.protected

    1.public - It can be acces anywhere

    2.private - It is only use to the particular class not outside the class
    ->private is type of acces modifer which is use for providing to accessibilty to a particular class members and the level of accessibilty

    3.protected - It comes with flexibility (To use a class, it must become a child class in order to access it)
    ->the same rule must be follow by the childern class of that pervious of actual class

#_Friend Function :- (we can access it outside any function)
A friend function is not a member of the class, but it can access the class's private and protected members because the class declares it as a friend.

#_Friend class :- (It can be used in the class where it is declared without any errors.)
It is a class that can access the private and protected members of another class because it has been declared as a friend.

#_Encapsulation :- Encapsulation means wrapping data and functions into one class.

#_Abstraction :- Hide complexity and show only neccesary things.

#_polymorphism :- Polymorphism means one name, many forms.
                  It allows the same function to behave differently.
(many+form) 

    1. Compile time polymorphism - 
        (i)function_overloading : (same function member) (same class)
        (ii)operator_overloading : (using same operator) (concating)

    2. Run time polymorphism - A no. of function members which was define in a base class but it get overwrite by it's own derived(child) class but with some changes. 

                             - it is used to impliment "function overloading" concept
                             to implement "function overriding that the number of function must be defined already inside the parent class which will be overrider by it's own children

                             - but in child class in order to "override" the alreday defined function members inside parent classs -> write same function name, same parameter and same datatype