When a non boolean is coerced into a boolean, does it become `true` or `false`?

Non booleans that become `false` are called `falsy`, non booleans that become `true` are called `truthy`.

# Falsy Values

- `""` - empty string
- `0`, `-0`, `NaN` - zero & invalid number
- `null`, `undefined`
- `false`

# Truthy

Any value that is not falsy is truthy. For example:

- `"hello"`
- `42`
- `true`
- `[]`, `[1, 2, 3]` - arrays
- `{}`, `{first: "Michael", last: "Scott"}` - objects
- `function foo() { ... }` - functions
