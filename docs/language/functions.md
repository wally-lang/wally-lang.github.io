# Functions

> **Warning**
> Wally is still in development, and the syntax and features are subject to change.

Wally is a functional programming language. This means that functions are first class citizens. This means that functions can be passed as arguments to other functions, and can be returned from other functions. Functions can also be assigned to variables.

## Declaring a function

A function can be declared using the `fn` keyword. The syntax for declaring a function is as follows:

```wally
fn <name>(<args>): <return type> {
    <body>
}
```

Where `<name>` is the name of the function, `<args>` is the arguments of the function, `<return type>` is the return type of the function, and `<body>` is the body of the function.

For example:

```wally
fn add(x: int, y: int): int {
    return x + y;
}
```

## Calling a function

A function can be called using the `()` operator. The syntax for calling a function is as follows:

```wally
<name>(<args>);
```

Where `<name>` is the name of the function, and `<args>` is the arguments of the function.

For example:

```wally
add(5, 10);
```

## Returning a value from a function

A value can be returned from a function using the `return` keyword. The syntax for returning a value from a function is as follows:

```wally
return <value>;
```

Where `<value>` is the value to return.

For example:

```wally
fn add(x: int, y: int): int {
    return x + y;
}
```

## Anonymous functions

Anonymous functions are functions that do not have a name. They can be assigned to variables, and can be passed as arguments to other functions. The syntax for declaring an anonymous function is as follows:

```wally
fn(<args>): <return type> {
    <body>
}
```

Where `<args>` is the arguments of the function, `<return type>` is the return type of the function, and `<body>` is the body of the function.

For example:

```wally
var add = fn(x: int, y: int): int {
    return x + y;
};
```

## Function parameters

A function can have zero or more parameters. The syntax for declaring a function parameter is as follows:

```wally
<name>: <type>
```

Where `<name>` is the name of the parameter, and `<type>` is the type of the parameter.

For example:

```wally
fn add(x: int, y: int): int {
    return x + y;
}
```

## Access modifiers

A functions default access modifier is `pub`. This means that the function can be called from anywhere. But if you want to restrict the access to the function, you can use the `priv` access modifier. The syntax for declaring a private function is as follows:

> Note: Private functions can only be called from within the same module.
> For more information about access modifiers, see the [Access modifiers](../access-modifiers) page.

```wally
priv fn <name>(<args>): <return type> {
    <body>
}
```

Where `<name>` is the name of the function, `<args>` is the arguments of the function, `<return type>` is the return type of the function, and `<body>` is the body of the function.

For example:

```wally
priv fn add(x: int, y: int): int {
    return x + y;
}
```

## Function overloading

A function can be overloaded. This means that a function can have multiple definitions. The syntax for declaring a function overload is as follows:

```wally
fn <name>(<args>): <return type> {
    <body>
}

fn <name>(<args>): <return type> {
    <body>
}
```

Where `<name>` is the name of the function, `<args>` is the arguments of the function, `<return type>` is the return type of the function, and `<body>` is the body of the function.

For example:

```wally
fn add(x: int, y: int): int {
    return x + y;
}

fn add(x: int, y: int, z: int): int {
    return x + y + z;
}
```
