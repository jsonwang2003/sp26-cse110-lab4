1. line 9 printed: `values added: 20`
2. line 13 printed: `final result: 20`
3. We should not use `var` because the variable declared by `var` will exist anywhere within this function, which can cause confusion and naming conflicts with different scopes
4. line 9 printed: `values added: 20`
5. line 13 printed an error. This is due to the `let` keyword makes it so the variable `result` referable only within the body of the condition. When line 13 trid to print out the `result`, the code could not find a variable `result` that is accessible with its scope.
6. There is an error where line 7 attempted to reassign a `const` variable `result` and the compiler throws a `TypeError`, causing line 9 to not print anything.
7. Similar to line 9, there is no output by line 13 as there was a error from line 7.
8. 