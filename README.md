# CSS :nth-child Selector and Dynamic DOM

This repository demonstrates a common issue with the CSS `:nth-child(n)` selector when dealing with dynamically added or removed elements.  The `nth-child` selector's functionality depends on the element's position among its siblings, and thus changes in the DOM will affect its selection criteria.

The `bug.css` file shows the incorrect styling, while `bugSolution.css` offers a solution.

## Bug
The problem arises when using `:nth-child` on a list or set of elements where items are added or removed dynamically (e.g., using JavaScript).  The styling will not update correctly, leading to inconsistencies.

## Solution
Instead of relying on `:nth-child`, consider more robust alternatives such as CSS classes applied dynamically through JavaScript.  This approach provides much more control and predictable styling regardless of DOM manipulation.