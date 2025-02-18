# Incorrect $inc operator usage in MongoDB
This example demonstrates an incorrect usage of the `$inc` operator in MongoDB. The `$inc` operator is used to increment a numerical field by a specified value. However, in the given example, a string value ('1') is provided instead of a number (1). This will result in an error. 

## Bug
The bug lies in the incorrect usage of the `$inc` operator.  Instead of incrementing the `field` by 1, the provided code tries to increment it by the string '1'.  MongoDB expects a numerical value for this operation.

## Solution
The correct way to increment the field is to provide a numerical value to `$inc`, like shown in `bugSolution.js`
