# python-game-

import random 
words = ["rambo", "shubhika", "pratham", "karan", "aryan", "mohit", "naisha", "ashutosh", "vaishnavi", "samiksha"]

correct_word = random.choice(words) 
user_input = input("guess the correct word- ")

lifeline = 4

while correct_word != user_input and lifeline>0:
  print("Wrong guess, try again.")
  if len(user_input) > len(correct_word):
    print("try a smaller word")
  else:
    print("try a larger number")
  lifeline = lifeline - 1
  user_input = input("Try again with different answer- ")


if correct_word == user_input:
  print("You Won, correct answer")
else:
  print("You lost. Game over")

print(lifeline)
print(correct_word)
 
