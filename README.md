# Express.js Route Parameter Error Handling

This repository demonstrates a common error in Express.js route handlers:  failure to handle invalid or missing parameters.  The `bug.js` file shows the flawed code, and `bugSolution.js` provides the corrected version with robust error handling.

## Bug Description

The original code attempts to access a user based on an ID passed as a route parameter. However, it doesn't handle cases where the ID is not a valid number or is missing, leading to a potential crash or unexpected behavior.

## Solution

The solution involves adding checks to validate the parameter before attempting to access the user.  The corrected code includes explicit error handling for missing IDs or non-numeric IDs, returning appropriate HTTP status codes and error messages.