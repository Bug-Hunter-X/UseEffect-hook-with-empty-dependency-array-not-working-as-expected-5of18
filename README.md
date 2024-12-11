# React useEffect Hook Bug

This repository demonstrates a common bug related to the `useEffect` hook in React.  The issue revolves around an empty dependency array (`[]`) in `useEffect` not preventing re-renders as expected. This can lead to unnecessary re-renders and performance problems.

## Bug Description

The `bug.js` file contains a component that uses `useEffect` with an empty dependency array.  Despite the empty array, the effect runs on every render, even though it should only run once after the initial render.

## Solution

The `bugSolution.js` file shows the corrected implementation. The bug is solved by correctly using the empty dependency array in `useEffect` to make it run only once after the initial mount.