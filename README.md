# Objective-C Array Index Out of Bounds Bug

This repository demonstrates a common error in Objective-C: accessing an array element using an index that is out of bounds.  This can lead to crashes or unexpected behavior in your application.

The `bug.m` file contains the buggy code, which attempts to access an array element with an invalid index. The `bugSolution.m` file provides a corrected version with proper bounds checking.

## How to reproduce

1. Clone this repository.
2. Open `bug.m` in Xcode.
3. Run the code. You should encounter a crash or unexpected behavior. 
4. Open `bugSolution.m` and run the corrected code, observing that no crash occurs.

## Solution

Always ensure that the index you're using to access an array element is within the valid range of 0 to `myArray.count - 1`.  Use checks to prevent accessing elements beyond the array's boundaries.  The `bugSolution.m` demonstrates a safe way to handle array access.