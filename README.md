# CSS Specificity and !important Conflict

This repository demonstrates an uncommon issue in CSS related to specificity and the `!important` declaration. The problem arises when attempting to override a style declared with `!important` using a more specific selector.

## Bug Description

A parent element has a style, then a child element has the same style with `!important` and a more specific selector tries to override it. The `!important` declaration takes precedence despite the selector's specificity.

## How to Reproduce

1.  Open `bug.css`.
2.  Observe the unexpected rendering.
3.  Examine `bugSolution.css` for the resolution.

## Solution

The solution involves refactoring the CSS to avoid using `!important` and leveraging cascading styles effectively.  The approach focuses on using a CSS methodology that minimizes the need for `!important` to enhance maintainability and predictability.