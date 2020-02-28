## The four digit game

Games are a nice way of practicing our programming skills, because they try to make a simple, constrained problem. In constrast, in data science we usually have to simplify the real world to make it amenable to analysis. We are going to try and make the game "4 digits".

Step 1: The computer randomly selects a 4 digit number, where none of the digits are repeated. e.g. `1452` is a valid number, but `5523` is not (because `5` is repeated)
Step 2: We make a guess at the number. For each guess, we get told two things
  - The number of digits we have right (i.e. the right digit in the right place) R
  - The number of digits we have right but in the wrong place W
Step 3: We win when we guess the correct number

For example, if the secret number is `4257`, an example game might look like
```
Please guess a number:  1234
    Numbers in right place: 1
    Numbers in wrong place: 1
# Comment not in game (2 is in the right place, 4 is right but in the wrong place)
Please guess a number: 4259
    Numbers in right place: 3
    Numbers in wrong place: 0
# Comment not in game (4,2,5 are in the right place, there is no 7 in this game)
Please guess a number: 4289
    Numbers in right place: 2
    Numbers in wrong place: 0
Please guess a number: 4256
    Numbers in right place: 3
    Numbers in wrong place: 0
Please guess a number: 4257
    Numbers in right place: 4
    Numbers in wrong place: 0
You guessed the code!
```

### Skills taught

- importing a module (random numbers)
- practice writing functions
- string <--> integer conversion
- loops (particularly the concept of `while` loops and `flag` variables)
- getting user input
- (if time) input validation
