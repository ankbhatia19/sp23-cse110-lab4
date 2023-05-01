

1. At line 12, the variable `i` is printed, which at this point should be equal to the
length of the list `prices`. Since the length of the list `prices` is 3 in this example,
we expect line 12 to print 3. This works because the variable `i` is declared with the `var` keyword,
which makes it global to the function `discountPrices`.
2. The variable `discountedPrice` will store the result of the final loop executed in the `for` loop,
which is the last element in the list `prices` multiplied by the discount rate. In this case, the last
element in the list `prices` is 300, and the discount rate is 0.5, so the result is 150. This works because
the variable `discountedPrice` is declared with the `var` keyword, which makes it global to the function `discountPrices`.
3. The variable `finalPrice` will store the result of `discountPrice` multiplied by 100, rounded to the nearest integer, then divided by 100.
In this case, the result is 150. Although I do wonder why multiplying by 100, rounding to the nearest integer, then dividing by 100 is necessary.
4. Although nothing will be printed since all `console.log()` statements are commented out, the function `discountPrices` will return a list
containing the discounted price of each element in the list `prices`. In this case, the list returned will be `[50, 100, 150]`.
5. At line 12, the variable `i` is not defined since we are using the `let` keyword now, which causes the variable `i`
to go out of scope after the for loop terminates.
6. The variable `discountedPrice` is not defined since we are using the `let` keyword now, which causes the variable `discountedPrice`
to go out of scope after the for loop terminates.
7. The variable `finalPrice` is still defined since its declaration is outside the for loop, so it is still in scope.
Hence, it prints normally and returns the value 150.
8. The function `discountPrices` will return a list containing the discounted price of each element in the list `prices`. In this case, the list returned will be `[50, 100, 150]`.
Although initially it looked like this would not be the case since the variable `discountedPrice` is not defined, the variable `discounted` was declared using `let`,
it will return the intended values.
9. The variable `i` goes out of scope since it is defined using the `let` keyword.
10. The number 3 will be printed since the variable `length` is still within scope.
11. The function `discountPrices` will return a list containing the discounted price of each element in the list `prices`.
It is no different from returning another variable declared using `let` or `var`.
12. Answers A-E are written below:
    1. `student.name;`
    2. `student['Grad Year'];`
    3. `student.greeting();`
    4. `student['Favorite Teacher'].name;`
    5. `student.courseLoad[0];`
13. Answers A - H are written below:
    1. `'3' + 2 = '32' `
    2. `'3' - 2 = 1 `
    3. `3 + null = 3`
    4. `'3' + null = '3null' `
    5. `true + 3 = 4 `
    6. `false + null = 0`
    7. `'3' + undefined = '3undefined'`
    8. `'3' - undefined = NaN`
14. Answers A - F are written below:
    1. '2' > 1 = true
    2. '2' < '12' = false 
    3. 2 == '2' = true 
    4. 2 === '2' = false 
    5. true == 2 = false 
    6. true === Boolean(2) = true
15. The `==` operator checks for equality after converting both operands to a common type, 
whereas the `===` operator checks for equality without converting the operands to a common type.
16. Answer is written in `part2-question16.js`
17. At the end of executing `modifyArray`, a new array is returned in which all elements in the array will be twice their original value. 
This is because the `modifyArray` function executes a callback for each element in the array that returns the current number
multiplied by 2. The callback function is specified by a parameter.
18. Answer is written in `part2-question18.js`
19. Ideally, the function prints the integers in the order `1 3 4 2` because the `setTimeout` call with a delay of
0 ms should in theory operate instantaneously. However, based on the output, it seems that the `setTimeout` call has an effect
on the order of the print statements. This is because the `setTimeout` call is asynchronous, so the print statements are
executed before the `setTimeout` call is executed. Hence, the print statements are executed in the order `1 4 3 2`.