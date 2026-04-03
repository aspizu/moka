# Enums

## Definition

supports `export`

```moka
enum Color {
    RED
    GREEN
    BLUE
}
```

## Usage

```moka
color: Color = Color.RED
```

## Methods

```moka
func Color.is_red() -> Bool {
    return self == Color.RED
}
```

## Implementing Interfaces

```moka
func ToString.to_string() -> String {
    match self {
        Color.RED -> "RED"
        Color.GREEN -> "GREEN"
        Color.BLUE -> "BLUE"
    }
}
```
