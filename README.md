# React Router Dom v6 Catch-all Route Conflict

This repository demonstrates a common issue in React Router Dom v6 related to catch-all routes (`/*`).  When a catch-all route is placed before other routes, it intercepts all requests, preventing other routes from ever being matched. This example shows the problem and its solution.

## Problem

The `/*` route in `App.js` is placed before the `/about` route. This causes the `/about` route to never be matched, resulting in only the `NotFound` component being displayed regardless of the URL.