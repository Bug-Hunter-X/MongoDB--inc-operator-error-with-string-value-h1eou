# MongoDB $inc operator error with string value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string value is provided instead of a number, the operation will fail.

## Bug Description
The provided code uses the `$inc` operator with a string value ('1') instead of a numeric value (1). This results in a MongoDB error.

## Solution
The solution involves changing the provided value to a number to fix the error.  This ensures that the operation will increment the field correctly.

## How to reproduce
1. Clone this repository.
2. Ensure you have a MongoDB instance running.
3. Run `bug.js`.  You'll see an error. 
4. Run `bugSolution.js`. This will correctly increment the counter.