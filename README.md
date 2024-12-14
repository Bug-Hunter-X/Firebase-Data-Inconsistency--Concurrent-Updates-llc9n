# Firebase Data Inconsistency: Concurrent Updates

This repository demonstrates a common issue in Firebase: data inconsistency arising from unsynchronized concurrent updates.  Two clients attempt to increment a counter simultaneously, potentially resulting in incorrect values.

The `concurrentUpdateBug.js` file showcases the problematic code.  The `concurrentUpdateSolution.js` file provides a solution using Firebase transactions to ensure atomicity.

## How to Reproduce

1.  Set up a Firebase project.
2.  Clone this repository.
3.  Replace placeholders with your Firebase configuration.
4.  Run both `.js` files concurrently. Observe the inconsistencies in the first file, and the correct behavior in the second.