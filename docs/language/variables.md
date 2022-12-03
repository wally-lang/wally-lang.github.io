# Variables

> **Warning**
> Wally is still in development, and the syntax and features are subject to change.

A variable in Wally consists of a name, a type and a value. The name is used to refer to the variable, the type is used to determine what kind of value the variable can hold, and the value is the actual value of the variable.

## Declaring a variable

A variable can be declared using the `var` keyword. The syntax for declaring a variable is as follows:

```wally
var <name>: <type> = <value>;
```

Where `<name>` is the name of the variable, `<type>` is the type of the variable, and `<value>` is the value of the variable.

For example:

```wally
var x: int = 5;
```

## Assigning a value to a variable

A variable can be assigned a value using the `=` operator. The syntax for assigning a value to a variable is as follows:

```wally
<name> = <value>;
```

Where `<name>` is the name of the variable, and `<value>` is the value of the variable.

For example:

```wally
x = 10;
```

## Immutable variables

A mutable variable (meaning that the value is not constant, it can be changed) can be declared using the `var` keyword (see above). But if you want to declare a variable as immutable (meaning that the value is constant, it cannot be changed), you can put the `const` keyword in front of the `var` keyword. The syntax for declaring an immutable variable is as follows:

```wally
const var <name>: <type> = <value>;
```

Where `<name>` is the name of the variable, `<type>` is the type of the variable, and `<value>` is the value of the variable.

For example:

```wally
const var x: int = 5;
```