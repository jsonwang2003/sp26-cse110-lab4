1. line 12 will print the number `3`. There is no error due to the variable `i` being declared using the keyword `var`, which is accessible by anywhere within the function `discountPrices`. With each iteration of the loop updates `i`, the varaible `i` will hold the value of the number of prices being processed. In this example, there are 3 prices to discount so line 12 prints out 3.
2. line 13 will print the last discounted price processed by the loop. There is no error due to the `var` declaration with the variable `discountedPrice`. With line 13 printing after the loop terminates, the discountedPrice remains there which holds the value that the last iteration of the loop processed. In this example, the last price was 300 with 50% off gives back 150.
3. line 14 will print the last price finalized by rounding. There is no error due to the `finalPrice` was decalred with `var` instead of `const`. With line 14 printing after the loop terminates, the `finalPrice` variable will hold the rounded result of the last `discountedPrice`. In this case, the `discountedPrice` equals 150 without decimals, which rounding gives back the same 150.
4. The function returns a list of discounted prices in the order given to the function. Since for each price was calculated and applied the discount and push into `discounted` in order, the returned price also will be in the order that was given. There are no errors as the `discounted` variable is declared by `var` and therefore accessible by `return` statement.
5. At line 12, there will be an error since the variable `i` is only accessible by the for-loop. line 12 cannot access/find the variable `i` at the scope it is at.
6. At line 13, there will also be an error since the `discountedPrice` is also only accessible inside the for-loop. Line 13 cannot access `discountedPrice` and throws a reference error.
7. At line 14, there will be no error since `finalPrice` is within the same scope as line 14. 
8. The function will return a list of discounted prices in the order given to the function, just like the version with `var` variables
9. At line 12, there will be an error since the variable `i` is only accessible by the for-loop. line 12 cannot access/find the variable `i` at the scope it is at.
10. At line 13 will print 3 as that is the number of prices being processed by the function. There is no error as the `console.log` is just reading the value in `length`, not changing the value.
11. The function will return normally as others do. This is due to none of the variables are trying to be reassigned with different values. `discounted` is just adding an element, not changing the data structure; `length` is never reassigned. `discountedPrice` though goes through the loop and technically holded different values in different iteration of the loop, they don't constitute as reassignment.
12. Here are the notations:
  - A) student.name
  - B) student["Grad Year"]
  - C) student.greeting()
  - D) student["Favorite Teacher"].name
  - E) student.courseLoad[0]
13. Arithmetic
  - A) '3'+ 2 = '32' since '3' is a string and it converts the overall result into a string where the `+` acts as an concatenation operation instead of add
  - B) '3' - 2 = 1 since `-` is not supported by string, the '3' is converted into a number
  - C) 3 + null = 3 since `null` is treated as the number 0 when type casted
  - D) '3' + null = '3null' since `null` is converted to a string literal as '3' is a string
  - E) true + 3 = 4 since true is converted to the number 1 when type casted
  - F) false + null = 0 since false is converted to the number 0 and null is also treated as 0 when type casted
  - G) '3' + undefined = '3undefined' since undefined is converted to a string literal as '3' is a string
  - H) '3' - undefined = NaN since `-` is not recognized as a string operation which converts both operand to a number and undefined is always treated as NaN, forcing the result to be NaN.
14. Comparisons
  - A) '2' > 1 = true sine '2' is converted to number 2 and 2 is greater than 1
  - B) '2' < '12' = false since both operands are string, the comparison is done by lexicographical order and '2' is greater than '1'
  - C) 2 == '2' = true since '2' is first converted to number 2 and 2 equals 2
  - D) 2 === '2' = false since `===` does not perform type casting and so a number is not equal to a string
  - E) true == 2 = false since true converts to number 1 and 1 is not equal to 2
  - F) true === Boolean(2) = true since `Boolean(2)` evaluates to true as 2 > 0, and true === true with same value and same type
15. `==` does automatic type casting before actually evaluating the comarison; `===` on the other hand does not do type casting, it checks for the type of the 2 operands first and returns false if the types don't match.
17. First the `newArr` is created and for each element in the array, run the callback function and append it to the `newArr`. The callback function just returns the double of the value inputed. With the array being [1, 2, 3], new array will be [2, 4, 6].
19. 1 4 3 2
20. 