
* number guesing game
* 
** dokumenta saturs
  
** saturs

**** 1.aprakstīt spēli

  jautra spele, kas attīsta domāšanas
**** 2.spēles loģika

**** spēles loģika ir aprakstīta šajā kodā:

import random

number = random.randint(1, 100)
guess = 0
tries = 0

while guess != number:
    if guess < number:
        print("pamēģini lielāku skaitli")
    else:
        print("pamēģini mazāku skaitli")
        
    guess = int(input("Uzmini skaitli: "))
    tries += 1
else:
    print(f"tu uzminēji pēc {tries} reizēm")
    print("tu uzmininēji")
