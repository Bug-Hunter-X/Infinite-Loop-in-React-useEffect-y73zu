# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by improperly using the `useEffect` hook.  The `bug.js` file contains the buggy code. The `bugSolution.js` file provides a corrected version. 

**The Bug:**
The `useEffect` hook attempts to update the `count` state within its own callback.  This creates an infinite loop because each update triggers a re-render, which in turn triggers the `useEffect` again.

**The Solution:**
The solution involves correctly managing state updates within `useEffect`. The corrected code demonstrates appropriate dependency arrays and conditional state updates.

This example highlights the importance of understanding how `useEffect` works and managing its dependencies to prevent common performance issues.