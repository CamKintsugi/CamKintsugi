#this is my simple dungeon script
import random

#starting health
health = 100

#into to the dungeon. pick a direction.
print("""You enter a dark dungeon.
There are walls to the east, west, and south. 
To the north is an open passage way. 
Do you go north? 1 for yes, 2 for no""")

#where are we going?
go = input("> ")

#set up the enemy
while health in range(1, 101):
	if go == "1":
		print("You encounter a spider. What do you do?")
		print("1. Hit the spider.")
		print("2. Do nothing.")
		print("3. Check health.")
		attack = input("> ")
		if attack == "1":
			print("You attacked and killed the spider.")
			print("There is an open passage way to the north.")
			print("Do you continue north? 1 for yes, 2 for no.")
			go = input("> ")
			if go == "1":
				health = 102
				print("Congrats! You found the exit! You win!")
			elif go == "2":
				health = 0
				print("You die a slow death of starvation. Game over.")
			else:
				print("What else do you think you can do here?")
		elif attack == "3":
			print(f"{health}")
		else:
			print("The spider attacked you. You lost health.")
			dmg = random.randrange(1, 11)
			health = health - dmg
			print(f"You have {health} health remaining.")
			if health <= 0:
				print("You have died. Game over.")

	else:
		health = 0
		print("You die a slow death of starvation. Game over.")
