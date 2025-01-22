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
- This code was incorrect and the error given was saying x was not in the scope. The error occured because the variable x did not properly bind to the value 5 as the code was missing the keyword "let"
- The fix for this was to insert the word "let" before x
    - `let x = 5`
    - Note that I could also do something like `let x: i32 = 5`
