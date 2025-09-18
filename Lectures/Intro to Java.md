# Introcution to Java
## Tue Sep 16
### Today we are taking a look at the main differences when using java and python. 

- Last week I learned some interesting differences between Python and Java. If needed go back to journal entry Class 1

- Switch statements: 
- Loops: 
    - There are 4 ways of looping in Java: the while loops, the for loops, for-each loops, and existing loops 
- Arrays: 
    - to declare an array, add [] after the type. 
        - Ex: int[] numbers;
    - You can intialize an Array with an Array literal or you can initialize it to a specific size. 
        - Ex: int[] numbers = {1,2,3 };
              int[] numbers = new int[10];
    - Array literals are delimited using curly braces. Python's list use square brackets. 
    - new is necessary to create a new array, because it is an object type 
    - lenght of it is indicated by the right-hand side, not left. Left side = type and Right side = value
- Indexing and Updating Arrays: 
    - First element of index is 0 
    - array variable can be indexed using []
    - Arrays are mutable, meaning they can be changed 
    - You can update it by using []
        - Ex: int[] a = {1,2,3} ; 
              String[] b = {"one","two","three"};
              a[0] == 1; Evaluates to true 
              a[2] = 99; change of the value of the third element           
- Determining the lenght of an Array: 
    - lenght property is used to know how long your array is
        - Ex: int[] a = {1,2,3,4,5};
              a.lenght;
- Comparing Arrays: 
    - == works like the is in python
        -Ex: int[] a = {1,2,3};
             int[] b = {1,2,3};
             int[] c = a;
             a == a // true 
             a == c // true
             a == b // false 
    - Arrays.equals(..) can be used to check if two arrays have same set of values
        - Ex: int[] a = {1,2,3};
              int[] b = {1,2,3};
              Arrays.equals(a,b); 
    - Traversing Arrays: 
        - There are 3 ways to traverse an Array
            - With for loops: 
            - With for-each loops: 
            - 
Go back to the link and read it throught again after class
Lambda was skipped 

- User input: 
    - use IO.readln
        Ex: String response = IO.readln("What is your favorite number?"); 
- Errors and Error Handling: 
    - Raising errors: 
        - Two types of errors: runtime exceptions and checked exceptions 
            - Runtime exceptions are errors that can appear any time and are used to refer to programming error 
            - Checked exceptions are errors 

              