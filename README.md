# MongoDB $inc Operator Error: String Increment

This repository demonstrates a common error when using the `$inc` operator in MongoDB: attempting to increment a field with a string value instead of a number.

The `bug.js` file contains code that reproduces the error. The `bugSolution.js` file shows the correct way to use the `$inc` operator.

## Bug
The original code incorrectly tries to increment the `counter` field by the string value "1".  This is not supported by MongoDB.

## Solution
The solution involves providing a numeric value to the `$inc` operator, ensuring that the field to be incremented is also a number.