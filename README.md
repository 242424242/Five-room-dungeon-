# Five-room-dungeon-
Five-room-dungeon 
#  date written: 10/22/2024
# this is all i have so far, plz enjoy

#latest version
# date written: 2/11/2025
# this is the latest version of the code and I might keep working on this project so do as you please with my code.


import random

while True:
    classes = input("""what class do you want to play as,
    Archer.
    Barbarian.
    Custom.""")
    if classes == "Archer" or "archer":
        name = input("What is your character's name?: ")

        sidedd = random.randint(1, 6)
        strengthF = random.randint(1, 7)
        perception = random.randint(1, 10)
        endurance = random.randint(5, 10)
        charisma = random.randint(1, 12)
        intelligence = random.randint(1, 13)
        agility = random.randint(1, 15)
        luck = random.randint(1, 10)

        print(name, "your health is", sidedd)
        print(name, "your strength is", strengthF)
        print(name, "your perception is", perception)
        print(name, "your endurance is", endurance)
        print(name, "your charisma is", charisma)
        print(name, "your intelligence is", intelligence)
        print(name, "your agility is", agility)
        print(name, "your luck is", luck)

    elif classes == "Barbarian" or "barbarian":
        name = input("What is your character's name?: ")

        sided = random.randint(15, 15)
        strengthF = random.randint(10, 20)
        perception = random.randint(1, 10)
        endurance = random.randint(10, 20)
        charisma = random.randint(1, 9)
        intelligence = random.randint(1, 8)
        agility = random.randint(1, 8)
        luck = random.randint(1, 10)

        print(name, "your health is", sided)
        print(name, "your strength is", strengthF)
        print(name, "your perception is", perception)
        print(name, "your endurance is", endurance)
        print(name, "your charisma is", charisma)
        print(name, "your intelligence is", intelligence)
        print(name, "your agility is", agility)
        print(name, "your luck is", luck)

    elif classes == "Custom" or "custom":
        name = input("What is your character's name?: ")

        sideddd = random.randint(5, 10)
        strengthF = random.randint(1, 10)
        perception = random.randint(1, 10)
        endurance = random.randint(5, 10)
        charisma = random.randint(1, 10)
        intelligence = random.randint(1, 10)
        agility = random.randint(1, 10)
        luck = random.randint(1, 10)

        print(name, "your health is", sideddd)
        print(name, "your strength is", strengthF)
        print(name, "your perception is", perception)
        print(name, "your endurance is", endurance)
        print(name, "your charisma is", charisma)
        print(name, "your intelligence is", intelligence)
        print(name, "your agility is", agility)
        print(name, "your luck is", luck)

    goblin_damage = random.randint(1, 3)
    goblin_health = 10
    damage = strengthF * 0.2
    goblin_hit_rate = random.randint(1, 6)

    boss_damage = random.randint(1, 3)
    boss_health = 15
    damagee = strengthF * 0.2
    boss_hit_rate = random.randint(3, 6)

    if goblin_hit_rate == 3:
        endurance -= goblin_damage
    player_damage = strengthF - 3 * 1.5

    confirm = input("Do you wish to play? Type 'yes' if Yes, Type no if you want to change your character: ")

    if confirm.lower() == "yes":
        print(
            "Thank you for giving me your name. Your goal is to solve puzzles and do through all the rooms. Good luck, Warrior!")
        break
    else:
        print("You have selected no. Please pick your name again and you will be given random stats.")

act1 = input("""you wake up in a small cave and look around, you see an exit straight ahead but it is surrounded with spinning 
blades,you look side to side and see a lever on the left wall.maybe it does something, do you flip the lever? """)

if act1 == "yes":
    print("the blades blocking the exit retract into the walls, you can now move to the next room")
    act2 = input("""You move on to the next room there are 2 paths to the right you see a sword 
and to the left you see the exit but it seems risky to get the sword do you do it and risk your life? """)
    if act2 == "yes":

        random_choice = random.randint(0, 99)

        if random_choice == 0:
            print("you fall down and drown")
        else:
            print(
                "You Get the sword and barely make it out you stepped on a broken piece of bridge and that platform the sword was on falls into the rocky river below")
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
                and on the left of the room you see a large gap in between you and a goblin holding a bow and a quiver of arrows.
                maybe you can make the jump and attack the goblin with the bow or you could sneak past the other goblin before he notices you, which do you pick, fight and get the bow
                or sneak to the next room? """)
                if fight == "fight and get the bow" or "fight the guy with the bow" or "fight":
                    print("you run towards the ledge and attempt to make the jump.")
                    random_choice = random.randint(0, 100)
                    if random_choice == 0:
                        print("you miss the jump and fall down into the endless hole")
                    else:
                        print(
                            """you make the jump over the endless hole and tackle the goblin to the ground but he breaks out of your grasp and he tries to fire an arrow at you""")
                        random_choice = random.randint(0, 3)
                        if random_choice == 0 or 2:
                            print(
                                "you dodge the arrow and cut off the goblin's arm before pushing him into the hole, you then turn around and pick up the bow")
                            fightt = input(
                                "you jump over the hole and land back on the other side once you hit the ground you notice a goblin charging towards you.")
                            if goblin_hit_rate > 6:
                                endurance -= goblin_damage
                                print("you were cut by the goblin's dagger and took", goblin_damage,
                                      "damage, your health is now", endurance)
                                print(
                                    "you fall to the ground stunned and the goblin attempts to stab you through the heart.")
                                if agility < 1:
                                    print("you fail to dodge the dagger and lose all the breath in your lungs before your vision fades and you are left in nothing but darkness.")
                            else:
                                hit = input("you dodge the attack and gain the chance to strike.do you take the chance to hit? ")
                                if hit == "yes":
                                    if agility > 4:
                                        goblin_health -= player_damage
                                        print(
                                            f"you strike the goblin and lower it's health. goblin health is now {goblin_health}")
                                        if goblin_health < 20:
                                            print(
                                                "the goblin falls to the ground and cowers in fear before running away.")
                                            print("you walk past him and jump down into the hole it was guarding")
                                            print("""you notice a pond under you and with a deep breath you dive into it.
                                            once you hit the water you start swimming towards land. as you hit land you hear a roar. the feeling of terror runs through your spine.
                                            you see the final door,so close but then an orc jumps out from behind a rock and stands between you and the door""")
                                            act5 = input(
                                                " he charges at you and you manage to dodge. do you take the chance to attack")
                                            if act5 == "yes":
                                                print("you strike him in the side and make him stumble.")
                                                boss_health - damagee
                                                the_end = input(
                                                    "you strike the orc and sun it for a brief period of time. do you strike again?")
                                                if the_end == "yes":
                                                    boss_health - damagee
                                                    ending = input("""you strike the orc once more and you start to notice how his defenses begin to falter,
                                                    he stares at you with fear his health getting worse. do you deliver the final blow. """)
                                                    if ending == "yes":
                                                        print("you stab your sword into the orc's chest and with a heavy thud it falls onto the ground.")
                                                        print("""You look back to the door the orc was guarding, the silence overwhelming.
                                                         Before You, an iron door stands, rusted but standing firm. With a deep breath, 
                                                         You push it open, but beyond lies only an empty void. No treasure. No monster. Just darkness""")
                                                        print("""You stand there for a long moment, the weight of the journey pressing down. 
                                                        Then it becomes clear—the dungeon wasn't meant to be conquered by strength or cunning. The true challenge was always within.""")
                                                        print("""The rooms, the traps, the monsters, each obstacle had only mirrored your own fears, your own doubts. 
	                                                        The real prize wasn’t treasure, but the truth you had to face about yourself.""")
                                                        print("""With a deep, steadying breath, you turn and walk out of the cave, the darkness receding.
                                                        The world outside is unchanged, but you found something deeper. 
                                                        You now carry the truth within, the knowledge that the greatest victory is in confronting oneself.""")
                                                        print("The adventure, in the end, was about finding peace within.")
                                                        print("")
                                                        print("")
                                                        print("""player, look back at the adventure. you solved puzzles and beat bad guys,
                                                        you might think back to this thinking the ending is all corny,but it's true, not all of your questions will be answered by others,
                                                        but they're still out there somewhere, you'll find them in life, no telling where they are or where they take you,
                                                        but everything ends in a good way, so instead of throwing you're dreams away,
                                                        leave them in the background, pursue them slowly and trust the process. so go your own adventure.
                                                        The adventure called life.""")
                                                    else:
                                                        print("the orc spins around")
                                                else:
                                                    print("the orc quickly turns around and knocks you unconscious.")
                                            else:
                                                print("the orc quickly turns around and knocks you unconscious.")
                        elif fight == "sneak" or "sneak by him" or "sneak by" or "sneak to the next room":
                            print(
                                "you attempt to sneak by but the goblin with the bow notices you and fires an arrow which pierces through your chest and you fall down to the ground as you fade into darkness.")
                        else:
                            print("the arrow pierces your flesh and you lose your before falling into the hole")
    elif act2 == "no":
        print(
            "you walk past it and enter the next room but end up being surprised a goblin and get slain. wish you could've gotten that sword to block the attack huh?")
elif act1 == "no":
    print("nothing happens and your still trapped.")
