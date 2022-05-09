# py-password-generator

https://replit.com/@alizoresh/pypasswordgenerator#main.py

# Password Generator Project

import random

	letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']

	numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']

	symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

	print("Welcome to the PyPassword Generator!")

	nletter = int(input("How many letters would you like in your password?\n")) 

	nsymbols = int(input(f"How many symbols would you like?\n"))

	nnumbers = int(input(f"How many numbers would you like?\n"))


# hard method

	passwordlist=[]

	for let in range(1,nletter+2):
		passwordlist.append(random.choice(letters))
 	for sym in range(1,nsymbols+1):
		passwordlist.append(random.choice(symbols))
 	for num in range(1,nnumbers+1):
		passwordlist.append(random.choice(numbers))
	
# diect result of for loop of py password

	print(passwordlist)

#shuffle random password but in list

	random.shuffle(passwordlist)

	print(passwordlist)

#Converting the list in to string by using for loop

	password = ""

	for char in passwordlist:
		password+=char
		print(password)

# for checking purpose

	print(type(password))

# the end
# one another method easy:
#Easy method

	passwordeasy=""
	for char in range(1,nletter+2):
  	passwordeasy+= random.choice(letters)
	for char in range(1,nsymbols+1):
  	passwordeasy+= random.choice(symbols)
	for char in range(1,nnumbers+1):
  	passwordeasy+= random.choice(numbers)
	print(passwordeasy)
#end of easy method
