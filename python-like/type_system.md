# Type system

- Nominal typing
- Restricted polymorphism

## Types

### Primitives

```
Boolean
None
Number
String
```

#### Literals

```
False
True
None
42
-42
"String"
```

### Functions

```
func(Number, String) Number
```

### Arrays

```
[]a
```

#### Operations

```
array[1]
array[1...42]
[ ...array, 42 ]
[ 42, ...array ]
```

### Records

- Elements are hidden outside the modules where they are defined.

```
type Person {
  name : String,
  age : Number,
}
```

#### Operations

```
person.name
Person{ name = "foo", age = 42 }
Person{ ...person, name = "bar" }
```

### Enumeration

```
type Foo
```

### Unions

```
Foo | Bar | Baz
```

### Any

```
Any
```

### Error

```
type Error {
  context : Any,
}
```

## Type coercion

```
x.(Number) # Number | Error
```

## Type alias

```
type Foo = Bar
```
