# Exercises lifetime3
## Lifetime3
- This code did not compile because the `Book` struct contains references and Rust requires you to create lifetimes for references within structs. 
- To fix this I added lifetimes to the references
    - To do this I updated the `Book` struct definition to include the lifetime, `Book<'a>`
    - Then I place the lifetime in each of the references, `author: &'a str` and `title: &'a str,`
- This worked as it fixed the compiler error that arose when the references had no lifetimes. 

## Question
Are lifetimes always necessary when dealing with reference? If not, in what situations are lifetimes not required? 