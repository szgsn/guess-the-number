# guess-the-number

#Number Guessing Game Objectives:

from random import randint
EASY_LEVEL_TURNS = 10
HARD_LEVEL_TURNS = 5

def check_answer(guess, answer, turns):
  if guess > answer:
    print("Too High.")
    return turns -1
  elif guess < answer:
    print("Too Low.")
    return turns -1
  else:
    print(f"It is the correct number {answer} ")

  def difficulty(): 
    user_choose_difficulty = input("Type 'easy' or 'hard': )
    if user_choose_difficulty == 'easy'
      return EASY_LEVEL_TURNS
    else:
      return HARD_LEVEL_TURNS

   def game():
      print("Welcome to the game!")
      print("I am thinking of a number between 1 and 100.")
      answer = radint(1,100)
      turns = difficulty()
      guess = 0
      while guess != answer:
        print(f"You have {turns} attempts remaining to guess the number.")
        turns = check_answer(guess, answer, turns)
        if turns == 0:
          print("You have run out of guesses, you lose.")
          return
        elif guess != answer:
          print("Guess again.")
game()
