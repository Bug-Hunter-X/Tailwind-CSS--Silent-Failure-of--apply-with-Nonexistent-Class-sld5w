# Tailwind CSS: Silent Failure of @apply with Nonexistent Class

This repository demonstrates a subtle bug in Tailwind CSS related to the `@apply` directive.  When using `@apply` with a class that does not exist, Tailwind CSS silently ignores the directive without producing any errors or warnings. This can lead to debugging challenges as the intended styling will be missing without any clear indication of the problem.

## How to Reproduce

1. Clone this repository.
2. Ensure you have Node.js and npm installed.
3. Run `npm install` to install project dependencies.
4. Start the development server (instructions might vary based on your setup).
5. Observe that the div element lacks the expected styling because the `nonExistentClass` does not exist.

## Solution

The solution involves rigorous testing and a thorough review of your Tailwind CSS configuration and your class names to ensure that all `@apply` directives refer to existing utility classes. Linting tools can also help catch these errors during development.  Consider using a dedicated Tailwind CSS linter.