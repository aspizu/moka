# Interfaces

## Definition

supports `export`

```moka
inter Greetable {
    func greeting() -> String
}

# default implementation
func Greetable.greet() {
    println(self.greeting())
}
```

## Implementation

supports `export`

```moka
struct Person {
    name: String
    age: Number
}

func Greetable.greeting() for Person {
    return "Hello, my name is " + self.name
}
```

## Usage

```
greetable: Greetable = Person(name: "aspizu", age: 21)
greetable.greet()
```
