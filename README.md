# rockpaperscissorpython
#100daysofPython

import random 
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
win = ('''

        ,,,,,,,,,,,,,
    .;;;;;;;;;;;;;;;;;;;,.
  .;;;;;;;;;;;;;;;;;;;;;;;;,
.;;;;;;;;;;;;;;;;;;;;;;;;;;;;.
;;;;;@;;;;;;;;;;;;;;;;;;;;;;;;' .............
;;;;@@;;;;;;;;;;;;;;;;;;;;;;;;'.................
;;;;@@;;;;;;;;;;;;;;;;;;;;;;;;'...................
`;;;;@;;;;;;;;;;;;;;;@;;;;;;;'.....................
 `;;;;;;;;;;;;;;;;;;;@@;;;;;'..................;....
   `;;;;;;;;;;;;;;;;@@;;;;'....................;;...
     `;;;;;;;;;;;;;@;;;;'...;.................;;....
        `;;;;;;;;;;;;'   ...;;...............;.....
           `;;;;;;'        ...;;..................
              ;;              ..;...............
              `                  ............
             `                      ......
            `                         ..
           `                           '
          `                           '
         `                           '
        `                           `
        `                           `,
        `
         `
           `.
''')
lose = ('''
  _..._
             ,'     `.
           ,'         `.
         ,'    _   ,-.  `.
         |    (_)  `-'   |
         |        >      |
         |     ,----.    |
         |    /,-""-.\   |
         `.  |/      "  ,'
           `.         ,'
             `._____,
             ''')

tie = ('''
      88             
  ,d    ""             
  88                   
MM88MMM 88  ,adPPYba,  
  88    88 a8P_____88  
  88    88 8PP"""""""  
  88,   88 "8b,   ,aa  
  "Y888 88  `"Ybbd8"'  
  ''')
#Write your code below this line 👇
inputchoice = input(" choose one from rock, paper, scissors:").lower()
computerchoice = random.choice(['rock', 'paper', 'scissors' ])
if (inputchoice == computerchoice):
  print("draw")
  print(tie)
elif (inputchoice == "rock" and computerchoice == "paper"):
  print("inputchoice:\n", rock)
  print("computerchoice:\n",  paper)
  print("Computer Wins!")
  print(lose)
elif (inputchoice == "paper" and computerchoice == "rock"):
  print("inputchoice:\n", paper)
  print("computerchoice:\n", rock)
  print("User Wins!")
  print(win)
elif (inputchoice == "paper" and computerchoice == "scissors"):
  print("inputchoice:\n", paper)
  print("computerchoice:\n", scissors)
  print("Computer Wins!")
  print(lose)
elif (inputchoice == "scissors" and computerchoice == "paper"):
  print("inputchoice:\n", scissors)
  print("computerchoice:\n", paper)
  print("User Wins!")
  print(win)
