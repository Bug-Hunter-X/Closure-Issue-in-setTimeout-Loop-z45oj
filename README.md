# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common closure-related issue in JavaScript when using `setTimeout` within a loop.  The expected behavior is to log the numbers 0 through 9, with a one-second delay between each log. However, due to the way closures work in JavaScript, the loop completes before the `setTimeout` callbacks execute, resulting in all callbacks logging the final value of `i` (which is 10). 

The `bug.js` file contains the problematic code, and `bugSolution.js` provides a corrected version.

## How to reproduce

1. Clone this repository.
2. Open `bug.js` and run it using Node.js or a browser's developer console.
3. Observe that the output is ten 10's instead of numbers from 0 to 9. 
4. Open `bugSolution.js` to see how the problem is fixed.