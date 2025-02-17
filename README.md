# React Native: Accessing State Before Mount

This repository demonstrates a common error in React Native: attempting to access component state or props before the component has finished mounting.  The error manifests as `undefined is not an object (evaluating 'this.state.myVariable')` or similar.

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides the correct implementation using the `useEffect` hook to ensure state and props are accessed after mounting.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run the app on a simulator or device.
4. Observe the console output, which will show the initial error from `bug.js`. Then run bugSolution.js and observe the fixed code.