# CSS Specificity Gotcha: Unexpected Color Inheritance

This repository demonstrates a subtle bug related to CSS selector specificity. The bug arises from the unexpected interaction of different selectors, including IDs, classes, and element selectors. The code showcases the various levels of specificity and how they determine which styles are applied.

## Bug Description

The core issue lies in understanding how CSS resolves style conflicts when multiple selectors apply to the same element. The default cascade order might lead to unexpected results, specifically when combining class selectors and ID selectors.

## Bug Reproduction

1.  Clone this repository.
2.  Open `bug.css` and examine the CSS code.
3.  Create an HTML file with the corresponding elements (div, elements with class "container", and the element with ID "specificDiv").
4.  Observe that the element's color will be 'yellow' due to the most specific selector. You might not have anticipated this behavior. 

## Solution

The solution involves a better understanding of CSS specificity and ensuring that selectors are written in a predictable and maintainable way. Refer to `bugSolution.css` for how the selector specificity should be handled correctly.

## Learning Points

- Understanding CSS specificity rules is crucial for avoiding unexpected styling issues.
- Carefully plan and organize your CSS selectors to improve code maintainability and predictability.