# Intro to JavaFX 
## Tue Nov 25

- Introduction: 
    - Set of GUI components for building graphical applications
    - Modern alternative to swing
    - Unlike Swing, JavaFX is not part of the JDK
    - Download as a separate package 
    - Or use Maven to specify JavaFX as a dependency

- JavaFX and Java modules:
    - Distributed using Java's new modules feature
    - Module is a collection of related packages
    - Modules give developers more control over what parts of a module are available to users of the module
    - All Java apps that use modules must have a module-info.java file

- Other GUI technologies :
    - Common features: 
        - Components
        - Layout Management 
        - Event handling 
        - Styling/theming 
        - Input validation
        - Internationalization support
        - Accessibility support 
    
- Feature of JavaFX:
    - Rich set of UI controls
    - Flexible APIs for reactinng to user actions and changes in data
    - Declarative UI definition using FXML
    - Styling via CSS 
    - Ability to display arbitrary web content using Web View
    - Ability to leverage GPUs
    - Built-in support for accessibility and internationalization

- The application class: 
    - Every JavaFX app starts with a class that 
        - Extends the JavaFX Application class
        - Overrides the start method

    - The main method calls Application.lauch()
    - Once JavaFX platform is ready, your class's start method is called 
        - With a stage object as an argument 

- Stage:
    - Represents the root window of an app
    - Usually has window decorations 
    - Stage usually contains a Scene

- Scene Class:
    - Consists of a scene graph 
    - Tree of node objects 
        - each node has 1 parent (except the root node)
        - each node may have 0 or more children 

- Node class hierarchy:
    - Parent: can contain child nodes
    - Group: for grouping related Nodes
    - Region: styleable with CSS
    - Control: interactive UI element
    - Pane: manages layout of children
    - Shape: represent drawable shapes, incl. text

- JavaFX coodinates:
    - the top left corner is at (0,0)

- Regions vs Groups:
    - Regions have a visual representation
        - can be styled
        - have spacing concerns 
    - Groups are purely logical
        - allows multiple nodes to be manipulated as a unit

- Region padding:
    - All regions have a setPadding method that can be used to determine how far child nodes are inset from the boundary of the region

- Panes:
    - Panes are special JavaFX classes that help arrange elements
    - Different panes arrange their children in different ways

- Shapes: 
    - javafx.scene.shape package contains many commonly used classes for drawing shapes and text
    - All derive from the shape class
        - Arc
        - Ellipse
        - Line
        - Polygon
        - Polyline

- Text: 
    - java.scene.text.Text class is used to draw text 
        - Also extends Shape
        - Adds ability to set font, styling 

- Color: 
    - javafx.scene.paint.Color class can be used to represent colors 
