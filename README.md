# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to using `innerHTML` to append elements in HTML.  The example showcases how attempting to append an element created via `createElement` using the `+=` operator with `innerHTML` leads to the element not being correctly added to the DOM.

The solution demonstrates the correct way to append elements using `appendChild`. This approach ensures that the element is correctly added to the DOM and avoids unexpected behavior.

## Bug
The bug lies in the use of `innerHTML += newElement` to append the newly created paragraph.  `innerHTML` replaces the entire content of the target element, hence it's not a suitable method for appending.