# React Native Dimensions.get('window') returns undefined on Android

This repository demonstrates a common issue in React Native where `Dimensions.get('window')` or `Dimensions.get('screen')` returns `undefined` on Android, particularly during initial app launch.  This can lead to crashes or unexpected behavior in components dependent on screen dimensions.

The solution involves using the `Dimensions` API correctly with a state variable to handle the asynchronous nature of dimension retrieval.

## Bug

The `DimensionsBug.js` file shows the incorrect usage of the `Dimensions` API, resulting in the `undefined` error.

## Solution

The `DimensionsBugSolution.js` file demonstrates the corrected usage, including a state variable to safely handle the asynchronous nature of obtaining screen dimensions.