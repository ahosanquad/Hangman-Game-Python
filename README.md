# Hangman Game

This is a Python-based implementation of the classic word-guessing game **Hangman**. The game is played via the terminal, where the player guesses letters to uncover a hidden word.

---

## Features
- The game randomly selects a word from a predefined word list.
- The hangman graphic updates with every incorrect guess.
- Tracks guessed letters and prevents duplicate guesses.
- Displays a hint with underscores for unrevealed letters.
- Provides a win or lose message depending on the outcome of the game.

---

## Prerequisites
- Python 3.7 or later.
- A `word_list.py` file containing a variable named `words` with a list of words (e.g., `words = ["python", "hangman", "developer"]`).

---

## How to Play
1. Run the `hangman.py` file in your terminal.
2. A word will be randomly selected, and the hint will display underscores (`_`) for unrevealed letters.
3. Enter a single letter as your guess:
    - If the letter is in the word, it will replace the underscores in the correct positions.
    - If the letter is incorrect, the hangman graphic updates with a new part.
4. Win by guessing all the letters in the word before the hangman graphic is fully drawn.
5. Lose if the hangman graphic is completed before you guess the word.

---

## Game Flow
1. Start the game by running the script.
2. The program will display:
    - The current hangman graphic.
    - The current hint (e.g., `_ _ _ _ _`).
    - A prompt for your guess.
3. After each guess:
    - The hangman graphic updates (for incorrect guesses).
    - The hint updates (for correct guesses).
    - A message appears if the guess was invalid or already guessed.
4. The game ends with a win or lose message, displaying the full word.

---

## Example Run
```
*************************
  
  
  
*************************
_ _ _ _ _
Enter a letter: a

*************************
 o 
 | 
  
*************************
_ _ a _ _
Enter a letter: e

*************************
 o 
/| 
  
*************************
_ _ a _ e
...
```

---

## Files
- **`hangman.py`**: The main game file.
- **`word_list.py`**: Contains the list of possible words.

---

## Customization
- **Modify the Word List**: Update `word_list.py` to include your desired words.
- **Change the Hangman Art**: Edit the `hangman_art` dictionary in `hangman.py` to use custom graphics.

---

## License
This project is open source and available under the MIT License.

---

## Acknowledgments
Thanks to the Python community for inspiration and resources!
