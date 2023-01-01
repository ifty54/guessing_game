# guessing_game
import random

def guessing_game():
    #guessing a number
    secret_number = random.randint(1,10)

    #prompt users to guess it
    guess = int(input("enter your guess: "))

    #keep track of the guess
    number_guess = 1

    #keeping asking user to guess until they make it
    while guess != secret_number:
        if guess > secret_number:
            print("too high")
        else:
            print("too low")
        guess = int(input("enter again your guess: "))
        number_guess += 1

    #finally guessed it right
    print(f"You've guessed it right after {number_guess} tries. The correct number is {guess}")


guessing_game()
