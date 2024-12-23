# React Router Dom Unexpected Behavior with Nested Routes and Wildcard Route

This repository demonstrates an unexpected behavior in React Router Dom v6 when using nested routes and a wildcard route ('/*'). The wildcard route is unexpectedly catching routes that should be handled by nested routes.

## Problem

When a wildcard route ('/*') is defined alongside nested routes, the wildcard route incorrectly intercepts routes that should be matched by nested routes. This behavior is inconsistent with expected routing behavior.

## Solution

The solution involves carefully ordering and structuring routes to ensure nested routes are processed before wildcard routes. By placing the wildcard route at the end of the route definition in the `Routes` component, the issue is resolved, as nested routes are prioritized.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.

Observe the unexpected behavior in the initial version. Then, compare it to the fixed version.