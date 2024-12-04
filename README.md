# React useEffect Hook Missing Dependency

This repository demonstrates a common error in React applications involving the `useEffect` hook: missing dependencies in the dependency array.  The `useEffect` hook is designed to perform side effects based on changes to specified values.  If a dependency is omitted, the effect might not run when expected, leading to unexpected behavior.

## Bug Description

The `MyComponent` initially displays a count of 0. Incrementing the counter does not update the console logs. This is because the `count` variable is not included in the dependency array for the `useEffect` hook.  The effect only runs once during the initial render.

## Solution

The solution includes the `count` variable in the dependency array. Now the effect runs whenever `count` changes, correctly reflecting the current value.
