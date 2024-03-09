# Simple-Maths-practice-game-using-python
      import random
      print("Welcome to the game.\nThis game is generally for kids who are in class 1, 2, 3")
      cl = int(input("Enter your class:"))
      if cl > 3 or cl <= 0:
          print("Sorry")
      else:
          k = int(input("Enter the number of questions you want to practice (Enter number > 0):"))
      
          for i in range(k):
              print("1) Addition\n2) Subtraction\n3) Multiplication\n4) Division")
              a = int(input("Enter the option from above that you want to practice today:"))
      
              b = random.randint(10 ** (cl - 1), 10 ** cl - 1)
              c = random.randint(10 ** (cl - 1), 10 ** cl - 1)
      
              if a == 1:
                  print(b, "+", c, "=")
                  e = int(input("Enter your answer:"))
                  d = b + c
              elif a == 2:
                  print(b, "-", c, "=")
                  e = int(input("Enter your answer:"))
                  d = b - c
              elif a == 3:
                  print(b, "*", c, "=")
                  e = int(input("Enter your answer:"))
                  d = b * c
              elif a == 4:
                  print(b, "/", c, "=")
                  e = int(input("Enter your answer in integer term:"))
                  d = b // c  # Use integer division
              else:
                  print("Choose among the options")
      
              if d == e:
                  print("Right answer")
              else:
                  print("Wrong answer")
