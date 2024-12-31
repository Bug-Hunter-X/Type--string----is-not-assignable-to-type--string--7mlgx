# Type 'string[]' is not assignable to type 'string'

This repository demonstrates a common TypeScript error: assigning an array of strings to a variable expecting a single string.

## Bug

The `greeter` function expects a single string as input. However, the `user` variable is defined as a string array.  Attempting to pass `user` to `greeter` results in a type error.

## Solution

The solution involves ensuring that the correct type is passed to the `greeter` function. This can be achieved by either:

1. Changing the `user` variable to a single string.
2. Modifying the `greeter` function to accept an array of strings and iterate over it or use destructuring to extract the relevant string.