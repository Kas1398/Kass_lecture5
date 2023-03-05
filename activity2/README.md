# Activities

## Task 1

Refer to the following link. Discuss how the Recursive Fibonacci with Memoization works:
https://www.cs.usfca.edu/~galles/visualization/DPFib.html

Ans:
  - Create a lookup table, such as an array or a dictionary, to store the results of previously computed subproblems.

  - Modify the recursive Fibonacci algorithm to first check the lookup table for the result of the current subproblem before computing it. If the result is in the lookup table, return it. If not, compute the result recursively as before. and so on

## Task 2

The stair case problem can be solved based on the Fibonacci series. There is a simple implementations in `./src/staircase2.cpp`.

  Ans:
    - This code uses recursion to find the Nth Fibonacci number and then uses the Fibonacci number to count the number of ways to reach the s'th stair.
    - In the fib function, if n is less than or equal to 1, it returns n itself. Otherwise, it recursively calculates and returns the sum of the n-1th and n-2th Fibonacci numbers using the formula fib(n) = fib(n-1) + fib(n-2).
    - Finally, in the main function, the value of s is set to 4, and the countWays function is called with s as its argument. The result is then printed to the console using cout.

- Explain how the code works. The following link might be useful:
  https://dev.to/alisabaj/the-climbing-staircase-problem-how-to-solve-it-and-why-the-fibonacci-numbers-are-relevant-3c4o

  Ans:
    - The fib() function is a recursive function that calculates the n-th Fibonacci number. It takes an integer n as an argument and returns the n-th Fibonacci number using the following formula: fib(n) = fib(n-1) + fib(n-2). The base case for the recursion is when n is 0 or 1, in which case the function simply returns n.

- Modify the code to use Dynamic Programming (Memoization)

## Task 3

Explain how the code in `./src/staircase3.cpp` works.

  Ans:
    - If the value of n is less than or equal to 1, then the function simply returns 1 as the base case.
    If the dp[n] has already been calculated before, the function immediately returns the value stored in dp[n].
    If the dp[n] has not been calculated before, the function calculates it using the formula dp[n] = fib(n - 1, dp) + fib(n - 2, dp); and then stores the result in the dp[] array for future use.
    The function then returns the value of dp[n].
    The countWays() function takes an integer n as its argument and initializes an integer array dp[] of size n+1 with -1 using the memset() function.
    The memset() function is used to set a block of memory to a particular value. In this case, all the elements in the dp[] array are set to -1.
    Then the fib() function is called with arguments n and dp[], which calculates the n'th Fibonacci number and stores the result in the dp[] array.
    Finally, the countWays() function returns the value of dp[n], which represents the number of ways to reach the n'th stair.
    In the main() function, the value of n is set to 4, and then the countWays() function is called with the value of n as its argument.
    Finally, the number of ways to reach the n'th stair is printed using the cout statement.

    

## Task 4: Individual (at home)

- There are `n` stairs, a person standing at the bottom wants to reach the top. Write a program that counts the number of ways someone can climb up to m stairs for a given value m. For example, if m is 4, it is possible to climb 1 stair or 2 stairs or 3 stairs or 4 stairs at a time. Make sure you use. Refer to the link below:
  https://www.geeksforgeeks.org/count-ways-reach-nth-stair/

  Ans:
    - Finally, we return the value of dp[m], which represents the total number of ways to climb up to m stairs.
    In the main function, we set m to 4 and call the countWays function with this value. The result is then printed to the console.

## Links

- https://cpp.sh/
- [leetcode.com](https://leetcode.com/problems/climbing-stairs/)
