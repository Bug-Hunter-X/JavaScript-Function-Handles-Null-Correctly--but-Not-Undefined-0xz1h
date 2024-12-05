# JavaScript Function Undefined Behavior

This repository demonstrates a subtle bug in JavaScript function handling of undefined values. The function `foo` correctly handles `null` inputs but behaves unexpectedly when given `undefined`.

## Bug Description
The function `foo` is designed to return 0 if the input `x` is `null`.  However, when `undefined` is passed, it produces `NaN` instead of handling it gracefully (e.g., returning 0 or throwing an error).  This inconsistency can be problematic. 

## Reproduction
1. Clone this repository.
2. Run `bug.js` using a JavaScript interpreter (like Node.js).  Observe the unexpected output.

## Solution
The `bugSolution.js` file provides a corrected version that explicitly handles both `null` and `undefined` inputs, providing a more consistent and robust behavior.