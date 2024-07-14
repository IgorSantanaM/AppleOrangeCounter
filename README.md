# Apple and Orange Problem

This C# program solves the problem of determining how many apples and oranges land on Sam's house. The program takes into account the starting and ending positions of Sam's house, the positions of the apple and orange trees, and the distances at which each fruit falls from their respective trees.

## Problem Description

Sam's house is located between points `s` and `t` on a one-dimensional axis. The apple tree is located at point `a`, and the orange tree is located at point `b`. When a fruit falls from its tree, it lands `d` units away from the tree along the axis. Negative values of `d` indicate that the fruit falls to the left of the tree, and positive values indicate that it falls to the right.

Given the starting and ending positions of Sam's house, the positions of the trees, and arrays of distances at which each apple and orange falls, the program determines:
- The number of apples that land on Sam's house.
- The number of oranges that land on Sam's house.

## Solution Explanation

The solution involves the following steps:
1. **Input Parsing**: Read the input values from standard input which include `s`, `t`, `a`, `b`, lists of distances for apples, and lists of distances for oranges.
2. **Calculating Landing Positions**: For each apple and orange, calculate its landing position using `position = treePosition + distance`.
3. **Counting Valid Landings**: Check if each fruit's landing position falls within the range `[s, t]`. If it does, increment the respective counter (`appleCount` or `orangeCount`).
4. **Output Results**: Print the counts of apples and oranges that land on Sam's house.

## How to Use

To run the program:
1. Ensure you have a C# compiler installed (such as Visual Studio or .NET SDK).
2. Copy the provided C# code into a file (e.g., `AppleAndOrangeProblem.cs`).
3. Compile and execute the program. Here's how you can do it using .NET CLI:
     ```bash
   dotnet new console -n AppleAndOrangeProblem
   cd AppleAndOrangeProblem
   dotnet run
    ```
4. Follow the prompts to enter input values as described in the problem statement. 

## Examples 
Given the following input:
``` diff
7 11
5 15
3 2
-2 2 1
5 -6
```
the `program` should output:
```
1
1
```
## Explanation:
  One apple and one orange land on Sam's house based on the given positions and distances.
