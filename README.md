# Direct Mutation of State Variable in React
This example demonstrates a common mistake when working with the `useState` hook in React: directly mutating the state variable instead of using the setter function provided by `useState`. 

## Bug
The `bug.js` file shows an incorrect implementation where the `count` state variable is incremented directly within the `useEffect` hook, which will not trigger a re-render, resulting in a stale value.

## Solution
The `bugSolution.js` file demonstrates the correct approach. Instead of directly mutating `count`, the `setCount` function is used to update the state value, triggering a re-render and displaying the correct count.
