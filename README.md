# Unexpected String Concatenation in JavaScript

This repository demonstrates a common JavaScript bug caused by the language's loose typing system.  The `+` operator in JavaScript behaves differently depending on the types of operands. If one operand is a string, it performs string concatenation instead of numeric addition, resulting in unexpected output.

## Bug Description

The `foo` function is intended to add two numbers. However, when a number and a string are passed, it concatenates them as strings.

## Solution

The solution involves using the `parseInt()` or `parseFloat()` functions to explicitly convert string operands to numbers before performing the addition. This ensures that the `+` operator performs arithmetic addition as intended.