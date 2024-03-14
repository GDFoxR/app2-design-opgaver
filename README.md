# Learning outcome

Knowledge about algorithms, datastructure and common programming paradigme.

## Purpose

The purpose of this branch is to test your knowledge about algorithm, datastructure and programming paradigm.

## Goal

This gives you a indication of wether you have a sufficient understanding of the subjects and wether you should be aware of some pit in your knowledge.

# Part 1 - Algorithms

## What is the key difference between a functions and algorithm?

<!-- The key difference between a function and an algorithm is in their definition and purpose.

A function is a piece of code designed to perform a specific task; it takes some input, processes it, and returns an output. Functions are building blocks in programming that allow for code reuse, modularity, and organization.

An algorithm, on the other hand, is a step-by-step procedure or formula for solving a problem. It is a conceptual idea independent of programming languages, focusing on the logic behind solving a specific problem. An algorithm can be implemented through one or more functions in a programming language, but its essence lies in the methodology and steps taken to reach a solution. -->

## The following code example, why is it a algorithm and why is it not?

```PYTHON
import numpy as np


def Possibility(x,y,n) :
    global Box
    if Box[x][y] == 0 :
        for i in range(9) :
            if Box[x][i] == n :
                return False
        for j in range(9) :
            if Box[j][y] == n :
                return False
        r = x
        c = y
        boxx = 0
        boxy = 0
        while r - 3 >= 0 :
            r = r - 3
            boxx = boxx + 1
        while c - 3 >= 0 :
            c = c - 3
            boxy = boxy + 1
        for i in range(3) :
            for j in range(3):
                if Box[i+boxx*3][j+boxy*3] == n:
                    return False
        return True

def Solve() :
    global Box
    for r in range(9):
        for c in range(9):
            if Box[r][c] == 0:
                for n in range(1,10):
                    if Possibility(r,c,n) == True:
                        Box[r][c] = n
                        if Solve() == False:
                            Box[r][c] = 0
                        else :
                            return True
                return False

Box = [
    [5, 0, 0,   6, 7, 0,    9, 0, 0],
    [0, 4, 0,   8, 0, 0,    0, 0, 0],
    [8, 0, 0,   5, 0, 0,    6, 1, 3],

    [0, 6, 2,   4, 0, 0,    0, 7, 0],
    [1, 0, 0,   0, 0, 3,    0, 2, 0],
    [3, 7, 4,   9, 0, 8,    0, 0, 0],

    [0, 9, 6,   1, 0, 7,    8, 0, 2],
    [2, 1, 8,   0, 0, 6,    0, 4, 5],
    [0, 5, 0,   0, 8, 0,    0, 9, 0]
    ]

Solve()
print(np.matrix(Box))





# Backtracking is an algorithmic paradigm that solves optimization and search problems by trying all possible solutions, and then backtracking and trying other solutions if the current solution does not work.

# In the case of the Sudoku solving program, the algorithm starts by trying to fill in a single cell in the puzzle with a possible value. If the program is able to solve the puzzle using that value, it moves on to the next cell. If it is not able to solve the puzzle using that value, it backtracks and tries another value for the current cell.

# The algorithm continues trying different values for different cells until it is able to solve the puzzle, or until it runs out of possible values for all cells.




```

# Part 2 - Datastructure

## What is the primary difference between datastructure and datatypes?

<!-- A data structure is a way of organizing and storing data in a computer so that it can be accessed and modified efficiently. It defines the layout of the data in memory, including the type and number of variables, their relationships to each other, and how they are accessed.

A data type, on the other hand, is a specific format for data, such as an integer, string, or floating-point number. It defines the properties and characteristics of the data, such as its size, range of values, and allowed operations.

In summary, data structures define the organization of data in memory, while data types define the format of the data. -->

## Name three datastructures

Array

Queue

Tree

### What are the strength

### What are the weakness

### What are the difference

### What are the simalarities

# Part 3 - Paradigm

## What is a programming paradigm?

## Compare two paradigms
