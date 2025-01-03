# CSS calc() Unexpected Behavior

This repository demonstrates an uncommon issue with the CSS `calc()` function when combining percentage and pixel units. The expected behavior isn't always observed due to the order of operations and unit handling.

## Bug Description
The `calc()` function produces an unexpected result when subtracting pixels from a percentage-based width. This occurs in scenarios where the expected behavior would be to calculate the percentage first, and then subtract the pixels.  This often results in the computed width being off.

## How to reproduce
1. Clone the repository
2. Open `bug.css` and `bugSolution.css`
3. Compare the behavior of the `calc()` function in both files.

## Solution
To avoid such unexpected behavior, ensure your calculations are clear by using parentheses to control operator precedence, particularly when combining units like percentages and pixels.