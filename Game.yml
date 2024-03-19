import random
comp1 =0
comp2 =0
com1_win=0
com2_win=0
Lst = ["Rock", "Paper", "Scissor"]
def Computer_Choose():
     Computer1_choose()
     Computer2_choose()
     win()

def Computer1_choose():
     c1 = random.choice(Lst)
     return c1
def Computer2_choose():
     c2 = random.choice(Lst)
     return c2
def win():
     comp1 =Computer1_choose()
     comp2 =Computer2_choose()
     if comp1 == "Rock":
          if comp2 == "Rock":
               print("\nComputer1 choose Rock & Computer2 Choose Rock.\n Tied ")
          elif comp2 == "Paper":
               print("\nComputer1 Choose Rock & Computer Choose Paper\n Computer1 Lose \n Computer2 win ")
          elif comp2 == "Scissor":
               print("\nComputer1 Choose Rock & Computer2 Choose Scissor. \nComputer1 Win \n Computer2 Lose")
     elif comp1 == "Paper":
          if comp2 == "Rock":
               print("\nComputer1 choose Paper & Computer2 Choose Rock. \n Computer1 win \n Computer2 Lose")
          elif comp2 == "Paper":
               print("\nComputer1 choose Paper & Computer2 Choose Papre. \n Tied")
          elif comp2 == "Scissor":
               print("\nComputer1 Choose Paper & Computer2 Choose Scissor.\n Computer1 Lose \n Computer2 win")
     elif comp1 == "Scissor":
          if comp2 == "Rock":
               print("\nComputer1 choose Scissor & Computer2 Choose Rock. \n Computer1 win \n Computer2 Lose ")
          elif comp2== "Paper":
               print("\nComputer1 choose Scissor & Computer2 Choose Papre \n Computer1 Lose \n Comuter2 Win ")
          elif comp2 == "Scissor":
               print("\nComputer1 Choose Scissor & Computer2 Choose Scissor.\n Tied")

def User_choose():
     Human = input("Enter Your Choose\n\t@. Rock\n\t@. Paper\n\t@. Scissor\n")
     if Human  in ["Rock", "rock", "r", "R"]:
          Human = "Rock"
          return Human
     elif Human in ["Paper", "paper", "p", "P"]:
          Human = "Paper"
          return Human
     elif Human in ["Scissor", "scissor", "s", "S"]:
          Human = "Scissor"
          return Human
     else:
          print("I don't understand, Try again\n")
          return User_choose()

def finle():
     comp1 = User_choose()
     comp2 = Computer2_choose()
     if comp1 =="Rock":
          if comp2=="Rock":
               print("\nYour choose Rock & Computer Choose Rock.\n Tied ")
          elif comp2=="Paper":
               print("\nYour Choose Rock & Computer Choose Paper\n Your Lose \n Computer win ")
          elif comp2=="Scissor":
               print("\nYour Choose Rock & Computer Choose Scissor. \n You Win \n Computer Lose")
     elif comp1=="Paper":
          if comp2=="Rock":
               print("\nYour choose Paper & Computer Choose Rock. \n YOu win \n Computer Lose")
          elif comp2=="Paper":
               print("\nYour choose Paper & Computer Choose Papre. \n Tied")
          elif comp2=="Scissor":
               print("\nYour Choose Paper & Computer Choose Scissor.\n You Lose \n Computer win")
     elif comp1=="Scissor":
          if comp2=="Rock":
               print("\nYour choose Scissor & Computer0 Choose Rock. \n You win \n Computer Lose ")
          elif comp2=="Paper":
               print("\nYour choose Scissor & Computer Choose Papre \n You lose \n Comuter Win ")
          elif comp2=="Scissor":
               print("\nYour Choose Scissor & Computer Choose Scissor.\n Tied")

print("\t\tWelcome to Rock Papar Scissor Game\n")
while True:
     print("Enter YOur Choose\n\t@. Computer \n\t@. Human\n\t@. End Game")
     User = input("")
     if User in ["Computer", "C", "computer", "c"]:
          C = Computer_Choose()
          while True:
               print("")
               user_choice = input("Do you want to play again? (Yes/No)\n")
               if user_choice in ["Y", "y", "yes", "Yes"]:
                    Computer_Choose()
               elif user_choice in ["N", "n", "no", "No"]:
                    print("")
                    break
               else:
                    print("##I don't Understand ##\n")
     elif User in ["Human", "H", "h", "human"]:
          f = finle()
          while True:
               print("")

               user_choice = input("Do you want to play again? (Yes / NO)\n")
               if user_choice in ["Y", "y", "yes", "Yes"]:
                    finle()
               elif user_choice in ["N", "n", "no", "No"]:
                    print("")
                    break
               else:
                    print("##I don't Understand##\n")

     elif User in ["end","e","End","E"]:
          print("\nThanks Play This Game@@@@")
          break

     else:
          print("Try Again ")

