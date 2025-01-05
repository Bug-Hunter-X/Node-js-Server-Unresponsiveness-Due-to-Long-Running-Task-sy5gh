# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js applications where a long-running task in the request handler can cause the server to become unresponsive.  The `server.js` file contains the problematic code, while `serverSolution.js` provides a solution using asynchronous operations.

## Problem

The server performs a CPU-intensive calculation in the request handler.  This blocks the event loop, preventing it from processing new requests.  The server appears to hang and stops responding.

## Solution

The solution involves using asynchronous programming techniques to prevent blocking the event loop.  The `serverSolution.js` file demonstrates how to achieve this using asynchronous functions and promises.