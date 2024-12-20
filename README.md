# JavaScript NaN Comparison Bug

This repository demonstrates a common error in JavaScript related to comparing NaN (Not a Number) values using loose comparison (==).  NaN is unique in that it's not equal to itself.

## Bug Description:
The `foo` function attempts to check if two numbers are equal. However, due to JavaScript's handling of NaN, it incorrectly returns `false` even when both inputs are NaN.

## Solution:
The solution uses the `Number.isNaN()` function to explicitly check if a value is NaN before performing the comparison.