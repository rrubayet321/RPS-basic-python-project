# RPS-basic-python-project


import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇

play= [rock, paper, scissors]
user_play= int(input("What do your choose? 0 for Rock, 1 for paper and 2 for Scissors\n"))
print(play[user_play])

computer_choice= random.randint(0,2)
print('Computer chose')
print(play[computer_choice])

if user_play>= 3 or user_play < 0:
  print('Your choice is invalid sir!')
elif user_play==0 and computer_choice==2:
  print('You won!')
elif computer_choice==2 and user_play==0:
  print('You lose!')
elif computer_choice > user_play:
  print('You lose!')
elif user_play > computer_choice:
  print('You won!')
elif user_play == computer_choice:
  print("It's a draw!")
  
