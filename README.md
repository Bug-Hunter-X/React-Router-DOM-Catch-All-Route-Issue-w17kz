# React Router DOM Catch-All Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router DOM v6. The catch-all route unexpectedly intercepts all navigation attempts, even when more specific routes exist.

## Problem

The provided `App.js` showcases a simple React Router setup.  Despite having routes for `/` and `/about`, the catch-all route `/` always renders, preventing access to other routes. 

## Solution

The solution, in `AppSolution.js`, demonstrates how to correctly position the catch-all route. By placing it last, React Router correctly handles route matching before falling back to the catch-all.