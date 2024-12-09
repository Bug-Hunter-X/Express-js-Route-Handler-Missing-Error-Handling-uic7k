# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID. If a non-numeric ID is provided, the application crashes due to a `NaN` comparison.

## Bug
The `bug.js` file contains the buggy code.  It attempts to parse the user ID as an integer, but fails to handle the case where the ID is not a number, leading to a runtime error.

## Solution
The `bugSolution.js` file provides a corrected version. It includes explicit checks to ensure the user ID is a number before attempting to find the user.