# Hangman Game Using Python

## Overview
This project is a Python implementation of the classic **Hangman Game**. The player must guess a randomly chosen word by guessing one letter at a time. Incorrect guesses reduce the player's lives, and the game ends when either the word is guessed or the player runs out of lives.

---

## Features
- **Random Word Selection**: A word is randomly chosen from a predefined list.
- **Dynamic Display**: Updates the guessed letters and shows progress visually.
- **Life System**: Players have 6 lives, with each incorrect guess reducing one life.
- **ASCII Art**: Displays the hangman stages based on remaining lives.
- **Feedback**: Notifies the player if their guess is correct or incorrect.

---

## How to Play
1. Run the script.
2. A random word is chosen, and the player sees blanks (`_`) for each letter in the word.
3. The player guesses one letter at a time.
4. The game provides feedback:
   - Correct guesses reveal the letter(s) in the word.
   - Incorrect guesses reduce the player's lives and update the hangman graphic.
5. The game ends when:
   - The player successfully guesses the entire word, or
   - The player runs out of lives.

---

## Example Gameplay

### Initial Display
```plaintext
 _                                             
| |                                            
| |__   __ _ _ __   __ _ _ __ ___   __ _ _ __  
| '_ \ / _` | '_ \ / _` | '_ ` _ \ / _` | '_ \ 
| | | | (_| | | | | (_| | | | | | | (_| | | | |
|_| |_|\__,_|_| |_|\__, |_| |_| |_|\__,_|_| |_|
                    __/ |                      
                   |___/    

_ _ _ _ _ _
  +---+
  |   |
      |
      |
      |
      |
=========
```

### Gameplay Example
#### Input and Feedback
```plaintext
Guess a letter: a
You guessed a letter that is there in the word!
_ a _ a _ a
  +---+
  |   |
      |
      |
      |
      |
=========
```

#### Another Input
```plaintext
Guess a letter: x
You guessed a letter that is not there in the word. You lose a life!
_ a _ a _ a
  +---+
  |   |
  O   |
      |
      |
      |
=========
```

### Endgame Example
#### Win
```plaintext
Guess a letter: b
You guessed a letter that is there in the word!
b a _ a _ a
Guess a letter: n
You guessed a letter that is there in the word!
b a n a n a
  +---+
  |   |
      |
      |
      |
      |
=========
You guessed the word. You win!
```

#### Lose
```plaintext
Guess a letter: z
You guessed a letter that is not there in the word. You lose a life!
_ _ _ _ _ _
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========
You ran out of lives. You lose!
The word is banana
```
