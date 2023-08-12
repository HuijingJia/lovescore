#this is love match test project.
print("Welcome to the Love Calculator!\nScore(40-50) means match perfectly;\nScore(<10 or >90) means you go together like coke and mentos;\nTry your score by typing your names:")
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")

name = name1 + name2
name = name.lower()  

T = name.count("t")
R = name.count("r")
U = name.count("u")
E = name.count("e")

number_true = T + R + U + E
number_TRUE = str(number_true)

L = name.count("l")
O = name.count("o")
V = name.count("v")
E = name.count("e")

number_love = L + O + V + E
number_LOVE = str(number_love)

score = int(number_TRUE + number_LOVE)

if (score < 10) or (score > 90):
    print(f"Your score is {score}, you go togrther like coke and mentos.")
elif score >= 40 and score <= 50:
    print(f"Your score is {score}, you are alright together.")
else:
    print(f"Your score is {score}.")

