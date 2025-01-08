# Unexpected NaN Result from Undefined in JavaScript Function

This repository demonstrates a common JavaScript error involving the handling of `null` and `undefined` values in function arguments.  The function `foo` correctly handles `null`, but produces an unexpected `NaN` result when passed `undefined`.

## Bug Description
The JavaScript function `foo` is designed to return 0 if the input `x` is `null` and `x + 1` otherwise. While it correctly handles `null`, it unexpectedly returns `NaN` when called with `undefined` due to attempting arithmetic on `undefined`.

## Solution
The solution involves explicitly checking for both `null` and `undefined` and handling them appropriately to prevent the `NaN` result.