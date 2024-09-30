

---

# Blackjack Game

## Overview
This project is a simple implementation of the classic card game **Blackjack**. The objective is to beat the dealer by having a hand value closer to 21 without exceeding it. Players receive two cards initially and can choose to "hit" for more cards or "stand" to keep their current hand. The game includes logic for handling Aces, which can count as either 1 or 11, depending on what benefits the player the most.

---

## Game Logic

### Card Representation
The game uses a list to represent card values:

```python
cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
```

- Aces are represented as 11.
- Face cards (Jack, Queen, King) count as 10.

### Functions

- **`add_user()`**: Adds a random card to the user's hand, ensuring no duplicate cards are drawn.
- **`add_comp()`**: Similar to `add_user()`, but for the dealer's hand.
- **`show_u()`**: Displays the user's cards and calculates the total value of the hand.
- **`sum_u()`**: Returns the total score of the user's hand, adjusting for Aces.
- **`sum_comp()`**: Calculates and returns the total score of the dealer's hand.
- **`show_user()`** and **`show_comp()`**: Display the cards for the user and the first card for the dealer, respectively.

> **Note**: The `art` file only contains ASCII designs for the game. You can use any design as per your preference.

---

## Game Flow
1. The game starts by dealing two cards to both the user and the dealer.
2. The user can choose to "hit" (draw another card) or "stand".
3. Scores are calculated after each action, and the game checks for winning conditions.
4. The dealer plays according to specific rules (typically hitting until reaching a score of 17 or higher).
5. The game ends when either the player stands or exceeds 21.

---

## Winning Conditions
- If the user’s score is equal to the dealer’s, it's a **draw**.
- If the user has a higher score without busting, they **win**.
- If both exceed 21, the user **loses**.
- If the dealer has a blackjack (an Ace and a 10-value card), the user **loses**.

---

## Getting Started

### Prerequisites
- **Python 3.x**
- **art** library for visual enhancements.

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/RamanRed/hacktoberfest-2.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd blackjack-game
   ```

3. **Install the required libraries** (if needed):

   ```bash
   pip install art
   ```

4. **Run the game**:

   ```bash
   python blackjack_game.py
   ```

---

