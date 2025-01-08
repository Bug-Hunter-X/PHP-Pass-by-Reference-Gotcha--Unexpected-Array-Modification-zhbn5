# PHP Pass-by-Reference Issue

This example demonstrates a common pitfall in PHP involving pass-by-reference in functions. When an array is passed by reference to a function, modifications within the function directly affect the original array outside the function's scope. This behavior is often unexpected and can lead to subtle bugs.

## How to Reproduce

1. Clone this repository.
2. Run the script `bug.php`.  Observe the output - you'll see the original array `$myData` has been modified in-place.
3. Run the script `bugSolution.php` to see how to resolve this issue using value copying.

## Solution

The recommended solution is to create a copy of the array before processing it inside the function.