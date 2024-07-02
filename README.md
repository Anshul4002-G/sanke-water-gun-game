# sanke-water-gun-game

"""
1=snake
-1=water
0=gun
"""

import random
yourstr=input("enter your choice")
youdict={"snake":1,"water":-1,"gun":0}
computer=random.choice([-1,0,1])
you = youdict[yourstr]

reversedict={1:"sanke",-1:"water",0:"gun"}

print(f" you choose {reversedict[you]} \n and computer choose {reversedict[computer]}")
if(computer==you):
    print("draw")
else:
    if(computer==-1 and you==1):
      print("you win")
    elif(computer==-1 and you ==0):
      print("you lose!")
    elif(computer==1 and you ==-1):
      print("you lose!")
    elif(computer==1 and you ==0):
      print("you win")
    elif(computer==0 and you == -1 ):
     print("yoou win")
    elif(computer==0 and you ==1):
     print("you lose!")
    else:
     print("something went wrong   ")
