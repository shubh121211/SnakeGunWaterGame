# SnakeGunWaterGame
import random
computer = random.choice([-1,0,1])
your_entery=input("enter your choise : ")
yt_dict={"s":-1 , "w":0 , "g":1 } 
reverse_Dict={-1:"snake" , 0:"water" , 1:"gun"}

you = yt_dict[your_entery]

print(f"your choise :{reverse_Dict[you]} \n computer choise : {reverse_Dict[computer]}")
if(computer == you):
    print("it's a draw!")
else:
    if(computer ==-1 and you == 1):
        print("You Win !")
    elif(computer ==-1 and you == 0):
        print("You lose !")
    elif(computer ==0 and you == 1):
        print("You lose !")
    elif(computer ==0 and you == -1):
        print("You Win !")
    elif(computer ==1 and you == -1):
        print("You lose !")
    elif(computer ==1 and you == 0):
        print("You win !")
    else:
        print("Something went wrong!")
