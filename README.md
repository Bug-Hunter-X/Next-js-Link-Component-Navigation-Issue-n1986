# Next.js Link Component Navigation Issue

This repository demonstrates a common issue with the Next.js `Link` component where it fails to correctly navigate to the intended page, acting like a standard HTML anchor tag instead.  The issue is likely due to improper usage or a conflict with other parts of the application.  See the `bug.js` file for the problematic code and `bugSolution.js` for the correction.

## Problem Description

The `Link` component, designed for client-side navigation within a Next.js application, is expected to handle routing efficiently without a full page reload. However, in this example, clicking the link behaves as though it were an HTML `<a>` tag, triggering a full page reload and potentially losing application state. This behaviour contradicts the intended functionality of the `Link` component.

## Solution

The solution involves ensuring that the `Link` component is used correctly within the application's context and that no conflicting routing configurations are present.  The `bugSolution.js` file offers a corrected version of the code, showcasing best practices in using the `Link` component.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm run dev` to start the development server.
4. Click the 'About Us' link.  Observe that the page reloads instead of performing a client-side navigation.
