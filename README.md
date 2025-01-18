# CSS `:nth-child` Selector Issue with Dynamically Added Elements

This repository demonstrates a common issue encountered when using the CSS `:nth-child(n)` selector with dynamically added elements. The selector doesn't always apply correctly to elements added to the DOM after the initial page load.

## Bug Description

The `bug.css` file contains a CSS rule that uses `:nth-child(n)` to style list items. However, when list items are added dynamically using JavaScript (not shown here, only relevant for context), the styling doesn't update correctly for the newly added items.

## Solution

The solution in `bugSolution.css` demonstrates how to work around this limitation.  Instead of relying on `:nth-child`, we use a class-based approach, dynamically adding classes to elements.  This approach avoids the complexities of `:nth-child` with dynamic content, leading to more reliable styling behavior.
