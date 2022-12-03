# Access Modifiers

> **Warning**
> Wally is still in development, and the syntax and features are subject to change.

Wally has two access modifiers: `public` and `private`. These are used to control the visibility of classes, functions, and variables.

## Public

A public member is accessible from anywhere. This is the default access modifier for classes and functions.

## Private

A private member is only accessible from within the class that it is declared in. This is the default access modifier for variables.

## Examples

```java
class Person { // public by default
    priv var name: string; // This variable is private
    pub var age: int; // This variable is public

    constructor(name: string, age: int) {
        this.name = name;
        this.age = age;
    }

    pub fn getName(): string {
        return name;
    }

    pub fn setName(newName: string): void {
        name = newName;
    }

    pub fn getAge(): int {
        return age;
    }

    pub fn setAge(newAge: int): void {
        age = newAge;
    }

    pub override fn toString(): string {
        return "Name: " + name + ", Age: " + age;
    }
}
```