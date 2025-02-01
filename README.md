# React useEffect Infinite Loop Bug
This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The issue arises from an incorrectly configured dependency array, leading to an infinite loop of re-renders.

## Problem
The provided `MyComponent` uses `useEffect` to log the current count to the console.  However, without `count` in the dependency array, the effect runs on every render, triggering a continuous update cycle.