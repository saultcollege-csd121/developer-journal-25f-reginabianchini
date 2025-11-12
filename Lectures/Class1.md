# Introcution to Java
## Thurs Sep 11
### Today we are starting to talk about Java

- Java is a hybrid language
    - Hybrid language means that the compiler converts Java code files into Java bytecodes

- Java vs JavaScript
    - Not the same language
    - Same name just for marketing nothing else

- Java Development Kit (JDK)
    - JVM need to be installed to be able to run Java
    - JDK is needed if you want to create Java programs
    - JVM = java
    - Compiler = javac
    - REPL shell = jshell

- Java Syntax
    - Syntax errors will happen when you break the grammatical rules
    - Syntax errors are detected by the compiler in a compiled language (compile-time errors)
    - Java is case sensitive
    - Instructions end in semi-colons
    - Code blocks are wrapped in curly braces
    - Indention doesn't matter (different from Python)
    - Comments: // (this is a one line comment)
                /*     */ (this is a multi-line comment)

- Values
    - Value is data that can be represented by a program
    - May be assigned to variables

- Static vs Dinamic typing 
    - Java is a statically typed language ( Java variables must be given a type in code)
        - Ex: x = 42; (wrong)
              int x = 42; (ok)
    - Python is a dinamically typed language

- Static typing
    - values assigned to variables must correspond to their types

- Declaration and assignment
    - varible declaration and assignment may be separate ( variable type only necessary on declaration)

- Variable assignment:
    - It is a statement, not mathematical equality

- Type inference:
    - var can be used instead of a variable type
    - only if variable is initialized to a value when it isdeclared
    - Compiler infers type from value assigned to variable

- Variable names: 
    - Alphabetical symbols
    - Numbers (but don't start with a number)
    - Underscore 
    - Keywords can't be used as variable names
    - You should use : Lower-case first letter and Upper-case first letter of each subsequent word

- Types: 
     - Primitive types
     - Object types

- Primitive types: 
    - pure values (boolean, byte, short, int, long, float, double, char)
    - have no methods
    - Primitive names all start with lowercase letter

- Object Types: 
    - Everything that is not one of the 8 primitive types are object type
    - they store a reference to the location where the actual data is stored
    - they may be composite
    - Object types names start with uppercase letter 

- Array
    - They are ordered collection of values
    - All elements must be the same type
    - Only one built in property : length
    - Fixed lenght
    - Array literal uses curly braces
    - Squre brackets intype declaration 
    - Index using [i] syntax
    - Is a reference (object) type
    - Ex: int[]myArray = {1,2,3};
          myArray.lenght;

- Creating Java Programs
    - Most people use IDE but they can also run in another way

- Classes: 
    - Object types are defined using classes
    - You can define your own class or use one that is already predefined for you
    - Every code file must be a class
    - IMPORTANT: name of the file must be the same as name of class
    - the public keyword indicates the 'visibility' of the class

- Function definition statments 
    - set of instructions may be created using a fucntion definition statement 
    - Functions may be called to execute the set of instructions 
    - Functions may return a value
    - Arguments may be used to provide input values to a function ( they are assigned to local variables called parameters)

- Functions
    - Functions must belong to a class
    - Class method: associated with the class and call from class name
    - Instance methods: Associated with an instance of the class, and call from object reference 

- Class method: 
    - May be called instance methods
    
- Functions: 
    - Functions definition must specify: visibility, binding, return type, name, type and name of each parameter 

    - Ex: public class MyApp {
        public static void greet(String name) {
            System.out.println("Hello, " + name);
        }
    }

- Functions (class methods)
    - Visibility: 
        - public: function can be called from the outside of class
        - Private: function can't be accesed from the outside, it needs to be inside the class
    - Binding: 
        - static - function is a class method
        - non-static - function is an instance method
    - Return type: specify the type of the value returned from the function
        - Use void if function does not return a value
    - Function name: 
        - Function names start with lowercase letter
    - Parameter list: 
        - each parameter must have a type and a name
        - Separate it with a comma
    - Print to console:
        - Equivalent to print in python
    
- Program Execution: 
    - begins with the main class method in the executed bytecode file
    - main method receives argument as an array of String objects

- Static typing: 
    - Allows the compiler to catch an entire category of bugs before you run the program
    - Force you to fix type errors 
    - Better for large software projects
    - Dinamically typed language allow you to 'ignore' types
    - More appropriate for prototyping and smaller software projects

- static == compile-time; dinamic == run-time
    - static: refer to things that are determined at compile-time
    - dynamic: refer to aspects that are determined at run-time

- Errors: 
    - Compile-time errors: errors caught during compilation, syntax and type errors are compile-time errors
        - Often indicated by IDE before compilation
        - prevent code from being compiled
        - Ex: Syntax errors
    - Run-time errors: Errors that occur while the program is running
        - Happen when the program is running 
        - Cause program to end  
        - Ex: file not found, invalid permission
    - Semantic / logic errors: Errors in program logic / behaviour
        - Cause unexpected/ incorrect program behaviour
        - Usually don't cause program to crash
        - Caused by incorrect logic in program

## Summary: In this class we learned the basic of Java and how it is a static language. We also learned a little bit about the structure, how it starts with main. We also talked about the different types of errors that can occur in a java program. We defined what is a static function and a public and private one too. We talked about objects. 

