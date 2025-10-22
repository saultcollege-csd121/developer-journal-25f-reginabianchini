# Using Objects
## Thu Sep 18
### Today we are talking about the different objects and how to use them in Java


### Abstraction: to ignore irrelevant details
    - It will ignore irrelevant parts of the system and focus in only the relevant parts
### Encapsulation: when you hide implementation details 
    - It will present an abstration that is usually called 'black box' to the 'outside world'
    - clean interface = good level of abstraction
    - <abstration = not enought control
    -  >abstraction = code too complex
    -Strategy: to write the program components with clean interfaces, and then mold this components to achieve your goal
    -Object Oriented Programming (OOP) main components = objects
### Funtion Signatures:
    - function interface = signature
### Objects: 
    - State (variable), and behaviour (methods)
    - OOP are built by creating a network structure of objects that will work together. 
### Class vs Object
    - a class is the thing itself and the object will be using it.
    -Ex: class will be the 'blueprint" of a house and object will be something that was made from the blueprint
    - Objects can be from the same class meaning that all will have the same behaviour
    - However, they can also have different classes for each object
    Object of different classes have different state and behaviour
### Single Responsibility Principle:
    - Each class has a single responsability

### Object Terminology: 
    - State = Intance variable, field, property, attribute
    - Behaviour = method
    - methods and instance varibles = members

### Class Interfaces: 
    - Public Interface = 
    -Private members = encapsulated so they are hidden

## Tue Sep 23
### Continuation of class about objects 

- Acessor and mutator methods:
    - mutator method change state of object 
        - Ex: House house = new House();
              house.openDoor(); 
    - Accessor method refer to instance but it doesn't change it 
        - boolean open = house.getIsDoorOpen();
        - Contains an object with accessing a variable information, accessing specific class variables, and functions associated with the specific instance. A good example of a class doesn't have any in math class attaching a bunch of variables and functions we don't have to do any. 
### Class vs Instance Variables
    - Class variables = type in general 
    - it uses the class name to refer in the code, like Math.PI
    - Used to store values that are common to all instance of a class
    -Call using class name, as in Math.sqrt(25)
    - Can't access instance variables

    - Instance varibles = one object instance of a class
    - it will store the internal state of an object instance 
    - call using object references, as in house.openDoor()
    -Can access instance variables 

### What kind of thing am I looking at ?
    - Consider the case pattern of the name...

    Case patter                         Means you're looking at a...
    ALL_CAPS                                Constant
    startsWithLowerCase                     Variable or function/method name
    StartsWithUpperCase                     Type(Class,interface,record,enum,etc) name

    - Consider the context of the name...

    Context                              Means you're looking at a...
    new TypeName(..)                        Constructor call
    TypeName.noParens                       Class variable (noParens) on TypeName
    TypeName.parens(..)                     Class method (parens) on TypeName
    varName.noParens                        Instance variable (noParens) of object (varName)
    varName.parens(..)                      Instance method (parens) of object (varName)

 ### Member visibility: 
- public or private
- public can be used anywhere 
- Private can only be used from inside the same class as the member

### System.out
- java class with public class variable named 'out'
is an object of type PrintStream
 ### Method overload:
 - when a class has multiple methods with the same name but different set of parameters 
 - necessary so statically typed languages can handle various types

 ### Review
 - Objects created using new keyword with constructor method call
 - An object encapsulates state(variables) and behaviour (methods)
    - Collective, variables/methods are callled members - Members are accessed by using the dot operator
- Variables storing objects are references
- Different kinds of objects are defined using classes
- Class members are associated with a class
    - Class members can be accessed via class; no object instance is required
    - Class variables are the same for every object instsnce of that class
- Instance members are associated with individual object instances
    - Instance members must be accessed via an object
    - Instance variables may differ for each object
- In java the static keyword determines if a member is an instance member or a class member

