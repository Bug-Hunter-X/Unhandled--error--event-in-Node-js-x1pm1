# Unhandled 'error' event in Node.js

This repository demonstrates an example of an unhandled 'error' event in Node.js and provides a solution to handle it gracefully.

## Bug

The `bug.js` file contains a simple HTTP server that doesn't handle potential errors.  If the server encounters an issue (like a network problem), it will crash without logging any information.

## Solution

The `bugSolution.js` file shows how to add an 'error' event listener to the server to catch and handle any errors, preventing the application from crashing unexpectedly.  The solution logs the error details to the console for debugging purposes.

## How to reproduce

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `node bug.js`.
4. While the server is running, try stopping it abruptly (e.g., using Ctrl+C) or interfering with its network connection.
5. Observe the unhandled exception.  Then run `node bugSolution.js` and repeat step 4 to see the handled exception.

## Additional Notes

Always handle potential errors in your Node.js applications to prevent unexpected crashes and to gain valuable insights into error causes.