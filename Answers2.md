# Excersises enums3 and strings4
## Enums3
- This code did seem to compile, however, the tests did not pass because `fn process()` was not implemented in the State structure implementation.
- To fix this I implemented `fn process()`
    - I created a match expression with the following lines:
        - `Message::Resize { width, height } => self.resize(width, height),`
        - `Message::Move(point) => self.move_position(point),`
        - `Message::Echo(s) => self.echo(s),`
        - `Message::ChangeColor(red, green, blue) => self.change_color(red, green, blue),`
        - `Message::Quit => self.quit(),`
    - These lines used all the other functions in the State Structure implementation so the elements in the State structure could be modified
