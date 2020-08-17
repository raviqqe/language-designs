# Python-like language

- [Type system](type_system.md)

## If statement

```
if foo
  bar()
else if baz
  qux()
else
  quux()
```

## For statement

### With iteration

```
for i in range(0, 42)
  foo()
```

### With condition

```
for foo
  bar()
```

## Switch statement

- Type switch

```
switch foo
case String
  bar()
case None
  baz()
default
  qux()
```

### Jump statements

```
break
continue
```

## Function definition

```
func foo(x Number)
  bar()
```

### Closure definition

```
func foo(x Number)
  func bar()
    return x

  return bar
```

## Variable definition

```
var foo Number = 42
```

## Exporting names

- By capitalization

```
func Foo() String
  return "foo"

var Bar Number = 42
```

## Import statement

```
import "github.com/foo/bar"
```

## Error handling

- `?` operator

```
func foo() None | Error
  bar()?
```
