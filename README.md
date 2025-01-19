# Uncommon Tailwind CSS Purge Error with Third-Party Library

This repository demonstrates an uncommon error in Tailwind CSS where the purge feature unexpectedly removes classes used by a third-party library, leading to missing styles.

## Problem Description
The issue arises when using a third-party library that dynamically generates or modifies HTML elements with Tailwind CSS classes. Due to the way Tailwind's purge feature analyzes the application's code, these dynamically added classes may not be included in the final CSS output.

## Solution
The solution involves modifying the Tailwind CSS configuration to explicitly include the necessary classes.  This can be done by adding a `content` array to your `tailwind.config.js` file.

## Reproduction Steps
1. Clone the repository
2. Install dependencies: `npm install`
3. Run the application: `npm run dev`
4. Observe that some styles are missing due to the purge error.
5. Apply the fix described in `bugSolution.js`.
6. Re-run the application to see the solution applied.
