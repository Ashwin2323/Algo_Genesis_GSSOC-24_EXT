# Spiral Matrix Traversal

Spiral matrix traversal involves traversing a matrix in a spiral or circular order, starting from the top-left corner and moving inward in a clockwise direction until all elements are visited. This technique is useful in various computational problems that involve matrix manipulations, pattern generation, or data retrieval.

## Problem Statement

Given a 2D matrix of integers, the task is to print the elements of the matrix in **spiral order**. The traversal begins at the top-left corner, proceeds to the right along the top row, then down the rightmost column, then to the left along the bottom row, and finally up the leftmost column, continuing inward until all elements are covered.

### Example:
Enter the number of rows: 3  
Enter the number of columns: 3  
Enter the matrix elements:  
`1 2 3
4 5 6
7 8 9`


The output should be:

`Spiral order: 1 2 3 6 9 8 7 4 5`



## Approach

### Steps to Traverse in Spiral Order:

1. **Define Boundaries**:
   - `top`: Initially at the first row.
   - `bottom`: Initially at the last row.
   - `left`: Initially at the first column.
   - `right`: Initially at the last column.

2. **Traverse in Four Directions**:
   - From **left to right** across the top boundary.
   - From **top to bottom** along the right boundary.
   - From **right to left** across the bottom boundary (if any row is left).
   - From **bottom to top** along the left boundary (if any column is left).

3. **Adjust Boundaries**:
   After each directional traversal, the corresponding boundary is adjusted (move inward).

4. **Repeat Until All Elements Are Traversed**:
   The traversal continues while there are still elements within the boundaries.

### Example Walkthrough:
For the given matrix:

