# Structs

## Definition

struct supports `export`, struct fields support `export`. struct fields are exported per-module.

```moka
export struct Person {
    export name: String = "aspizu"
    export age: Number = 21
}
```

struct default values are evaluated at the time of struct instantiation.

## Instantiation

```moka
# positional style
person = Person("aspizu", 21)
# keyword style
person = Person(name: "aspizu", age: 21)
```

## Methods

```moka
export func Person.greeting() -> String {
    return "Hello, my name is " + self.name
}
```

## Generic structs

```moka
export struct List<T> {
    export items: Array<T> = []
}

export func List.add(item: T) {
    self.items.add(item)
}
```
