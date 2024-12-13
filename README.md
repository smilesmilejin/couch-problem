# couch-problem
Problem to be completed during Industry Prep - Interview Prep activity time

## Problem Statement

The first patent for a folding bed was awarded to Sarah E. Goode in 1885. She was a former slave and the first Black woman to receive a patent. Shortly after, Leonard C. Bailey, a Black inventor, was awarded a patent for a piece of furniture that could be converted between a bed and a couch. Today, this is commonly called a sleeper sofa.

Your goal will be to write classes to model sleeper sofas and sheets to put on them.

### Wave 1

Provided for you is a `Couch` class. This `Couch` class should NOT be modified. Instead, you should make a new class, SleeperSofa that is a subclass of `Couch`.

Each sleeper sofa should have four instance variables, `length` and `width`, `folded_out`, and `sheets`.

`length` and `width` should be numbers that represent the current dimensions of the sofa. `folded_out` should be a boolean representing whether the sofa is currently folded out to be a bed. `sheets` should hold a reference to the sheets currently on the sofa, or None if there are currently no sheets.

The sleeper sofa's constructor should take a length and width. It should begin NOT folded out and with no sheets on.

### Wave 2

You should add an instance method to SleeperSofa, `convert`. This method invert the boolean value of `folded_out`.

Additionally, when folding out the sleeper sofa, its width should be doubled. When folding the sleeper sofa back in, its width should be halved.

### Wave 3

You should create a class, Sheets. This class should have an instance variable `material` that holds a string representing what material the sheets are made out of.

The Sheets constructor should take one optional argument, material. If it is not supplied, the material should default to "cotton".

You should add two methods to SleeperSofa: `put_on_sheets` and `remove_sheets`.

`put_on_sheets` should accept an argument, `sheets`. If the sofa is folded out AND there are not any sheets currently on the sofa, `put_on_sheets` should set the sofa's sheets to the sheets passed in. However, if there are already sheets on or the sofa is not folded out no action should be taken.

`remove_sheets` should set the sofa's sheets to None.

### Wave 4

Modify the `convert` method on sleeper sofa so that the sofa can only be folded back in if there are currently no sheets on the sofa.

Sleeper sofa history source: https://science.howstuffworks.com/innovation/everyday-innovations/who-invented-the-sleeper-sofa.htm

## Notes for the Interviewer

### Delivery Notes

#### THIS QUESTION IS MEANT TO BE DONE ONE WAVE AT A TIME!

- Please only explain the first wave to your interviewee first. Do not discuss the second wave or have them begin implementation on it until they have the first wave fully working. Progress in this fashion for each wave.

#### THE TESTS ARE HELPFUL!

- Encourage your interviewee to closely look at the tests before they begin implementation.


### Clarifying Questions

#### Q: How should I handle invalid input? 
A: You can assume the input will be valid.

#### Q: Can I modify the Couch class?
A: No.

#### Q: Should the length/width be ints or floats?
A: Either should work for the given test cases.

#### Q: Is it OK to lie on my couch all day?
A: Yes, if that's what's best for your well-being at the time. Live your truth 💜

### Hints

- Make sure your candidate's classes aren't accidentally indented and inside the Couch class! The auto-indenting Replit does makes it easy to make this mistake. If you see your candidate do this, you can immediately let them know.

- If your candidate is struggling to form an algorithm, encourage them to explain how they would do it by hand. Afterwards help them to see what data structures might be useful.
