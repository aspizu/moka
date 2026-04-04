# Union

Unions only support union of already defined types. Unions support methods.

## Definition

supports `export`

```moka
struct Some<T> {
    value: T
}

union Maybe<T> {
    Some<T>
    Null
}
```
