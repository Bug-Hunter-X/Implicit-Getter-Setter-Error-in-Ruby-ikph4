# Ruby Implicit Getter/Setter Bug

This repository demonstrates a common error in Ruby related to implicit getter and setter methods.  New Ruby developers frequently stumble upon this issue when they expect the language to automatically create instance variables.

## The Bug

The `bug.rb` file contains a simple class with an instance variable `@value`.  The `value` method acts as an implicit getter. However, attempting to assign a new value directly through `my_object.value = 20` fails because there is no implicit setter method created. This results in a `NoMethodError`.

## The Solution

The solution, shown in `bugSolution.rb`, uses an explicit setter method `value=` to handle assignments correctly.