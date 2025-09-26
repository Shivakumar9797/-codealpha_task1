/* Hangman*/
import random

words = ["python", "java", "computer", "keyboard", "programming"]
word = random.choice(words)
guessed = ["_"] * len(word)
tries = 6

print("Welcome to Hangman Game!")

while tries > 0 and "_" in guessed:
    print("\nWord:", " ".join(guessed))
    print("Chances left:", tries)
    guess = input("Enter a letter: ").lower()

    if guess in word:
        for i in range(len(word)):
            if word[i] == guess:
                guessed[i] = guess
        print("Correct guess!")
    else:
        tries -= 1
        print("Wrong guess!")

if "_" not in guessed:
    print("\nYou Won! 🎉 The word was:", word)
else:
    print("\nGame Over 💀 The word was:", word)
