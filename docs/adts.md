# ADTs

## Definition

supports `export`

```moka
struct Some<T> {
    value: T
}

choice Maybe<T> {
    Some<T>
    Null
}
```
