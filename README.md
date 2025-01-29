# CSS Specificity Bug

This repository demonstrates a common issue related to CSS selector specificity. The provided CSS code intends to style list items, but due to a more specific selector, only list items within a particular element are styled, unexpectedly overriding the more general style rule.

The `bug.css` file contains the buggy code, while `bugSolution.css` shows the corrected version.

The bug arises from the differing specificity of the selectors. The selector `nav li` has higher specificity than the selector `li`, causing the latter to be overridden even though it appears earlier in the stylesheet.