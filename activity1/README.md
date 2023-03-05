# Activities

## Task 1

- Refer to the following link. Discuss how the
  Recursive Factorial works:
  https://www.cs.usfca.edu/~galles/visualization/RecFact.html

  Answer:
    - The algorithm takes an integer n as an input.
     It checks if n is equal to 0 or 1. If so, it returns 1 since 0! and 1! are both equal to 1.
     If n is greater than 1, the algorithm calculates the factorial of n-1 recursively by calling itself with the input value of (n-1).
    The result of the recursive call is then multiplied by n to get the factorial of n.

- Refer to the following link. Discuss how the Recursive Fibonacci works:
  https://www.cs.usfca.edu/~galles/visualization/DPFib.html

  Ans:
    - The Fibonacci sequence is a series of numbers in which each number is the sum of the two preceding ones. The sequence starts with 0 and 1, and the next number in the sequence is the sum of the two preceding ones (i.e., 0+1=1, 1+1=2, 1+2=3, 2+3=5, and so on). 

## Task 2

There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. There is a simple implementations in `./src/` folder. Discuss how the code works.

Ans:
  - The function 'number_of_paths' takes an integer n as input and returns the number of ways to climb the stairs. If n is less than or equal to 0, the function returns 0 since there are no ways to climb the stairs. If n is 1, there is only one way to climb the stairs (by taking one step), so the function returns 1. If n is 2, there are two ways to climb the stairs (by taking one step twice or by taking two steps once), so the function returns 2.

## Task 3

- There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs or **3 stairs** at a time. Write a program that counts the number of ways, the person can reach the top. You can use the following program as a starter `./src/staircase1.cpp`. Also the link below might useful:
  https://www.includehelp.com/cpp-programs/stair-case-program-to-solve-the-staircase-problem.aspx

## Task 4: Individual (at home)

- What are the pros/cons of recursive over iterative Programming?

Ans: 
  - In general, the choice between recursive and iterative programming depends on the specific problem and the requirements for performance, readability, and maintainability. For problems that have a self-repeating or self-similar structure, recursive programming may be the best approach, while for problems that do not have this structure, iterative programming may be more appropriate.

- Difference between recursion and induction.

Ans:
  - Recursion refers to a process or function that calls itself one or more times within its own definition. Recursive functions are often used to solve problems that can be broken down into smaller sub-problems that are themselves similar to the original problem. Recursion is commonly used in programming languages to solve a wide variety of problems.

  - Induction, on the other hand, is a method of proof used in mathematics to establish the truth of a statement for all members of an infinite set. The principle of mathematical induction states that if a statement is true for a base case (often a specific number) and if the statement is also true for any number that comes after the base case (called the induction step), then the statement is true for all numbers in the infinite set. Induction is used to prove statements that follow a pattern or are dependent on previous cases.

> Refer to the [links](#links) section below.

## Links

- https://cpp.sh/
- [Difference Between Recursion and Induction](https://www.geeksforgeeks.org/difference-between-recursion-and-induction/)
- [Recursion vs Iterative Programming](https://www.softwaretestinghelp.com/recursion-in-cpp/)
