# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by an incorrectly specified dependency array.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected code.

## Bug Description
The original code includes a `useEffect` hook without a proper dependency array. This causes the effect to run on every render, leading to an infinite loop and crashing the application.

## Solution
The corrected code includes `[count]` in the dependency array of the `useEffect` hook. This ensures the effect only runs when the value of `count` changes.