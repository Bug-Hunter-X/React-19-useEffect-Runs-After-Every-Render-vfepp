# React 19 useEffect Runs After Every Render

This repository demonstrates a common issue in React 19 where the `useEffect` hook runs after every render, leading to performance problems and unexpected behavior.  The example showcases the problem and its solution.

## Problem
The `useEffect` hook in the provided `bug.js` file lacks a dependency array, causing it to re-run on every render. This is inefficient and can lead to infinite loops or unexpected side effects.

## Solution
The corrected code in `bugSolution.js` demonstrates how to fix this issue. By including the `count` variable in the dependency array, the `useEffect` hook only runs when `count` changes, solving the performance issues and unexpected behavior.

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console logs in the browser developer tools and see the frequency of updates.
5. After fix the bug using the solution file, run the app and observe the difference.