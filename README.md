# Python: Handling ZeroDivisionError in Average Calculation
This repository demonstrates a common error in Python—the `ZeroDivisionError`—that occurs when dividing by zero. The `calculate_average` function is initially vulnerable to this error when passed an empty list. The solution demonstrates a robust way to handle empty input and prevent the error.

## Bug Description:
The original `calculate_average` function fails when provided with an empty list as input, raising a `ZeroDivisionError`. This is because it attempts to divide the sum of the list (which is 0 for an empty list) by the length of the list (which is also 0).

## Solution:
The improved version of the function includes a check for an empty list. If the list is empty, the function returns 0 to avoid the error. Otherwise, it proceeds with the average calculation.