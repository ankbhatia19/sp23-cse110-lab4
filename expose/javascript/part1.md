## Part 1: A Quick Introduction

1. Line 9 prints the result 20, as expected.
2. Line 13 prints the result 20, which was not expected since I'd originally thought 
that the `var result` would go out of scope after exiting the if statement.
3. Line 9 prints the result 20, as expected.
4. Line 13 returns an error since the variable `result` went out of scope. This is what
I'd originally expected when using the `var` keyword, but it seems that the `var` keyword makes
the variable global to the function, not just the if statement. 
5. Attempting to execute the code returns an error indicating that the variable `result` is a `const` and cannot be 
reassigned a value.
6. Same as 5.