# RockPaperScissors
# A traditional game of rock paper scissors from our childhood made using PYTHON

import random
user=input("enter a choice(rock,paper,scissors):\n")

while True:

 possible_actions = ["rock", "paper","scissors"]
 computer_action =random.choice(possible_actions)
 print(f"\n You chose {user}, computer chose {computer_action}.\n")

 if user==computer_action:
    print(f"Both player got same output. Its a tie!")

 elif user=="rock":
    if computer_action== "scissors":
        print("Rock smashes scissors! You Win!")
    else:
        print("Paper covers rock! You lose!")
 elif user== "paper":
    if computer_action=="rock":
        print("Paper covers rock! You win!")
    else:
        print("Scissors cuts Paper! Yyou lose!")
 elif user=="scissors":
    if computer_action=="rock":  
        print("Rock smashes scissors! You lose!")
    else:
        print("scissors cuts paper! You win!")

 play_again=input("Play again? (y/n):\n")
 if play_again.lower()!= "y":
        break          

