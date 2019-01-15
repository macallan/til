# Equality

The difference between `==` and `===` is something that I have never felt confident in.

Kyle Simpson explains this extremely well in [You Don't Know JS](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md):

> The difference between == and === is usually characterized that == checks for value equality and === checks for both value and type equality. However, this is inaccurate. The proper way to characterize them is that == checks for value equality with coercion allowed, and === checks for value equality without allowing coercion; === is often called "strict equality" for this reason.
