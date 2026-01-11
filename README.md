# Rock-Paper-Scissors-Game
Rock Paper Scissors is a hand game for two or more players. Participants say “rock, paper, scissors” and then simultaneously form their hands into the shape of a rock (a fist), a piece of paper (palm facing downward), or a pair of scissors (two fingers extended). Rules: Rock smashes scissors, Paper covers rock, Scissors cut paper.

import random
rock=["ROCK","PAPER","SCISSOR"]
while (True):
    hi=random.choice(rock)
    for i in range(len(rock)):
        print(i,"-->",rock[i])
    d=int(input("Enter you choice:"))
    print("YOU -->",rock[d])
    print("COMPUTER -->",hi)
    if (hi==rock[d]):
        print("Tie")
    elif (hi==rock[0]):
        if d==rock[1]:
            print("You Won")
        else: 
            print("Computer Won")
    elif hi==rock[1]:
        if d==rock[0]:
            print("Computer Won")
        else:
            print("You Won")
    elif hi==rock[2]:
        if d==rock[1]:
            print("You Won")
        else:
            print("Computer Won")
    exit=int(input("Press 0 to exit any other key to continue :"))
    if exit==0:
        break
