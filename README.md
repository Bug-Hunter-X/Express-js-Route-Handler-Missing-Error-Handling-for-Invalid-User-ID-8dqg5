# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID but fails to handle cases where the ID is not a valid number.

## Bug

The `bug.js` file contains an Express.js route handler that fetches a user based on their ID.  The code attempts to parse the ID as an integer, but it doesn't handle the scenario where the ID is not a number or is otherwise invalid. This can lead to unexpected behavior or crashes.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler.  It includes error handling to check if the ID is a valid number.  If the ID is invalid or the user is not found, an appropriate error response is returned.