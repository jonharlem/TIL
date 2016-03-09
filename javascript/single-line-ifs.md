# Single-line 'if' statements

There are a lot of strong opinions writing single line 'if' statements. Javascript allows you to not use curly braces when only one statement is guarded by the 'if' statement.

```
if (x < 10)
	doSomething();

/* is the exact same as...*/
if (x < 10) {
	doSomething();
}
```

 While it can be tempting, since it saves time and keystrokes, it is not ideal for maintainability and readability. If you accidentally add a second statement to the 'if' block, without the curly braces, the additional statement will run regardless of the block's condition. This can create a tough bug to catch if it is indented like the existing 'if' statement. 

 ###The Solution

 The problem exists when the 'if' statement is broken up into two lines. The compiler sees this as a singular statement guarded by a single condition.

To solve the problem, if the statement you are writing is small and not worth the 'heft' of the curly braces, just keep it on one line.

```
if (x < 10) doSomething;
```