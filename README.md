# solitaire-py
ReadMe

PRESS FORK(looks like a Y button next to share button) to make a copy for access to Ed terminal
RUN game.py

This game functions similarly as the popular game called solitaire with added AI implementation
SUITS:
D for Diamond ♦, C for Club ♣, H for Heart ♥, S for Spade ♠
RANKS:
A12345678910JQK
COMMANDS WHEN PLAYING THE GAME (*1):
-	“UNDO” or “RE”
	Undo your previous move. 
	•	If you are prompted with “No previous move!”, you are trying to undo your last move while you do not have one.  (Note that undo will also be counted as a move in the step counter.

-	THE RANK OF THE CARD FOLLOWED BY THE SUIT OF THE CARD + (c/s)
	Move the desired card automatically
	•	E.g., (7H) means moving 7♥ (*1&2) 
	•	If you are prompted with “No possible move, please try again!”, your move is not available, please input an available command.
	•	You can specify where you move your card, type a “c” if you wish to move the card to the columns or type a “s” if you wish to move the card to the stacks.  (e.g., 7H c)

-	“RESTART”
	Start a new game
	•	After you entered restart, you will be prompted with “Are you sure to restart game? Your current progress will be lost! Restart? (Y/N):”. Enter “y” for yes or “’no” for no. (	*1)

-	“FLIP” or “F”
	•	  (bottom card would be closed if opened card is larger than 3)

-	“EXIT”
	Quit game

*1 Not case sensitive
*2 Priority of card movement:
 1. To Stack (if available)
    	2. To available column (if any, prioritize to column 1 and so on)

HOW TO PLAY

1.	The game starts on its own for the first time
2.	When you play the game, you are required to enter a command
3.	You can enter “restart” if you have no other possible moves.
4.	If you are prompted with “Invalid input, please try again!”, you have input a wrong command, please input a correct command.
5.	Rearrange the face up cards by inputting the name of the card, for example, “6D”, and the card will be automatically moved to the available column.
6.	Keep placing the cards on top of each other until you cannot move anymore. Each column should be alternating in colour and move in descending order.
7.	Build your foundation piles starting with the aces. You may move cards of the corresponding suit to the pile in ascending order.
8.	You can start a new column in an empty space using a king.
9.	You can input the commands shown on the previous page.
10.	Repeat steps 5-9 until there is no possible move. 
11.	Your number of moves with be counted by the move counter on the top of the card deck.
12.	When you win the game, you will be prompted with “Congratulations, you won! Start a new game? (Y/N):”, you can choose to restart another game. Enter “y” for yes or “’no” for no. (Not case sensitive)

For more information on how to play solitaire you can click the link below:
https://www.wikihow.com/PlaySolitaire#:~:text=To%20play%20solitaire%2C%20try%20to,up%20card%20at%20the%20bottom.

Scoring system
There is a score board on the top of the deck, the calculation of the score are showed below:
•	+5 for card move from deck to column
•	+5 for card in column opened
•	+10 for card move to stack
•	-15 for card from stack to column
•	-100 for deck cycled for 1 time
•	The scores are always positive
