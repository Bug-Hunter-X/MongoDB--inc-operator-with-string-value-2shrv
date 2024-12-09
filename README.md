# MongoDB $inc operator with string value

This repository demonstrates an uncommon error related to the `$inc` operator in MongoDB update operations. The error occurs when a string value is provided to `$inc` instead of a numeric value.

## Bug Description
The code attempts to increment the `count` field in a document using `$inc`, but it passes a string '1' as the increment value.  This results in unexpected behavior, potentially no change or an error depending on the MongoDB version. 

## Solution
The solution corrects the code by passing a numeric value (integer) as the increment value to `$inc`.