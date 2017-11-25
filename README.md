# guessinggame
Generate a random number between 1 and 9 (including 1 and 9). Ask the user to guess the number, then tell them whether they guessed too low, too high, or exactly right.Extras:  Keep the game going until the user types “exit” Keep track of how many guesses the user has taken, and when the game ends, print this out.







import random as f


t=f.randint(0,10)
time=0
guess=0
ks="y"
while True:
	print("Hi Melody Lets Play A Game")
	guess=input("please guess the num between 1-9 ")
	g=int(guess)
	if g==t:
		print("you guess right")
		time+=1
		print("you guess ", time ,"times")
		time=0
	if g<t:
		print ("you guess low")
		time+=1
	if g>t:
		print("you guess high")
		time+=1
	k=input("type exit to quit or click enter to continue")
	if k=="exit":
		break
print("game has been exited")

