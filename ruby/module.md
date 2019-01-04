# Ruby Module Mixin

Modules are nice because they use composition rather than inheritance. In ruby it is not possible to inherit from multiple classes, so instead we can use modules and mixins. 

Say we have a couple of functions (`hello` and `what_up`) that we want to be easily accessible from classes that already have a super class. We should encapsulate them in a module `GreetingModule` in a file called `greeting_module.rb`:
```ruby
module GreetingModule
  def hello(name)
    puts "Hello #{name}!"
  end

  def what_up(name)
    puts "What up #{name}!"
  end
end
```

Now we can include this module in any class, giving us access to those functions.

```ruby
require_relative '../greeting_module.rb'

class Welcome < SuperClass
  include GreetingModule
  
  def welcome_message(name)
    welcome = what_up("John")
  end
end
```

The welcome class has access to the functions inside of GreetingModule now. 
