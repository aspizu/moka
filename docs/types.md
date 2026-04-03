# Types

## Core Primitive Types

The system utilizes several fundamental types to represent data and execution flow. These types are designed to align closely with standard ECMAScript behaviors while providing clear semantic boundaries.

### `Never`

The `Never` type represents a value that can **never exist**. It is typically used for expressions that are guaranteed to fail or for functions that never finish executing (e.g., a function that always throws an exception or enters an infinite loop). Since it is impossible to instantiate, it serves as a powerful tool for exhaustive type checking.

### `Null`

The `Null` type is a **unit type** used to denote the intentional absence of a value.

- **Unique Value:** The type `Null` contains exactly one value: `null`.
- **Compatibility:** This is functionally identical to the ECMAScript `null` value.

### `Bool`

The `Bool` type represents a logical entity and consists of two distinct values: `true` and `false`.

- **Compatibility:** These correspond directly to ECMAScript boolean values.

### `Number`

The `Number` type is used for numeric data.

- **Compatibility:** This type is equivalent to the standard ECMAScript `Number` type (double-precision 64-bit binary format IEEE 754 values).

### `String`

The `String` type is used to represent textual data.

- **Compatibility:** This type aligns with ECMAScript `String` values, representing a sequence of 16-bit unsigned integer values (UTF-16 code units).
