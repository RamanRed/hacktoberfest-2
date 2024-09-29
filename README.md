Blackjack Game
Overview
This project is a simple implementation of the classic card game Blackjack. The objective is to beat the dealer by having a hand value closer to 21 without exceeding it. Players receive two cards initially and can choose to "hit" for more cards or "stand" to keep their current hand. The game includes logic for handling Aces, which can count as either 1 or 11, depending on what benefits the player the most.

Game Logic
Card Representation
The game uses a list to represent card values:
python
Copy code
cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
Here, Aces are represented as 11, and face cards (Jack, Queen, King) count as 10.
Functions
add_user(): Adds a random card to the user's hand, ensuring no duplicate cards are drawn.

add_comp(): Similar to add_user(), but for the computer's hand.

show_u(): Displays the user's cards and calculates the total value of the hand.

sum_u(): Returns the total score of the user's hand, adjusting for Aces.

sum_comp(): Calculates and returns the total score of the computer's hand.

show_user() and show_comp(): Display the cards for the user and the first card for the dealer, respectively.

Note : art file only contains ascii design for game you can use any as per your need.

Game Flow
The game starts by dealing two cards to both the user and the dealer.
The user can choose to hit (draw another card) or stand.
The scores are calculated after each action, and the game checks for winning conditions.
The dealer plays according to specific rules (typically hitting until reaching a score of 17 or higher).
The game ends when either the player stands or exceeds 21.
Winning Conditions
If the user’s score is equal to the computer’s, it's a draw.
If the user has a higher score without busting, they win.
If both exceed 21, the user loses.
If the dealer has a blackjack (an Ace and a 10-value card), the user loses.
Getting Started
Prerequisites
Python 3.x
The art library for visual enhancements.
Installation
Clone the repository:

bash
Copy code
      
     git clone https://github.com/RamanRed/hacktoberfest-2.git
Navigate to the project directory:

bash
Copy code
cd blackjack-game
Install the required libraries (if needed):

bash
Copy code
pip install art
Run the game:

bash
Copy code
python blackjack_game.py
