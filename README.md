# **Pick Game 🎲**

This is a two-player dice game implemented in JavaScript. I have used HTML, CSS and JavaScript for building dynamic and interactive web applications. 

## 📋 Project description

The Pick Game is a turn-based dice game for two players. Each player rolls a dice to accumulate points in their Current Score. Players can "hold" their score to transfer it to their Total Score and pass the turn to the other player. The first player to reach 100 points wins.

### Main functionality:

#### **1. DOM Manipulation and Element Selection**
The game relies on selecting and updating HTML elements dynamically:

• Players' Total Scores: score--0, score--1

• Players' Current Scores: current--0, current--1

• Active Player Indicators: .player--0, .player--1

• Dice Element: .dice (image that shows the dice roll)

• Buttons: .btn--roll, .btn--hold, .btn--new

#### 2. Game Initialization (init function)

The init function is used to reset the game and set the starting conditions:

• Both players' scores (Total and Current) are reset to 0.

• The active player is set to Player 1 (Player 0 in the code).

• The dice is hidden initially (dice.classList.add('hidden')).

• Winner and active styles are cleared.

#### 3. Rolling the Dice (btnRoll event listener)

The Roll Dice button generates a random number (1–6), displays the dice image, and updates the current score. If a 1 is rolled:

• The Current Score resets to 0.

• The turn switches to the next player using the switchPlayer function.

#### 4. Holding the Score (btnHold event listener)

The Hold button allows the active player to save their Current Score to their Total Score. After holding:

• The game checks if the player has reached the winning score of 100.

• If so, the game ends, and the winner styling is applied.

• Otherwise, the turn switches to the next player.

#### 5. Switching Players (switchPlayer function)

The switchPlayer function handles the logic for alternating between Player 1 and Player 2:

• Resets the Current Score of the active player.

• Toggles the player--active class to visually indicate the active player.

#### 6. Resetting the Game (btnNew event listener)

The New Game button calls the init function to restart the game. All scores, styles, and states are reset.


### 🛠️ Technologies used
• HTML – the structure of a web page

• CSS – providing simple design and visual effects

• JavaScript – game logic and interactivity

# How to test the Project





