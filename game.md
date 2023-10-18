## Izvedot number guessing spēli ar Python programmēšanas valodu

### Dokumenta saturs

#### 1. Spēles apraksts
Interesenta spēlē kas atīsta loģiku.

#### 2. Spēles loģika

Dators nejauši ģenerē vienu skaitli no 1 līdz 100. Tālāk, piedāvā spēlētājam uzminēt to skaitli. Un t.t.

Spēles loģika ir labi aprakstīta sājā kodā:
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
