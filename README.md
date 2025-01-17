# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js where exceptions within an HTTP server are not handled correctly, leading to unexpected behavior and crashes.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version with robust error handling.

## Problem

The original code lacks proper error handling.  If an error occurs during request processing (e.g., database connection failure, file system error), the server crashes without sending an informative error response to the client. 

## Solution

The improved code uses a `try...catch` block to wrap the request handling logic. This allows the server to catch exceptions, log them for debugging, and send a well-formatted error response to the client, maintaining server stability.