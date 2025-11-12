# Implementing Types
## Thu Sep 25
### We started learning about Implementing Types in Java

- Enumerations: way to represent types that can have one of a pre-defined set of values 
    - sometimes a type can be only one of a limited set of values
    - Ex: Yes/No/maybe/ status
    - Using strings to represent the possible values works but is prone to typos that cause run-time errors
    - use enums instead is way better
    - Ex: enum Answer {Yes, No, Maybe}
    - Enums can be used as a type ( the compiler will catch type errors in addition to typos)
- Records: a way to represent types that consist of multiple parts
    - Records are immutable
    - Contructor with the same arguments as its properties
    - Automatic .equals, .toString, and .hashCode methods
    - Any time that you need to store a multi-part value that is not a collection like list or map just use record instead of class

- Object Oriented Programming (OOP): 
    - Build programs out of objects 
    - each object groups related state and behaviour around a single theme
    - class defines one kind of object
    - each class has a single responsability, presents clean abstraction and encapsulates implementation details

- Class example - Stopwatch: 
    - instance/class variables always declared directly inside class scope. You can't declare instance/class variables inside a method
    - Convention: methods come after variables in a class definition
    - Responsability: Track a time interval 
    - Abstraction (public interface):
        - start()
        - stop()
        - getElapsedTime()
    - Encapsulation ( private members)
        - uses System.getCurrentTimeMilis() to track time

- Accessor vs Mutator methods: 
    - Accessor method: return the vaulue of an instance variable
    - Mutator method: changes the values of an instance variable

- Common OOP Pattern: 
    - Make all instance variable private
    - Provide public accessors (getters)
    - provide public mutators (setters)
    - So implementation can be changed without changing public interface
    - Ex; getter = 'getFoo'
          setter = 'setFoo'

- The 'this' keyword: 
    - inside class definition the this keyword can be used to refer to the object on which a method was called 
    - refers to the current object because count is an instance variable

- Constructor: 
    - method that initializes an object instance of a class 
    - always have the same name as the class
    - usually public
    - no return
    - may be overloaded to provide multiple ways to construct an object
    - no-parameter constructor sets count to 0 by default
    - java will automatically insert a no-parameter constructor if no constructor is defined
    - Common errors: forgeting to initialize instance variables

- Calling Constructors from constructors:
    - Sometimes is something that is useful to do

- Variable scope:
    - scoping rules apply for variables used in a class definition
    - variables are accessible anywhere inside the block in which they are declared

- Shadowing (common error):
    - occours when a variable name in a narrower scope is the same as that of one in a wider scope

- Deciding variable scope: 
    - keep the scope of a variable as narrow as possible

## Summary: 
- Classes can be used to define custom types in OOP code
- Objects are created using the constructor of a class
- constructors may be overloaded; if no constructor is defined on a class, the JDK automatically adds a no-parameter constructor
- Instance methods may access the value of the instance variables for a specific object of a class using the 'this' keyword
- enums are useful for representing a type that has a specific limited set of values
- records are useful for representing immutable, multi-part values 

- Instance variables may be used inside any instance method, but local variables may only be used inside the method they are declared in - True

- Two object of the same class have the same instnce variables, but may have different values in those variables - true

- The fact that you can call the System.out.prinln() function without knowing the code for the println frunction is an example of encapsulation - true
