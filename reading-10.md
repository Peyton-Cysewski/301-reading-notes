# Reading Notes 10

## The Call Stack

The call stack is what interpreters use to understand where its place is in a script, keeping track of functions and what other functions are being called from inside other functions. Once a function has been completed, then it is removed from the call stack and the script progresses forward. A stack overflow error occurs when a the allotted room for stack runs out. This is most common with functions that recursively call themselves with no end condition.

## Errors

- Reference - when a variable has not been declared yet, the computer does not know what it is or where to find it
- Syntax - when a function is meant to be written a certain way, but it cannot read it due to a stray character, for example
- Range - certain data types have set ranges that, for example, cannot be negative
- Type - some operations are data type specific where they only work correctly on specific datas

Catching errors is also very important. To add stability to code, being able to catch an error and move on allows the functionality to continue. The most common way of doing this is with a try...catch statement. There may be some unforseen side effects if the code isn't written carefully, but it should allow it to be functional even if an error occurs somewhere down the line.

Linters that look for syntax errors are very helpful when trying to write code. They can be add-ons but are often built into some of the bigger text editors.



#### [Home](README.md)