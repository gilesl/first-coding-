first-coding-
=============

#A simple guess my number game

#Import a random number generator 

import random

exit ="y"

while exit=="y":

    number = random.randint(1,10)
    guess = -1
    count = 0

    print ("I'm thinking of a number between 0 and 10 can you guess it?..")

    while guess != number:
        guess = int(input("Whats your guess ..."))
        count=count+1

        if guess == number:
            print("Thats correct in ......... ",count,)  
        elif guess < number:
            print("To small")
        elif guess > number:
            print("To large")
            
    exit=input("Type 'y' to play again any other key to exit...")

print("Thanks for playing")
