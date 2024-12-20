# React Lifecycle Method Bug

This repository demonstrates a common bug in React components related to the use of deprecated lifecycle methods. Specifically, the example shows how using `componentWillReceiveProps` can lead to unexpected behavior and data inconsistencies.

## Bug Description
The component `BuggyComponent.js` incorrectly utilizes `componentWillReceiveProps` to update its internal state based on changes in props. This method is deprecated and unreliable in modern React applications.

## Solution
The solution is provided in `FixedComponent.js`.  Instead of `componentWillReceiveProps`, it leverages the `useEffect` hook to effectively respond to prop changes, updating the component's state with the latest prop values.

## How to reproduce the bug:
1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the inconsistent state updates in the buggy component and compare with the correct behaviour in the fixed component.