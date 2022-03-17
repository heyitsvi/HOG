#The Game of HOG 
 Made as part of Berkeley 61A SICP
##Rules
 In Hog, two players alternate turns trying to be the first to end a turn with at least 100 total points. On each turn, the current player chooses some number of dice to roll, up to 10. That player's score for the turn is the sum of the dice outcomes. However, a player who rolls too many dice risks:

*Sow Sad. 
 If any of the dice outcomes is a 1, the current player's score for the turn is 1.

 Example 1: The current player rolls 7 dice, 5 of which are 1's. They score 1 point for the turn.
 Example 2: The current player rolls 4 dice, all of which are 3's. Since Sow Sad did not occur, they score 12 points for the turn.

*Picky Piggy.
 A player who chooses to roll zero dice scores the nth digit of the decimal expansion of 1/7 (0.14285714...), where n is the opponent's score. As a special case, if n is 0, the player scores 7 points.

 Example 1: The current player rolls zero dice and the opponent has a score of 3. The 3rd digit of the decimal expansion of 1/7 is 2: 0.14[2]85714285714285, The current player will receive 2 points.
 Example 2: The current player rolls zero dice and the opponent has a score of 14. The 14th digit of the decimal expansion of 1/7 is 4: 0.1428571428571[4]285, so the current player will receive 4 points.
 Example 3: The current player rolls zero dice and the opponent has a score of 0. The current player will receive 7 points.

*Hog Pile. 
 After points for the turn are added to the current player's score, if the players' scores are the same, the current player's score doubles.
 Example:
  Both players start out at 0. (0, 0)
  Player 0 rolls 2 dice and gets 5 points. (5, 0)
  Player 1 rolls 1 dice and gets 5 points. Player 1's score doubles. (5, 10)
  Player 0 rolls 2 dice and gets 6 points. (11, 10)
  Player 1 rolls 8 dice and gets 1 points. Player 1's score doubles. (11, 22)

###To run the project
 python3 hog_gui.py

####[Check the online version of this game](https://hog.cs61a.org/)