# Uncommon HTML Bug: Event Listener on Non-Existent Element

This repository demonstrates an uncommon HTML bug related to adding event listeners to elements that don't exist in the Document Object Model (DOM) when the script is executed.

## Bug Description
The bug lies in attempting to add an event listener to an element with the ID 'nonExistentElement' which is not present in the HTML structure.  This can lead to silent failures or unexpected behavior, making it more challenging to debug than common syntax errors.

## Bug Reproduction
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that there is no error message, but the event listener's function never executes.

## Solution
The `bugSolution.html` file provides a corrected version, including a check to ensure the element exists before attaching the event listener.

## Lessons Learned
This bug highlights the importance of:
* Thoroughly checking if elements exist before manipulating them in JavaScript.
* Utilizing browser developer tools to inspect the DOM and identify potential issues.
* Writing robust code that handles potential errors gracefully.