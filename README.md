# Unnecessary useEffect with Console Logs in React

This repository demonstrates a common React bug involving an `useEffect` hook with an empty dependency array that still causes unnecessary console logging, potentially impacting performance and making debugging more difficult.

## Bug Description

The `MyComponent` component uses `useEffect` with an empty dependency array (`[]`). This is intended to make the effect run only once after the initial render. However, the `console.log` statements inside the effect and cleanup function still execute, causing unwanted output.

## Solution

The solution removes the unnecessary `console.log` statements, leading to a cleaner and more performant component.