# Python-like language

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
  bar
```

## Switch statement

```
switch foo
case String
  bar()
case None
  baz()
default
  qux()
```

### Special statements

```
break
continue
```

## Function definition

```
func foo()
  foo
```

## Variable definition

```
var foo String = "foo"
```

## Export annotation

```
export func foo() String
  return "foo"

export var bar String = "bar"
```
