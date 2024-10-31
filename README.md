# Five-room-dungeon-
Five-room-dungeon 
#  date written: 10/22/2024
import random


print("FRD Please input your name")
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
print(name, "your intelligence is",intelligence)
print(name, "your agility is",agility)
print(name, "your luck is",luck)


enemy = input("What is your enemies name?")


s = random.randint(1, 10)
f = random.randint(1, 10)
p = random.randint(1, 10)
e = random.randint(1, 10)
c = random.randint(1, 10)
i = random.randint(1, 10)
a = random.randint(1, 10)
l = random.randint(1, 10)
print(enemy,"health is", s)
print(enemy, "strength is", f)
print(enemy, "your perception is", p)
print(enemy, "your endurance is", e)
print(enemy, "your charisma is", c)
print(enemy, "your intelligence is",i)
print(enemy, "your agility is",a)
print(enemy, "your luck is",l)
# all we have done rn, updates coming soon.
print("Thank you for Giving me your name your goal is to solve puzzles and beat",enemy,"at the end good luck Warrior.")
