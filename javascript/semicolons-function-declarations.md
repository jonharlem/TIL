# Semicolons after Function Declarations in Javascript

When I was learning JavaScript I would sometimes (before I was aware of linters) put semicolons following a function declaration. While this is not grammatically incorrect, the semicolons after function declarations are not of any use. 

*This applies to function **declarations**, not function **expressions**

```
function add2 (x) {
	return x+2;
};
```
According to [ecma-international.org](http://www.ecma-international.org/ecma-262/6.0/#sec-function-definitions), function declarations are not terminated by a semicolon. If there is a semicolon--like in the above example--the semicolon is parsed as a separate **empty statement, which doesn't do anything**. Although, empty statements do no harm, they provide zero value.

So when it comes to function declarations...**Leave out the trailing semicolon**.