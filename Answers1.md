# Sections 00 (Intro) to 05 (Vecs)

## Section 00
### Intro1
- This code did compile as it was not meant to have anything wrong
- I did add another print line though just for fun
### Intro2
- This code did not compile because the name of the print line function was incorrect
    - The name they used was `printline!("Hello world!")`
- I fixed this by using the proper function name for print line
    - The correct name is `println!()`

## Section 01
### Variables1
- This code was incorrect and the error given was saying x was not in the scope. The error occurred because the variable x did not properly bind to the value 5 as the code was missing the keyword "let"
- The fix for this was to insert the word "let" before x
    - `let x = 5`
    - Note that I could also do something like `let x: i32 = 5`
### Variables2
- This code declares a binding for x but does not actually bind anything to x
    - The declaration is `let x;` which does not bind anything to x
- The fix for this is to give x a value
    - I gave x the value 10 by changing the declaration to `let x: i32 = 10`
### Variables3
- This code does not compile because x's binding is not initialized. A value was never given to x similar to the problem before
- The fix is to give x a value
    - I gave x the value 42 by changing the code to `let x: i32 = 42`
### Variables4
- This code does not compile because x was not declared mutable
- To fix this I changed the code to `let mut x = 3` which makes x mutable
### Variables5
- This code does not compile because number is of type str in the first declaration so the line `number = 3` causes a type mismatch error
- To fix this I added the keyword "let" to that line of code so it now reads `let number = 3`
    - I think this worked because the new declaration shadowed the old declaration of `let number = "T-H-R-E-E"`
    - It is my understanding that even though number was not declared mutable, it was able to be shadowed when the type was change to int
### Variables6
- This code does not compile because in rust, constants must be typed when declared and the code given does not do this
- The fix is to give the constant a type like this `const NUMBER: i32 = 3`

## Section 02
### Functions1
- The function call_me() was never defined in the scope which causes this code to not compile.
- The fix was to define a function call_me()
    - `    fn call_me() {println!("Call me!");}`
### Functions2
- This did not compile because the parameter for the function was not given a type
- The fix is to provide the parameter with the proper type so in this case `num: i32`
    - Note that I also put `-> ()` after the argument declaration which is not require but is just specifying that nothing is returned
### Functions3
- This code did not compile because the function call did not include an argument which is declared in the function
- To fix this, I added a number to the function call, `call_me(4)`
### Functions4
- This code did not compile because a return type was expected for the function but not provided
- The fix was to add the proper return type in the function declaration like so, `fn sale_price(price: i64) -> i64`
### Functions5
- This code did not compile because a return type was declared but the function did not return a value. When a semicolon is put at the end of a line that is not specified as a return statement, the line will not return anything. 
- There are a couple ways to fix this:
    - The change I made was to add return like so `return num * num;`
    - Another option is to remove the semicolon, `num * num`
    - You may also remove the semicolon and add return, `return num * num`

## Section 03
### if1
- This code does not compile because a function is declared but is not really implemented. My job is to implement it.
- 