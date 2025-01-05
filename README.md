# React useEffect Hook Missing Dependency

This repository demonstrates a common error in React applications involving the `useEffect` hook: omitting a necessary dependency from the dependency array. This can lead to unexpected behavior and subtle bugs that are difficult to track down.

The `bug.js` file shows the incorrect implementation, where the `count` variable is not included in the dependency array of the `useEffect` hook. This causes the effect to run only once, after the initial render, instead of after every state update.

The `bugSolution.js` file provides the corrected implementation. By including `count` in the dependency array, the effect now runs every time the `count` state variable changes, resulting in the expected behavior.

This example highlights the importance of carefully considering the dependencies passed to `useEffect` to ensure your component behaves as intended.