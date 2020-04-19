# Reading Notes 09

## Functional Programming

Functional programming is a structure of programming that avoids mutability and state-changing. This type of programmign uses pure functions that are deterministic in nature with no side effects. One common mistake is to use global variables that are passed into functions. If that global varible was ever different, then it would cause a side effect on the function. This can be changed by passing that global variable as an argument into the function. For the same reason, reading an external file that can change is not a pure function. As far as side effects go, passing in a parameter by reference would change the origin variable. Instead, a copy of the variable should be passed in: by value.

## Refactoring

Having code that is easy to read is very important. If possible, re-write your code in a way that does not hamper its efficiency and makes the understandability somewhat reasonable. It does not need to be easily readable ot the lehman, but having some concepts easier to read, like nested loops, woudl be a huge deal. It allows people to quickly grasp what is going and perhaps contribute to what has been written.



#### [Home](README.md)