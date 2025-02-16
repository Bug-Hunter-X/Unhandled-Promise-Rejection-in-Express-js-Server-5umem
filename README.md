# Unhandled Promise Rejection in Express.js Server

This repository demonstrates a common error in Node.js applications: unhandled promise rejections.  The `bug.js` file shows an Express.js server with an asynchronous operation that can throw an error.  Crucially, it lacks proper error handling, leading to a silent failure.  The `bugSolution.js` file provides a corrected version with robust error handling. 

## How to reproduce

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `node bug.js`.  Observe that the server starts but crashes silently when the promise rejects.
5. Run `node bugSolution.js`. Observe that the server starts and handles the error gracefully.