# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook causing an infinite render loop.  The component renders continuously, leading to performance issues and console spam. The solution showcases how to correctly use the dependency array to prevent this.

## Bug
The `bug.js` file contains the buggy code where the `useEffect` hook lacks a dependency array, triggering the effect on every render.  This leads to the `console.log` statement executing repeatedly. 

## Solution
The `bugSolution.js` file provides the corrected code. By including `[count]` as the dependency array, the `useEffect` hook now only runs when the `count` variable changes.