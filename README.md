# React useEffect Hook Dependency Array Issue

This repository demonstrates a common error in React's `useEffect` hook: creating unintended infinite loops due to issues with the dependency array.

## The Bug
The `bug.js` file contains a simple counter component.  The `useEffect` hook is used to log the current count to the console. However, there's a subtle error in how the dependency array is used, which will cause the component to re-render infinitely.

## The Solution
The `bugSolution.js` file corrects the error by properly managing the dependency array of the `useEffect` hook. This version ensures the effect only runs when the `count` value actually changes.