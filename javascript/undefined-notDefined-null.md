# Undefined, not defined, and null
Understanding the difference between undefined and not defined requires understanding the difference between a declaration and a definition:

Trying to use a variable that has not been declared and doesn't exist will throw an error `var name is not defined` and the script will stop. A variable is undeclared when it does not use the `var` keyword. 

`var y` is a **declaration**. You are not defining what the value holds. Instead, you are declaring its existence and the need for memory allocation.

```
var x; // declaring x
console.log(x); // undefined
```

An initialization is both a declaration and a **definition**. The value for variable x is assigned and declared in the same line.

```
var x = 1 // x is defined as 1
```


Variable and function declaration are processed before any code is executed. Because of this, variable and function declarations can appear to be used before they are declared. This is called **hoisting**.

**`null`** is a variable that is defined to have a null value. A variable is rarely defined as `null`, although it can be returned as a value from a function.

---

- `undeclared` variables don't exist
- `undefined` variables exist, but don't have anything assigned to them
- `null` variables exist and have null assigned to them




