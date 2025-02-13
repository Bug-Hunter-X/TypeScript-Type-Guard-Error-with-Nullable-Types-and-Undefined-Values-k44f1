# TypeScript Type Guard Error with Nullable Types and Undefined Values

This repository demonstrates a common error in TypeScript related to type guards and undefined values when working with nullable types.

## The Bug
The `greet` function is designed to handle null values gracefully. However, if an undefined value is passed, the type guard doesn't prevent a runtime error.

## The Solution
The solution involves explicitly checking for undefined values in addition to null values.  This ensures that the function handles all potential scenarios without throwing errors.

## How to reproduce
1. Clone the repository
2. Run `tsc bug.ts` to compile the buggy code
3. Run `node bug.js` to see the runtime error
4. Run `tsc bugSolution.ts` to compile the fixed code
5. Run `node bugSolution.js` to see the corrected output