# React useEffect Hook Runs on Every Render

This repository demonstrates a common error in React's `useEffect` hook where the effect runs on every render, even when it shouldn't.  The issue stems from an improper use of the dependency array.

## Problem

The provided `bug.js` file shows an `useEffect` hook without a dependency array or with an incomplete dependency array. This causes the effect to re-run on every render, causing unnecessary re-renders, performance issues, and potential unexpected behavior.

## Solution

The `bugSolution.js` file demonstrates the correct usage of the `useEffect` hook.  The dependency array is correctly specified to only run the effect when the `count` variable changes.  This prevents unnecessary re-renders and solves the performance issues.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs to see the unexpected behavior in `bug.js` and the improved behavior in `bugSolution.js`.
