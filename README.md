# Unexpected Behavior with Loose Equality (==) in JavaScript

This example demonstrates an uncommon bug in JavaScript related to the use of loose equality (==) when comparing function arguments with null or undefined.

## Bug Description
The `foo` function uses loose equality (==) to check if the arguments `a` and `b` are null or undefined. This approach has unexpected behavior because loose equality does not always behave as expected with null and undefined.  Specifically, `null == undefined` evaluates to true, while `null === undefined` evaluates to false.

## Bug Solution
The solution uses strict equality (===) to explicitly check for null or undefined. This avoids the unexpected behavior of loose equality and ensures more predictable behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js`.
3. Run the JavaScript code in your preferred environment (e.g., browser's console, Node.js).
4. Compare the outputs of both functions. 
