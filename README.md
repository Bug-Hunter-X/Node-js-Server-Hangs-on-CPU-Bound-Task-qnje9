# Node.js Server Hangs on CPU-Bound Task

This repository demonstrates a common issue in Node.js where a server hangs when performing a CPU-intensive task without proper asynchronous handling.  The `bug.js` file shows the problematic code, and `bugSolution.js` provides a solution using asynchronous operations.

## Problem

The `bug.js` file creates an HTTP server that performs a computationally expensive loop in its request handler. This blocks the event loop, preventing Node.js from handling other requests. The server effectively becomes unresponsive.