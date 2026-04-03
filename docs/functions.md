# Functions

## Definition

Functions support `export` Function names should be in snake_case.

```moka
func factorial(n: Number) -> Number {
    if n == 0 {
        return 1
    }
    return n * factorial(n - 1)
}
```

### Default argument values

The expression is evaluated at the time of function calling.

```moka
func factorial(n: Number = 1) -> Number {}
```

## Calling

```
# positional arguments
factorial(10)
# keyword arguments
factorial(n: 10)
```

## main function

exporting a main function makes a module executable

```moka title="MyScript.moka"
export func main() {

}
```

```bash
moka run MyScript.moka
```
