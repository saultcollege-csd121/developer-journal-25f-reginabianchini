- I will be creating a guessing game that will tell the user to guess a number from 1 to 10. The user will insert theit guesses and then every guess will be stored in a separate file until the right number is typed. 

- I don't know how to generate a random number in java. 
    - I just looked in the https://stackoverflow.com/questions/18647479/random-number-from-1-25-in-java-sequence and got the answer for it. Now I understand it. 

- I also need to try creating a list with the numbers that can be typed
- After I need to create the loop to loop through this list to then select the right one 
- I don't know if I should try to register the number of attempts that it took for the person to get the answer right or not. I think for now I will try to just leave without it. 


## Code explanation:
- Random: will be used to generate random numbers that will be the correct number for the code
- Loop: will be created to make the code continue running until the user guess the right number. 
- Conditionals: will be the "Not the right number! Try again" and "That is the number!"
- Attempts: it will count and register at the file how many attempts the user had to do to get to the correct number
- Try/catch: will be the part that will be handling the errors. If there is any invalid inputs on the code the try/catch will prevent the code of crash
- List: It will contain a list where it will be stored the number of attempts 
- Create file: will create a new file with all the answers that were attemped by the user until getting the right number.

## Summary: 
In this Lab I tried to create a guessing game where the user had to guess a number from 1 to 50. 
After that the code will have a loop that will be looping on the code until the user gets the correct number.
Every time the user inserts a new guess it will be copied to a file and the times pf guesses will be conted and displayed at the end when the user guess the right number