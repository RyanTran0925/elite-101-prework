# elite-101-prework
import random

def recheck():
  recheck = input("do you need anything else?")
  while recheck == ("yes"):
   print(choice())

def reservation():
 clock = input("what time is good for you?")
 print(f"we will see you at {clock}")
print(recheck)

def order_up():
  order = input("what would you like?")
  if order == ("crackers"):
    print("your crackers are coming")
  elif order == ("banana"):
    print("your banana is coming")
  elif order == ("house-made flan"):
    print("your house-made flan is coming")
  elif order:
    print("i believe we do not have that here")
    print(order)       

def menu ():
  print ("1. Crackers")
  print ("2. Banana")
  print ("3. Flan")
  selection = int(input("Enter choice: "))
  if selection==1:
    Crackers ()
  elif selection==2:
    Banana ()
  elif selection==3:
    Flan ()
  else:
    print("Invalid Choice. Enter 1-3")
    menu()



def Crackers ():
  print ("The cracker is a small biscuit made up of mostly water and flour. The cracker is also seasoned with salt for flavor")
  recheck()

def Banana():
  print ("The banana is a unique fruit that is found in the tropical area of central america. The banana has a sweet taste to it")
  recheck()

def Flan():
   print("Made with eggs, condensed milk, and whole milk. The house-made flan has a sweet and soft taste to it")
   recheck()

def rewind():
  responses = [
    "Hm, i seem to not understand, please try again",
    "may you repeat that please?",
    "Im sorry, but I do not understand"
  ]
  return random.choice(responses)
  print(choice)

choice = input("1.make reservation\n 2.order food\n 3.check menu\n what would you like to do?\n")

if choice == ("1"):
    time = input("what time is good for you?")
    out_put = print("we will see you at {time}")
    #print(recheck)

elif choice == ("2"):
  print(order_up())

elif choice == ("3"):
  print(menu())

elif choice:
  print(rewind())
