# Positional Arguments vs. Keyword Arguments
I just learned that in ruby you can have either positional arguments or keyword arguments and would like to consider the usage of both.

## Positional arguments

A simple function that has a single required argument can eliminate the need for a description of each argument.

Consider the function call:
```ruby
prepend_dude("you are awesome")
```

Without looking at the function (defined below) we have a pretty good sense of what the input is used for.
```ruby
def prepend_dude(input)
  return nil unless input.is_a?(String)   # Check to make sure input is a string
  return "dude #{input}"
end
```

I think that this is the only scenario in which keyword arguments are not necessary. 

## Keyword Arguments

If a function's arguments are optional or there is more than one I will always opt for keyword arguments.

Consider the function call:
```ruby
prepend_phrase("you are awesome", "dude")
```

Without looking at the function it is ambiguous which parameter will be prepended to the other. 

```ruby
prepend_phrase("you are awesome", to: "dude")
```
