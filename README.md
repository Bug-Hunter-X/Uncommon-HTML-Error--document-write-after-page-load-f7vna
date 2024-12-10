# Uncommon HTML Error: document.write() After Page Load

This repository demonstrates a subtle but potentially problematic error in HTML involving the use of `document.write()` after the page has finished loading.  Improper usage of this method can lead to unexpected rendering issues or errors.

## The Bug

The `bug.html` file contains a `document.write()` call placed within a `<script>` tag.  If the script executes after the HTML document has completely loaded, using `document.write()` can overwrite the existing HTML content, causing unexpected behavior.

## The Solution

The `bugSolution.html` provides a corrected version. Instead of `document.write()`, it leverages DOM manipulation to dynamically add content. This approach is more robust and reliable, ensuring consistent rendering regardless of script execution timing.