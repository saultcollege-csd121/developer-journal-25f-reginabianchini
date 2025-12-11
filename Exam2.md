# Exam 2 
## Tue Dec 9

- creating a class hyerarqui based on a description, not a lot of code just basic structure. 

- Look for description of a text and describe it. 

- What makes an interface different from an class

- He will give some code that is a method with a dependency


- abstraction: ignoring irrelevant details to focus on essential features

-  Encapsulation: hiding implementation details
    - visiability modifiers (private, protected, public)
    - module exports
    - bundling data and methods that operate on that data within one unit 

- Generalization: sharing common details in a broader abstraction
    - Inheritance: "is-a" relationship
    - superclass vs subclass

- Polimorphism: enabling uniform interaction for different types 
    - Classic definition: "many forms"
    - Dynamic method dispatch 

- buttonaddAction(EventHandler)

- void addAction(EventHandler e) {
    //some code 

    e.handle(myEventObject);
}

- Liskov Substitution Principle (LSP): subtypes must be substitutable for their types
    - Ensures that a subclass can stand in for its superclass without altering the correctness of the program
    - Promotes reliability and maintainability in object-oriented design



    interface Steerable {  
     public void turn(Integer numberDegrees); 
} 
interface Drivable { 
    public void go(); 
    public void stop(); 
} 
public class Vehicle implements Steerable,Drivable { 
    private String name; 
    public void Vehicle(String name) { 
    this.name = name; 
   } 
    public void turn(Integer turn)  { 
         System.out.println("The " + name +" turned" +  turn + "degrees"); 

   } 

   public void go () { 
        System.out.println("Vroom! The " + name + "is driving"); 
   } 

  public void stop() { 
       System.out.println("Screech! The" + name + "stopped" )
  } 
} 


public class Point { 
     public int pointer = 0; 
     public int direction = 0; 

    public Point(int pointer, int direction) { 
       this.pointer = pointer; 
       this.direction = direction; 

     } 
     @Override 
     public String toString() { 
        return "(" + pointer + ","+ direction + ")"; 
     }  
  } 

public class LabelledPoint extends Point { 
      public String letter = "";  
    public LabelledPoint(int pointer, int direction, String letter) { 
        super (pointer, direction); 
        this.letter = letter; 
      } 
@Override 
     public String toString() { 

       return  letter + ":"+ super();  
     } 
} 