# React useState Bug: Incorrect State Modification

This repository demonstrates a common error when using the `useState` hook in React: directly modifying the state object instead of using the setter function. This leads to the UI not updating correctly.

## Bug Description

The `bug.js` file contains a React component that incorrectly attempts to increment the count by directly modifying the state object. This doesn't trigger a re-render, resulting in a stale UI.

## Solution

The `bugSolution.js` file provides the correct way to update the state using the setter function provided by `useState`.  The setter function ensures that React correctly updates the UI after state changes.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe that clicking the button in `bug.js` doesn't increment the count. Then see `bugSolution.js` for the fix.