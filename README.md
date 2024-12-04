# Unexpected Null Handling in JavaScript Function

This repository demonstrates a subtle bug in a JavaScript function that involves unexpected null handling.  The `foo` function is designed to add two numbers; however, it prematurely returns `null` if either input is `null`, even if the other input is a valid number. This behavior might be unintended, leading to incorrect results in certain scenarios.

The `bug.js` file contains the buggy code, while `bugSolution.js` offers a corrected version that handles null values more gracefully.

## Bug Description
The `foo` function's logic to handle `null` values isn't robust enough. It returns `null` immediately if either argument is `null` rather than attempting to handle the `null` in a way that avoids failure.