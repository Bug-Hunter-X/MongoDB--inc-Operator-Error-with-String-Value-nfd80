# MongoDB $inc Operator Error with String Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB: providing a string value instead of a numeric one. The `$inc` operator is used to increment a numeric field by a specified value. Attempting to increment with a string will throw an error.

## Bug Description
The provided code snippet uses the `$inc` operator to increment the `age` field. However, it incorrectly provides a string value ('1') instead of a number (1). This leads to an error because `$inc` expects a numeric increment.

## Solution
The solution is to ensure that the value provided to `$inc` is a number, not a string.  The corrected code is shown in `bugSolution.js`.