# Infinite Rendering Bug in React useEffect

This repository demonstrates a common error in React's `useEffect` hook that leads to infinite re-rendering.  The problem arises from omitting dependencies in the `useEffect` hook's second argument, causing the effect to run on every render, triggering an infinite loop.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console, the component continuously renders.

## Solution

The solution involves adding the `count` variable as a dependency to the `useEffect` hook. This ensures the effect only runs when `count` changes, preventing the infinite loop.

## Learn More

For more information on the `useEffect` hook and its dependencies, refer to the official React documentation:
[https://reactjs.org/docs/hooks-reference.html#useeffect](https://reactjs.org/docs/hooks-reference.html#useeffect)