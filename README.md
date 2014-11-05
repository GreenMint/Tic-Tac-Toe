Tic-Tac-Toe
===========

This is the code of the game Tic Tac Toe I created during class last year when I was finished with the other assignments.
The code is sloppy and not refactored. 

Since I dont know how to show the GUI of an application written in the Java-Editor on github, here is a screenshot:
http://i.imgur.com/qUccztP.png


Functions
===========

turn() :
    Game mode 1 (Player vs. Player):
      At first it is checked whether the game is still running or not by using a boolean. Then if it is the turn of Player 1
      or Player 2. At last the button which is clicked is assigned the variable of the Player(p1 - 1, p2 - 2) and the 'X' for
      Player 1 or the 'O' for Player 2 if the button has not yet been pressed.
      
    Game mode 2 (Player vs. Computer(easy)): 
      The choice by this computer is made by creating a random number between 0 and 8 using the computer() function.
      
    Game mode 2 (Player vs. Computer(normal)):
      This computer is almost the same as the easy one with just a minor difference. Again a random number is created and 
      if it is less or equal than a certain number the computer hinders the clayer to win with the block() function.
    
    Game mode 2 (Player vs. Computer(hard)):
      The computer with the hardest difficulty always checks if it can win first. If not it tries to hinder the player to
      win. If neither is possible the turn is made with a random number again.
      
    At the end of each turn in every game mode the check() function is called to check if the game has ended with the
    move made this turn.
      
sLabel() :
    This function is just used for convenience in the block() and win() functions.
    
block() :
    The block() function is responsible for checking whether or not the player could win the next turn and preventing it.
    
win() :
    win() is checking if there is a possible move for the computer to make to win this round.
    
check() :
    Checking if there is a winning condition met by either player or if there arent any more possible moves to make. If so
    the game ends and the winner is displayed. Draw is displayed if neither of the players won. The score of the winner is 
    raised by one.
    
    

      
