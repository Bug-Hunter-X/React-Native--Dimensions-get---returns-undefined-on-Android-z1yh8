# React Native Dimensions.get() Undefined Issue on Android

This repository demonstrates a common issue encountered when using the `Dimensions.get()` API in React Native on Android.  The problem arises because the `Dimensions` API doesn't always provide immediate values.  Attempting to use the dimensions before they're available results in `undefined` being returned, potentially leading to crashes or unexpected behavior in your application.

The `bug.js` file shows the error, and `bugSolution.js` provides a solution using the `useEffect` hook to handle the asynchronous nature of the `Dimensions` API.