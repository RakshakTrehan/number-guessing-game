# 🎯 Number Guessing Game

A simple command-line number guessing game written in Python. The computer picks a secret number between 1 and 100, and you try to guess it in as few attempts as possible. After every guess you get a hint telling you to go higher or lower.

## Features

- Random secret number from 1 to 100 on every run
- "Higher" / "Lower" hints after each guess
- Counts your attempts and shows the total when you win
- Beginner-friendly code, with no external libraries needed

## Requirements

- Python 3.6 or newer (uses f-strings)

Check your version with:

```bash
python --version
```

## How to Run

1. Clone this repository (or download the file):

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Run the game:

   ```bash
   python 18_The_Perfect_Guess.py
   ```

## How to Play

1. The game picks a secret number between 1 and 100.
2. Type your guess and press Enter.
3. If the number is wrong, you'll be told to guess **higher** or **lower**.
4. Keep guessing until you find the number.
5. The game tells you how many attempts it took.

## Example Gameplay

```
Guess the number: 50
Higher number please
Guess the number: 75
Lower number please
Guess the number: 62
Lower number please
Guess the number: 59
You have guessed the number, 59 correctly in 4 attempts
```

## How It Works

- `random.randint(1, 100)` generates the secret number.
- A `while` loop keeps asking for guesses until the guess matches the secret number.
- `if` / `elif` compares each guess to the secret number and prints the hint.
- A counter variable tracks how many guesses were made.

## Tips

Try the **halving strategy**: always guess the middle of the remaining range (50, then 25 or 75, and so on). It can find any number from 1 to 100 in at most 7 guesses.

## Ideas for Future Improvements

- [ ] Handle invalid input (letters, empty input) without crashing
- [ ] Add a limit on the number of attempts
- [ ] Add a "Play again?" option
- [ ] Add difficulty levels (e.g. 1-10, 1-100, 1-1000)
- [ ] Keep track of the best score

## What I Learned

This project helped me practice:

- Using the `random` module
- `while` loops and conditional statements
- Taking user input and converting types with `int()`
- Formatting output with f-strings

## Author

Made by **<your-name>** as part of my Python learning journey.
