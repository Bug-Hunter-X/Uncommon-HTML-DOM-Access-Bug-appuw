# Uncommon HTML DOM Access Bug

This repository demonstrates an uncommon bug in HTML related to accessing a DOM element before it's fully loaded into the Document Object Model (DOM). Attempting to manipulate an element before it exists results in a runtime error.

## Bug Description

The bug is caused by trying to access and modify the `innerHTML` property of the element with the id `myDiv` before the browser has finished parsing and rendering the HTML.

## Solution

The bug is fixed by using the `DOMContentLoaded` event listener. This event fires when the HTML document has been completely loaded and parsed, but before any external resources (like images or scripts) have been loaded.