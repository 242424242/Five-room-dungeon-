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
    classes = input("""what class do you want to play as
    Archer.
    Barbarian.
    Custom.""")
    if classes == "Archer" or "archer":
        name = input("What is your character's name?: ")

        sided = random.randint(1, 6)
        strength = random.randint(1, 7)
        perception = random.randint(1, 10)
        endurance = random.randint(1, 10)
        charisma = random.randint(1, 12)
        intelligence = random.randint(1, 13)
        agility = random.randint(1, 15)
        luck = random.randint(1, 10)

        print(name, "your health is", sided)
        print(name, "your strength is", strength)
        print(name, "your perception is", perception)
        print(name, "your endurance is", endurance)
        print(name, "your charisma is", charisma)
        print(name, "your intelligence is", intelligence)
        print(name, "your agility is", agility)
        print(name, "your luck is", luck)
    elif classes == "Barbarian" or "barbarian":
        name = input("What is your character's name?: ")

        sided = random.randint(1, 15)
        strength = random.randint(1, 13)
        perception = random.randint(1, 10)
        endurance = random.randint(1, 14)
        charisma = random.randint(1, 9)
        intelligence = random.randint(1, 8)
        agility = random.randint(1, 8)
        luck = random.randint(1, 10)

        print(name, "your health is", sided)
        print(name, "your strength is", strength)
        print(name, "your perception is", perception)
        print(name, "your endurance is", endurance)
        print(name, "your charisma is", charisma)
        print(name, "your intelligence is", intelligence)
        print(name, "your agility is", agility)
        print(name, "your luck is", luck)
    elif classes == "Custom" or "custom":
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

    confirm = input("Do you wish to play? Type 'yes' if Yes, Type no if you want to change your character: ")

    if confirm.lower() == "yes":
        print("Thank you for giving me your name. Your goal is to solve puzzles and beat", enemy, "at the end. Good luck, Warrior!")
        break
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
            act3 = input("""you walk into the next room, inspecting it you find two levers and a dispenser,
             in the middle of the room you see a trapdoor that seems to be locked and maybe one of the levers can unlock it when switched.
              so which one do you press. left or right. """)
            if act3 == "left":
                print("""three arrows shoot out from the dispenser and peirce through your flesh, 
                you fall to the ground and lie there in agony as the world around you fades into darkness""")
            elif act3 == "right":
                print("""the trapdoor opens and you hear an ear piercing roar coming from below,
                 you look behind you and see the walls start to close in, leaving you with one choice, jump down the hole""")
                fight = input("""you jump through the trapdoor and after a brief second you land into a small body of water, 
                once you climb onto land you look around the room and see a goblin on the right side of the room who seems to be guarding somthing 
                and on the left of the room you see a large gap inbetween you and a goblin holding a bow and a quiver of arrows""")
    elif act2 == "no":
        print("you walk past it and enter the next room but end up being surprised a goblin and get slain. wish you could've gotten that sword to block the attack huh?")
elif act1 == "no":
    print("nothing happens and your still trapped.")
