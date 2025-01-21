# Tailwind CSS @apply Directive Variable Resolution Issue

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to properly resolve variables when applied to custom styles.

## Bug Description

When using `@apply` with custom styles containing variables, the variables are not resolved, leading to the styles not being applied correctly or at all.

## Reproduction

1. Clone this repository.
2. Open `bug.css` to see the buggy implementation.
3. The expected outcome is that the `.container` class should have the styles defined by the `@apply` directive.
4. The actual outcome is that the styles are not applied because the variables are not resolved correctly.
5. Open `bugSolution.css` to view the proposed solution.

## Solution

The solution involves ensuring that variables are correctly defined and accessible within the scope where the `@apply` directive is used.  In the solution file (`bugSolution.css`), the variables are defined within the custom style declarations.