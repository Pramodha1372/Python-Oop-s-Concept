# Python-Oops-Concept

+ Python is a multi-paradigm programming language.
    1. Procedure-oriented programming (POP) - main emphasis is on functions
    2. Object-oriented programming (OOP) - stress on objects
    
+ One of the popular approaches to solve a programming problem is by creating objects. 
+ This is known as OOP.
+ The concept of OOP in Python focuses on creating reusable code. 
+ This concept is also known as DRY (Don't Repeat Yourself).
+ Object is simply a collection of data (variables) and methods (functions) that act on those data.
+ Class is a blueprint for the object.
+ An object is also called an instance of a class.
+ The process of creating this object is called instantiation.
+ Object-oriented programming (OOP) involves the use of objects to create programs.
+ An object represents an entity in the real world that can be distinctly identified.
+ Python automatically assigns each object a unique id for identifying the object at runtime.
+ An object’s state (also known as its properties or attributes) is represented by variables, called data fields.
+ Python uses methods to define an object’s behavior (also known as its actions).
+ A Python class uses variables to store data fields and defines methods to perform actions.
+ A class is a contract—also sometimes called a template or blueprint—that defines what an object’s data fields and methods will be.
+ The self parameter is a reference to the current instance of the class, and is used to access variables,methods that belongs to the class.
+ It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class.
+ Whenever an object calls its method, the object itself is passed as the first argument. So, c1.getArea() translates into Circle.getArea(c1).
+ the first argument of the function in class must be the object itself. This is conventionally called self. It can be named otherwise but we highly recommend to follow the convention.
+ All classes have a function called init(), which is always executed when the class is being initiated.
+ Use the init() function to assign values to object properties, or other operations that are necessary to do when the object is being created.
+ Class functions that begins with double underscore (__) are called special functions as they have special meaning.
+ Of one particular interest is the __init__() function. This special function gets called whenever a new object of that class is instantiated. This type of function is also called constructors in OOP. We normally use it to initialize all the variables.

+ **Types of constructors** :

    1. default constructor: The default constructor is a simple constructor which doesn’t accept any arguments. Its definition has only one argument which is a reference to the instance being constructed.

    2. parameterized constructor: constructor with parameters is known as parameterized constructor. The parameterized constructor takes its first argument as a reference to the instance being constructed known as self and the rest of the arguments are provided by the programmer.
+ Any attribute of an object can be deleted anytime, using the del statement.
+ When we do cobj = Complex(1,3), a new instance object is created in memory and the name cobj binds with it.
+ On the command del cobj, this binding is removed and the name cobj is deleted from the corresponding namespace. The object however continues to exist in memory and if no other name is bound to it, it is later automatically destroyed.
+ This automatic destruction of unreferenced objects in Python is also called garbage collection.

**Types of variables and methods**

1. In Python, a static variable is a variable that is shared among all instances of a class, rather than being unique to each instance. It is also sometimes referred to as a class variable, because it belongs to the class itself rather than any particular instance of the class.
+ Static variables are defined inside the class definition, but outside of any method definitions. They are typically initialized with a value, just like an instance variable, but they can be accessed and modified through the class itself, rather than through an instance.

2. Instance Varibales are those attributes that are not shared by objects. Every object has its own copy of the instance attribute i.e. for every object, instance attribute is different.
+ Within the class by using self and object reference.

+ static/class var can be accessed using objects as well as class names but instance variables can be accessed using only objects.

**Instance, Class and Static Methods**
1. Instance method are methods which require an object of its class to be created before it can be called. 
+ To invoke a instance method, we have to create an Object of the class in which the method is defined.
2. A class method is a method that is bound to the class and not the object of the class. 
+ They have the access to the state of the class as it takes a class parameter that points to the class and not the object instance. 
+ It can modify a class state that would apply across all the instances of the class.
3. A static method is a method that belongs to a class rather than an instance of a class. 
+ This means you can call a static method without creating an object of the class. 
+ Static methods are sometimes called class methods.

**Instance methods need a class instance and can access the instance through self . Class methods don't need a class instance. They can't access the instance ( self ) but they have access to the class itself via cls . Static methods don't have access to cls or self .**

**INHERITENCE**

+ Aquiring all the properties and bahaviuors of one class to another class.
+ It is a mechanism that allows you to create a hierarchy of classes that share a set of properties and methods by deriving a class from another class. 
+ Inheritance is the capability of one class to derive or inherit the properties from another class.

*TYPES :*
1. Single level
2. Multi level
3. Multiple
4. Hybrid
5. Hierarchical

**Super class**

+ In Python, the super() function is used to refer to the parent class or superclass. It allows you to call methods defined in the superclass from the subclass, enabling you to extend and customize the functionality inherited from the parent class.

**POLYMORPHISM**

- Poly means many
 - Morpgh - forms
 - Polymorphism refers to bahaving the same function or operator differently base on situations or one function can have multiple characterstics for example Human can play different character like son, husband, student, teacher and so on
*Types - Method overloading and Operator over loading*

**Operator Overloading**

+ Operator Overloading means giving extended meaning beyond their predefined operational meaning. For example operator + is used to add two integers as well as join two strings and merge two lists. It is achievable because ‘+’ operator is overloaded by int class and str class. You might have noticed that the same built-in operator or function shows different behavior for objects of different classes, this is called Operator Overloading

**Method Overloading**

+ Method Overloading is an example of Compile time polymorphism. In this, more than one method of the same class shares the same method name having different signatures. Method overloading is used to add more to the behavior of methods and there is no need of more than one class for method overloading.

*Note* : Python does not support method overloading. We may overload the methods but can only use the latest defined method.

**Method Overriding**

+ Method overriding, on the other hand, refers to defining a method in a subclass with the same name as the one in its superclass. The subclass method then overrides the superclass method.

**ENCAPSULATION**

+ Process of restricting the object to change some data is called Encapsulation
+ And It is a process of encapulating data and methods and work on the same data.
+ To restict the data, we have to create private variable and methods
+ To create private variable we have to use __ (double underscore)
+ private variables --- keep a __ before the variable
+ we can change the values of private variables outside(by calling an object) it will not give error but when we access the same private variables with other methods in the class, the value will still remains same(the new changes wont be reflected).

**ABSTRACTION**

- Hiding complex information and show only neccesary information is abstraction
- For example, TV remote or send sms to friends

**ENCAPSULATION** - It describes the idea of wrapping data and the methods that work on data within one unit. 

**ABSTRACTION** - It is defined as a process of handling complexity by hiding unnecessary information from the user.

**DATA HIDING** - It is a concept which underlines the hiding of data or information from the user.
