# Explain the difference between any, unknown, and never types in TypeScript.

## Core Type Differences

### `any` Type
- **Purpose**: Opt-out of type checking
- **Behavior**: Allows assignment from/to any type without compilation errors
- **Use Case**: Migration from JavaScript or when type is truly dynamic
- **Risk**: Loses all type safety benefits


### `unknown` Type
- **Purpose**: Type-safe counterpart to any
- **Behavior**: Accepts any value but requires type checking before use
- **Use Case**: When type is uncertain but safety is desired
- **Risk**: Forces type narrowing before operationss

### `never` Type
- **Purpose**: Represent values that never occur
- **Behavior**: Cannot have any value assigned
- **Use Case**: Exhaustive checks, infinite loops, always-throwing functions
- **Risk**: Ensures unreachable code is properly handled




# What is the use of enums in TypeScript? Provide an example of a numeric and string enum.

## TypeScript Enums

Enums in TypeScript are used to define a set of named constants, which can be numeric or string-type. Enums are a basic way to manage sets of related values and can simplify code readability and maintenance.


### `Numeric` Enums
TypeScript enums are numeric by default. Each enum member gets a numeric value, with the first default value being 0 and each member following it incrementing by 1.


### `String` Enums
String enums allow each member to be associated with a string value. This comes in useful if you need to be able to represent a group of related string values.

## Benefits of Using Enums

- **Readability**: Enums provide meaningful names to sets of related values, making the code more readable.
- **Maintainability**: Enums help in managing sets of constants in a centralized manner.
- **Type Safety**: Enums provide compile-time checking, reducing the chances of errors.