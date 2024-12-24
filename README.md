# Incorrect Conditional Rendering in useEffect Hook
This repository demonstrates a common bug in React applications involving the `useEffect` hook and conditional rendering. The bug occurs when the update logic within the `useEffect` hook does not cover all possible states, potentially causing unintended behavior or rendering glitches.

## Bug Description
The provided code snippet showcases a component that updates the document title based on a counter's value. However, the conditional statement within the `useEffect` hook only updates the title if the counter is greater than 0. This results in the title remaining unchanged when the counter is 0, creating an unexpected discrepancy between the displayed count and the document title.

## Solution
The corrected code ensures that the document title is updated regardless of the counter's value. This is accomplished by removing the conditional statement and always updating the title based on the current count value.

## How to Reproduce
1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.
5. Observe the document title as you increment and decrement the counter.  You'll notice the discrepancy with the buggy code and the correct behavior with the solution.
