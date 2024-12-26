# React setInterval Memory Leak

This repository demonstrates a common error in React components that involves using `setInterval` within the `useEffect` hook without proper cleanup. This can lead to memory leaks and unexpected behavior.

## Bug Description
The `MyComponent` uses `setInterval` to update the count every second. However, it lacks the cleanup function in `useEffect` to clear the interval when the component unmounts, leading to a memory leak.