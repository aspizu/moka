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
    switch self {
        case Color.RED {
            return "RED"
        }
        case Color.GREEN {
            return "GREEN"
        }
        case Color.BLUE {
            return "BLUE"
        }
    }
}
```
