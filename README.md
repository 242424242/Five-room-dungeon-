# Five-room-dungeon-
Five-room-dungeon 
#  date written: 10/22/2024
import random
import random
from itertools import repeat
# this is all i have so far, plz enjoy
import random

while True:
    print("FRD, please input your name")
    name = input("What is your character's name?: ")

    sided = random.randint(1, 10)
    strength = random.randint(1, 10)
    perception = random.randint(1, 10)
    endurance = random.randint(1, 10)
    charisma = random.randint(1, 10)
    intelligence = random.randint(1, 10)
    agility = random.randint(1, 10)
    luck = random.randint(1, 10)

    print(name, "your health is", sided)
    print(name, "your strength is", strength)
    print(name, "your perception is", perception)
    print(name, "your endurance is", endurance)
    print(name, "your charisma is", charisma)
    print(name, "your intelligence is", intelligence)
    print(name, "your agility is", agility)
    print(name, "your luck is", luck)

    enemy = input("What is your enemy's name?: ")

    s = random.randint(1, 10)
    f = random.randint(1, 10)
    p = random.randint(1, 10)
    e = random.randint(1, 10)
    c = random.randint(1, 10)
    i = random.randint(1, 10)
    a = random.randint(1, 10)
    l = random.randint(1, 10)
    print(enemy, "health is", s)
    print(enemy, "strength is", f)
    print(enemy, "perception is", p)
    print(enemy, "endurance is", e)
    print(enemy, "charisma is", c)
    print(enemy, "intelligence is", i)
    print(enemy, "agility is", a)
    print(enemy, "luck is", l)

    confirm = input("Do you wish to play? Type 'yes' if Yes: ")

    if confirm.lower() == "yes":
        print("Thank you for giving me your name. Your goal is to solve puzzles and beat", enemy, "at the end. Good luck, Warrior!")
        break  # Exit the loop if the user confirms
    else:
        print("You have selected no. Please pick your name again and you will be given random stats.")





act1 = input ("""you wake up in a small cave and look around, you see an exit straight ahead but it is surrounded with spinning 
blades,you look side to side and see a lever on the left wall.maybe it does something, do you flip the lever? """)




if act1 == "yes":
    print("the blades blocking the exit retract into the walls, you can now move to the next room")
    act2 = input("""You move on to the next room there are 2 paths to the right you see a sword 
and to the left you see the exit but it seems risky to get the sword do you do it and risk your life? """)
    if act2 == "yes":


        random_choice = random.randint(0, 1)


        if random_choice == 0:
            print("you fall down and drown")
        else:
            print("You Get the sword and barely make it out you stepped on a broken piece of bridge and that platform the sword was on falls into the rocky river below")

elif act1 == "no":
    print("nothing happens and your still trapped.")
