# MohamedAliGuessTheNumberGame


import random

def guess(x):
    random_number = random.randint(1, x)
    guess = 0
    while guess != random_number:
        gues = int(input(f'guess a number between 1 and {x}:'))
        if guess < random_number:
            print('sorry, guess again. Too low.')
        elif guess > random_number:
            print('sorry guess again. Too high.')

    print(f'yay, congrats. you have guessed the number {random_number} correctly!!!')

guess(100)
