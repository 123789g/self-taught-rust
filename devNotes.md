## Goals
  1. Become proficient enough to fix my own problems.
  2. Gain a stronger confidence in my backend abilities.
  3. Contribute that Grappling Hook idea I have to Veloren.

## General Thoughts
  1. The Rust compiler is strict but it is very easy to read.
  2. I have no clue what the signifigance of having precise annotations is. How many MB of ram do I save? Can I even percieve it? Why not make every data annotation the biggest and be done with it?

## Data Type Annotations
  Rust requires most variables to be attatched to a data type annotation.
  Example | let number: u8 = 10
  For **intergers**
    i8, i16, i32, i64, i128
    u8, u16, u32, u64, u128
    *i# means it can be negative. u# means it cannot.*

## Variables
  By default, the variable prefix, **let**, is immutable. For mutability, or the re-use of a variable, you must add mut before the variable name.
  Example | let mut number: u8 = 10
  For **Strings** this does NOT seem to be the case.

## Shadowing
  As we know, let is immutable. The value within it cannot be changed. But within functional programming paradigms, they get around this by running the variable into it's own function that modifies it in some way.
  Example | let number: u8 = 10 -> let number = number + 1

## Concatination
  Concat, or adding values, is a bit tricky in Rust as you cannot just bind 2 strings together with the + symbol. No, you must add a bit - **.to_owned()**
    I don't know what this does, but it's important or something.
  Example | println!(number.to_owned() + "Oh fr?");

## Functions
  Functions are called with **fn** as opposed to Python's **def** or JS's **function**.
  It goes without saying, but you must have initilized/created the function somewhere BEFORE you use it.

  The entire line that makes up a function's head is called it's **signature**.
    Example | "fn call_me(num: u32) {}".

  Function returns shouldn't use a **;**. Or if they do, they should explictily say **return x;**
