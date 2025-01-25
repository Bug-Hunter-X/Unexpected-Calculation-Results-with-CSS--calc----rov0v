# Unexpected Calculation Results with CSS `calc()`

This repository demonstrates a subtle bug involving unexpected calculation results when using the `calc()` function in CSS. The bug is difficult to detect because it doesn't always produce an obvious error, and standard CSS validators may not flag it. 

The `bug.css` file contains the problematic CSS code.  The `bugSolution.css` file shows a corrected approach.

## Bug Description
The `calc()` function in CSS doesn't always behave predictably when units are mixed, or when more complex calculations are nested.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in a web browser. 
3. Observe the unexpected rendering, which will differ from expected behaviour.

## Solution
The solution involves careful attention to unit consistency and order of operations within `calc()`. See `bugSolution.css` for the fix.  Adding extra parenthesis to enforce order of operations can resolve some issues.