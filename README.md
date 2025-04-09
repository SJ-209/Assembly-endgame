Assembly Endgame
Overview
Assembly Endgame is a word-guessing game inspired by the classic game Hangman. Developed as part of Scrimba's course project, the goal is to guess the hidden word within a limited number of attempts while avoiding incorrect guesses. Each incorrect guess "eliminates" a programming language, and the game is over when all languages are lost.

Features
Interactive word-guessing gameplay.
Keyboard-based letter selection for a seamless user experience.
Tracks correct and incorrect guesses dynamically.
"Game Over" mechanic when too many incorrect guesses occur.
Option to reset the game and start fresh.
Random farewell messages for eliminated programming languages.
How to Play
A random programming-related word is selected (e.g., react).
You start with all programming languages "active."
Guess the word one letter at a time by clicking the displayed keyboard buttons.
Correct Guesses: Revealed in the hidden word.
Incorrect Guesses: A programming language is eliminated.
Lose the game if you make too many incorrect guesses.
Win the game by correctly guessing all letters in the word.
Technologies Used
React: For building the interactive UI.
JavaScript: For game logic and dynamic rendering.
CSS: For styling and animations.
Project Features
Dynamic Letter Guessing:

Displays letters when guessed correctly.
Tracks incorrect guesses visually on the keyboard.
Keyboard Interaction:

Buttons dynamically update to reflect "correct" or "wrong" states.
Disabled buttons prevent duplicate guesses.
Language Elimination:

Incorrect guesses "remove" a language visually from the list.
Random farewell messages (e.g., "RIP, JavaScript!") are displayed for eliminated languages.
Game Over Mechanic:

Ends the game after exceeding the incorrect guess limit.
Displays a "New Game" button to restart.
Responsive Design:

Optimized for various screen sizes for a great user experience.
Installation
Clone the repository:

git clone https://github.com/yourusername/assembly-endgame.git
cd assembly-endgame
Install dependencies:

npm install
Start the development server:

npm start
Open your browser at http://localhost:3000 to play the game.

Project Structure
src/
│
├── components/         # React components
│   ├── App.jsx         # Main component
│   ├── Keyboard.jsx    # Letter keyboard component
│   ├── GameStatus.jsx  # Displays game status (win/lose)
│   └── Languages.jsx   # Programming languages visualization
│
├── utils/              # Utility functions
│   └── getFarewellText.js # Generates farewell messages
│
├── assets/             # Static files (e.g., icons, images)
│
├── App.css             # Main stylesheet
├── index.js            # Application entry point
└── index.html          # Static HTML template
How It Works
Game Initialization:

The game selects a random word.
The user starts with 8 "lives" (number of languages).
Game Loop:

Players click a letter to guess.
Correct guesses reveal the letter in the word.
Incorrect guesses eliminate a language with a farewell message.
End States:

Win: All letters guessed correctly.
Lose: More than 8 incorrect guesses.

This project was developed as part of Scrimba's Frontend Developer Path. A big thanks to the instructors and Scrimba community for their support.