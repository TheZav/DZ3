# DZ3
import random
rnum = random.randint(1,1000)
tr = 1
while True:
  g = int(input("Guess the number - 1-1000!   "))
  if g != rnum:
    tr += 1
    if tr < 11:
      print("That's wrong, let's try again! You have",11-tr,"tries still...")
    elif tr == 11:
      print("And that's the game! You've lost!")
      break
  elif g == rnum:
    print("And we have a winner! You've guessed the number on your",tr,"try!")
    break
