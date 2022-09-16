# Stone-Paper-Scissor


import random


# Rock
Rock=("""
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
""")

# Paper
Paper=("""


     _______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)
""")

# Scissors
Scissors=("""
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
""")

game_images= [Rock,Paper,Scissors]

choice=int(input("What do you choose? Type 0 for rock, 1 for Paper or 2 for Scissors. "))

if choice >=3:
  print("oops you typed an invalid number, you loose")
else: 
 print(f"your choice is :{choice} {game_images[choice]}" )

 computer_choice=random.randint(0,2)
 print(f"The computer choice is: {computer_choice}{game_images[computer_choice]} " )



 if computer_choice==choice:
  print("Match is draw")
 elif computer_choice ==1 and choice==2:
  print("you win")
 elif computer_choice==1 and choice==0:
  print("computer wins")
 elif computer_choice==2 and choice==1:
  print("computer won")
 elif computer_choice==2 and choice==0:
  print("you won")
 elif computer_choice==0 and choice==1:
  print("you won")
 elif computer_choice==0 and choice==2:
  print("computer won")
  
  
  
  
  sample output:
  What do you choose? Type 0 for rock, 1 for Paper or 2 for Scissors. 0
your choice is :0 
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)

The computer choice is: 2
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
 
you won
 



  
  
