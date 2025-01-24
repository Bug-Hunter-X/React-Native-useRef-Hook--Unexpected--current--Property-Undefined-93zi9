# React Native useRef Hook: Unexpected 'current' Property Undefined

This repository demonstrates a common issue in React Native where the `current` property of a `useRef` hook is unexpectedly undefined, leading to unexpected behavior or crashes. The problem often arises when the component re-renders before the ref has been properly assigned.

## Problem
The `UnexpectedRef.js` file shows the problematic code. The `current` property of the ref is accessed within a function that might be called before the ref has been initialized correctly, resulting in `undefined`.

## Solution
The `UnexpectedRefSolution.js` file demonstrates a solution. This uses an optional chaining operator (?.) and nullish coalescing operator (??) to handle the case where the `current` property is undefined gracefully, preventing crashes and ensuring a more robust application.

## Steps to Reproduce
1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to start the app.
5. Observe the behavior.