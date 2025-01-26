# Unexpected Null Return in Addition Function

This repository demonstrates a common JavaScript bug related to null value handling in an addition function. The initial function returns null if either input is null, which is not always the desired behavior.  The solution provides a more robust approach to managing null inputs.

## Bug Description

The provided `foo` function directly returns `null` when either `a` or `b` is null. While functionally correct, this behavior can be unexpected. A better approach might involve treating `null` values as 0, providing a default value, or throwing an error, depending on the desired functionality.

## Solution

The improved function checks for `null` values and converts them to 0 before performing the addition.  This allows the function to handle `null` inputs gracefully without abruptly returning `null`.