# Lab 6
## Tue Nov 25

- Ideas:
    - Egg Timer
    - Habit tracker 
    - Recipe Scaler and grocery list generator
    - Flashcard Quiz with Spaced Repetition
    - Mini Strategy Game 
    - Personal Budget Planner with category charts
    - Workout Timer + Exercise Circuit Builder


### I will create an Egg timer that will have four different settings for different styles of eggs. It will have a circle in the middle that will change colours depending on its state. 


 -    Spinner<Integer> uses generics because it stores Integer values
- SpinnerValueFactory is an abstract class
- There are different subclasses of it:
        IntegerSpinnerValueFactory
        DoubleSpinnerValueFactory
        ListSpinnerValueFactory

- The first Java line the JVM executes is main, which calls launch(args)
- launch bootstraps JavaFX and eventually calls the overridden start(Stage primaryStage) method
- start constructs the UI (BorderPane, controls, spinners, buttons), sets up event handlers (setOnAction) and the Timeline (created later when Start is pressed), builds the Scene, and calls primaryStage.show().
- User actions (button presses and combo box selection) drive runtime behavior via the setOnAction handlers; JavaFX calls the registered EventHandler when those events occur.
- When the user clicks Start, the handler computes secondsLeft from the selected preset or spinners
- Polymorphism allows different objects to respond differently to the same method call.
-  It mainly happens through method overriding—where a subclass replaces a method from its parent—and Java decides at runtime which version to run depending on the actual object.
- main -> launch -> start(Stage) (UI construction) -> handlers respond to user events.