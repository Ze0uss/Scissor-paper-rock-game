# Scissor-paper-rock-game
- Scissor paper rock game with the help of python 




* How to Play Rock, Paper, Scissors: A Simple Guide 

- Rock, paper, scissors (also known as Rochambeau, Roshambo, or Janken) is a fun and easy hand game that anyone can learn and enjoy.
 It’s a great way to make minor decisions when you and a friend can’t agree on something, or even just an entertaining way to pass the time.
 The neat thing about the game is that almost anybody can pick the rules up in a matter of seconds.
 In this article, we’ll break the game down so that you and a friend can play whenever you’d like.


* Things You Should Know

1. Rock beats scissors, scissors beat paper, and paper beats rock.
2. Agree ahead of time whether you’ll count off “rock, paper, scissors, shoot” or just “rock, paper, scissors.”
3. Use rock, paper, scissors to settle minor decisions or simply play to pass the time.

             
             
             
  '''The random module is a built-in module to generate the pseudo-random variables.
  It can be used perform some action randomly such as to get a random number, selecting a random elements from a list, shuffle elements randomly, etc '''
             
             
             
             
           import random
             
                def gameWin(comp, you):
                    if comp == you:
                        return None
                        
                    elif comp == 's':
                        if you == 'p':
                          return False
                        elif you == 'r':
                          return True

                   elif comp == 'p':
                        if you == 'r':
                            return False
                       elif you == 's':
                          return True

                  elif comp == 'r':
                      if you == 's':
                          return False
                      elif you == 'p':
                          return True


              # print("Comp turn: Scissor(s) Paper(p) Rock(r)")
              randNo = random.randint(1, 3)
              if randNo == 1:
                  comp = 's'
              elif randNo == 2:
                  comp = 'p'
              elif randNo == 3:
                  comp = 'r'

              print("Scissor(s) Paper(p) Rock(r)?")
              you = input("your turn:  \n ")
              a = gameWin(comp, you)

              print(f"Computer chose:  {comp}")
              print(f"you chose:  {you}")

              if a == None:
                  print("The game is tie")
              elif a:
                  print("You Win! ")
              else:
                  print("You Lose! ")
                  
                  
                  
                  



A simultaneous, zero-sum game, it has three possible outcomes: a draw, a win or a loss.
A player who decides to play rock will beat another player who has chosen scissors ("rock crushes scissors" or "breaks scissors" or sometimes 
"blunts scissors" but will lose to one who has played paper ("paper covers rock"); a play of paper will lose to a play of scissors ("scissors cuts paper"). 
If both players choose the same shape, the game is tied and is usually immediately replayed to break the tie.


Rock paper scissors is often used as a fair choosing method between two people, similar to coin flipping, drawing straws, 
or throwing dice in order to settle a dispute or make an unbiased group decision. Unlike truly random selection methods, however, 
rock paper scissors can be played with a degree of skill by recognizing and exploiting non-random behavior in opponents.
    
