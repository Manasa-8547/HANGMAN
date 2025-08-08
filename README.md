
# 🎮 Hangman Game - Python

A classic word-guessing game implemented in Python where players try to guess a fruit name letter by letter!

# 👨‍💻 Developer Information 
- **Developer**: P.Manasa
- **Roll No**: 222T1A3145
- **Institution**: Ashoka Womens Engineering College.

## 🎯 Game Description

Hangman is a traditional word-guessing game where the player attempts to guess a secret word by suggesting letters within a limited number of attempts. In this version, all the secret words are names of fruits.

## 🚀 Features

- Random fruit word selection from a curated list
- Letter-by-letter guessing mechanism
- Input validation (single letters only)
- Duplicate guess prevention
- Dynamic chances calculation based on word length
- Win/lose conditions with appropriate messages
- Keyboard interrupt handling (Ctrl+C)

## 📋 Requirements

- Python 3.x
- No external dependencies required (uses built-in modules)

## 🎮 How to Play

1. Run the Python script
2. The game will display empty spaces representing letters in the secret fruit name
3. Enter one letter at a time when prompted
4. Correct guesses will reveal the letter's position(s) in the word
5. You have `word_length + 2` chances to guess the entire word
6. Win by guessing all letters before running out of chances!

## 📝 Game Rules

- Only single alphabetic characters are accepted
- Case-insensitive input (both 'A' and 'a' work)
- Duplicate guesses are not allowed
- Wrong guesses reduce your remaining chances
- Game ends when you either guess the word or run out of chances

## 🍎 Available Words

The game includes the following fruit names:
- apple, banana, mango, strawberry, orange, grape
- pineapple, apricot, lemon, coconut, watermelon
- cherry, papaya, berry, peach, lychee, muskmelon

## 📁 File Structure

```
hangman-game/
│
├── hangman.py          # Main game file
└── README.md          # This file
```

## 🔧 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/hangman-game.git
   cd hangman-game
   ```

2. **Run the game:**
   ```bash
   python hangman.py
   ```

3. **Follow the on-screen instructions to play!**

## 💻 Code Example

```python
# Example gameplay
Guess the word! HINT: word is a name of a fruit
_ _ _ _ _ 

Enter a letter to guess: a
a _ _ _ _ 

Enter a letter to guess: p
a p p _ _ 

Enter a letter to guess: l
a p p l _ 

Enter a letter to guess: e
The word is:  apple
Congratulations, You won!
```

## 🛠️ Technical Details

### Key Components:
- **Random Word Selection**: Uses `random.choice()` to pick a fruit name
- **Input Validation**: Comprehensive checking for valid letter inputs
- **Game State Tracking**: Monitors guessed letters and remaining chances
- **Win Condition**: Uses `Counter` from collections to compare letter counts

### Error Handling:
- Invalid input types (numbers, symbols)
- Multiple character inputs
- Duplicate letter guesses
- Keyboard interrupts (graceful exit)

## 🎨 Sample Output

```
Guess the word! HINT: word is a name of a fruit
_ _ _ _ _ _ 

Enter a letter to guess: a
a _ _ a _ a 

Enter a letter to guess: n
a n a n a 

Enter a letter to guess: b
The word is:  banana
Congratulations, You won!
```

## 🤝 Contributing

Contributions are welcome! Here are some ways you can improve the game:

1. **Fork the repository**
2. **Create a feature branch:** `git checkout -b feature-name`
3. **Make your changes and commit:** `git commit -m 'Add some feature'`
4. **Push to the branch:** `git push origin feature-name`
5. **Submit a pull request**

### Possible Enhancements:
- Add different word categories (animals, countries, etc.)
- Implement difficulty levels
- Add a graphical hangman drawing
- Create a scoring system
- Add multiplayer functionality
- Implement word hints

## 🙏 Acknowledgments

- Inspired by the classic Hangman game
- Thanks to the Python community for excellent documentation
- Built as a learning project for Python programming

---

**Enjoy playing Hangman! 🎉**

*Made with ❤️ and Python*
