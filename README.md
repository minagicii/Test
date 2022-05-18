# Code

guess_count = 1

while guess_count < 3:
 import random
 randomNumber = random.randint(1, 100)
 print("Welcome to the number guessing game")
 print("See how many guesses you take until you guess the number between 1 and 100.")
 userNumber = int(input("Enter your guess:"))


 if userNumber > randomNumber:
    print("Too high, Try again!")
    guess_count = guess_count + 1
 elif userNumber < randomNumber:
    print("Too low, Try again")
    guess_count = guess_count + 1
 else:
     print("Well done")

if guess_count > 3:
    print("It took you three attempts to guess the number")
    print("GAME OVER")
else:
    print("Error")
