# Off-by-one error in Java array iteration
This repository demonstrates a common off-by-one error in Java when iterating over an array.  The error occurs because the loop condition `i <= arr.length` attempts to access an index that is out of bounds.  The correct condition should be `i < arr.length`.

## How to reproduce the bug
1. Compile and run `Bug.java`.
2. Observe the `ArrayIndexOutOfBoundsException`.

## How to fix the bug
1. Modify the loop condition in `BugSolution.java` to `i < arr.length`.
2. Recompile and run `BugSolution.java`. This will successfully iterate through the array without error.