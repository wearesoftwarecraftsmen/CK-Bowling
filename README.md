# Code Kata: Bowling

Kata used from [Uncle Bob](http://butunclebob.com/ArticleS.UncleBob.TheBowlingGameKata)

## Before you Begin
- Do **not** read ahead
- Work only **one** task at a time; part of the kata is to learn to work *incrementally*
- We are only testing for correct inputs

### Libraries
* [MSpec](https://github.com/machine/machine.specifications)
* [Develop with Passion: Specifications](https://github.com/developwithpassion/developwithpassion.specifications)
* RhinoMocks
* [Fluent Assertions](http://fluentassertions.codeplex.com/)

## Problem Domain
The game consists of 10 frames as shown above.  In each frame the player has
two opportunities to knock down 10 pins.  The score for the frame is the total
number of pins knocked down, plus bonuses for strikes and spares.

A spare is when the player knocks down all 10 pins in two tries.  The bonus for
that frame is the number of pins knocked down by the next roll.  So in frame 3
above, the score is 10 (the total number knocked down) plus a bonus of 5 (the
number of pins knocked down on the next roll.)

A strike is when the player knocks down all 10 pins on his first try.  The bonus
for that frame is the value of the next two balls rolled.

In the tenth frame a player who rolls a spare or strike is allowed to roll the extra
balls to complete the frame.  However no more than three balls can be rolled in
tenth frame.