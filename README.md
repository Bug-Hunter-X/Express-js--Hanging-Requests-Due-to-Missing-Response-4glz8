# Express.js Hanging Request Bug

This repository demonstrates a common error in Express.js applications where requests hang because the server fails to send a response. The bug is caused by a missing `res.send()` or similar method within a request handler.

## Bug
The `bug.js` file contains an Express.js application with a route handler that lacks a response.  This leads to hanging requests. 

## Solution
The `bugSolution.js` file fixes this by adding a `res.send()` method to send a response to the client.

## How to reproduce
1. Clone this repository.
2. Navigate to the project directory.
3. Run `node bug.js`.
4. Open your browser and navigate to `http://localhost:3000`. You'll observe that the request hangs or times out.
5. Repeat steps 2-4 with `bugSolution.js` to see the fix in action.

## Contributing
Contributions are welcome!