# Uncommon HTML Bug: Strict Equality Comparison

This repository demonstrates an uncommon bug related to strict equality (===) comparisons in JavaScript code embedded within an HTML file.

The bug arises from the implicit type coercion in JavaScript when using the loose equality operator (==) and not being explicitly aware of type differences while using strict equality (===).

## Bug Description:
The provided HTML file includes a JavaScript script that compares a number (5) and a string ("5") using the strict equality operator (===).  Strict equality checks for both value and type equality, resulting in the script determining that the two values are not equal, when one might expect them to be equal for the purposes of conditional logic.

## Solution:
The solution involves explicitly converting the number or string before comparison to maintain consistency, and provides a more robust and predictable result.