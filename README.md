# JavaScript ZeroDivisionError: Silent Failure

This repository demonstrates a common yet subtle error in JavaScript:  a `ZeroDivisionError` that can silently fail without throwing an explicit error.

The `bug.js` file contains a function `foo` that intends to handle cases where either `a` or `b` is zero.  However, it only checks the parameters before doing the division, so if it is zero the division will still happen leading to an error. The solution is provided in `bugSolution.js`

## How to reproduce

1. Clone this repository.
2. Run `bug.js` (e.g., using Node.js: `node bug.js`).
3. Observe the silent failure (or exception in strict mode).