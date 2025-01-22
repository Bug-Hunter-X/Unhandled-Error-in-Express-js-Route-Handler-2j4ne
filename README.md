# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js applications: failing to handle invalid user inputs or edge cases in route handlers.

The `bug.js` file shows a route handler that's vulnerable. The `bugSolution.js` provides a solution by adding robust error handling.

## Problem

The `bug.js` example lacks proper error handling for missing or invalid `userId` parameters.  This can lead to errors and crashes if the route is accessed with an invalid ID. 

## Solution

The `bugSolution.js` example addresses this issue by:

1. Validating the `userId` parameter to ensure it's a number.
2. Returning a proper error response (e.g., 400 Bad Request) if the ID is invalid.
3. Using a try...catch block for potential database query errors.