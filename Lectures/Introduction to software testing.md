# Introduction to software testing
## Tue Oct 28
### 

- I was working on lab 3 last class, I missed last class because of it. 

- What is software testing ? 
    - Running software or software components in specific ways to verify that it works as expected. 

 - Why test ? 
    - Ensure software quality
    - Identify bugs 
    - Detect regressions

- When should the code be tested ? 
    - Early and often
    - Test-driven development (TDD) tests are written before the tested code
    - In bug-driven development (BDD) tests are written in reponse to detected bugs, and prevent the bug from being re-introduced 

- Kind of tests: 
    - Scope : the level of detail at each testing occurs 
    - Execution purpose : how tests are executed
    - Context : in which context tests are executed
    - Testing purpose : the broad testing purpose of a set of tests
    - Special focus : a specific domain for a set of tests

- Kinds of tests by scope: 
    - Unit
    - Integration
    - End-to-end/ System
    - Acceptance

- Kinds of tests by execution pattern: 
    - Manual
    - Automatic
    - Continuous

- Kinds of tests by context 
    - Static 
    - Dynamic

- Kinds of tests by testing purpose
    - Functional 
    - Non-functional
    - Regression 
    - Smoke/Sanity
    - Alpha/Beta

- Kinds of tests by special focus
    - Performance 
    - Security
    - Compatibility
    - Usability
    - Recovery/Failover

- Testing frameworks: 
    - most software platforms have it to make the process of writing and running unit tests easier

- Writing automated tests:
    - writing automated tests helps ensure program correctness
    - once tests have been written it is easier and fast to re-run them all and verify that they all pass
    - create a separate program that runs the program and verifies that it produces expected output given specific input and tests that individual program components work as expected 
    - each test should clearly state the expected output, the actual output, and make a visual distinction between passed and failed states

 - Unit testing with JUnit: 
     - JUnit is the most used unit testing framework for java
     - To use it in a Maven project, simply add it as a dependency
     - Using IDEA, can be run individual test methods, all test methods within a test class, and all tests in all test classes

- Writing tests
    - test program should have many tests, each verifying that a specific starting state or sequence of inputs produces the expected results
    - test all possible inputs and check for expected outputs

- Choosing what to test
    - Input validation: test the valid parameters produce correct results, and don't need to test parameters that are outside precondition limits
    - Boundary conditions: test values at the upper/lower bounds for parameters that have a limited acceptable range of values, and test that null and empty string/list are handled correctly
    - Special cases: test values that trigger special cases in conditionals/ loops
    - Exception handling: if conditions should cause an error to be thrown, test that those conditions do in fact throw an exception
    - code coverage : percentage number that indicates how much of your code is executed as a result of running your tests. 
    - focus testing on most important components 