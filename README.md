# React Router v6 Catch-all Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) placed before other routes causes unexpected routing behavior. The catch-all route should always be the last route defined within the `Routes` component. 

## Bug
The `bug.js` file shows an example where the catch-all route is defined before other routes, which prevents the other routes from working correctly. 

## Solution
The `bugSolution.js` file demonstrates the correct way to define routes, with the catch-all route placed last to ensure that it only matches if no other routes are matched.  This ensures that other routes are given priority before resorting to the 404 not found page.