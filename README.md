# React Native FlatList Performance Issue

This repository demonstrates a performance issue encountered when using React Native's FlatList component with a large dataset (1000 items in this example).  The rendering of this many items leads to significant lag and jank, impacting the user experience.

## Problem

The `bug.js` file shows a basic implementation of FlatList rendering 1000 items.  On lower-end devices or emulators, this will noticeably slow down the UI.

## Solution

The `bugSolution.js` file presents potential solutions to mitigate the performance issue, such as using `windowSize` and `removeClippedSubviews` props for optimization.  Additional approaches like virtualization libraries or pagination might be necessary for extremely large datasets.