# :focus-visible CSS Pseudo-class Incompatibility

This repository demonstrates a common issue with the CSS `:focus-visible` pseudo-class:  incompatibility with older browsers.  The `:focus-visible` pseudo-class is intended to only style elements when they receive focus in a way that's visually apparent to the user (not just programmatically).  However, older browsers lack support, leading to styling issues.

## Bug

The `bug.css` file contains CSS that uses `:focus-visible`.  In modern browsers, this works as expected. In older browsers, the styles are applied regardless of whether the focus is visually apparent, potentially leading to unexpected visual behavior or accessibility issues.

## Solution

The `bugSolution.css` file offers a solution using feature detection and alternative styling.  It checks for support of `:focus-visible` before applying styles, providing fallback styling for older browsers to maintain consistency and functionality.