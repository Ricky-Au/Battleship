# Battleship
Description:
     This battleship esq games rules are the player takes turns against a computer player both sides goals are to take down all of the oppenents ship before they take all of yours. Our version is written in C++ and requires the arduino and the use of serial monitor to see the battlefield. The use of the arduino is for a minigame for the player.

The arduino must be set up properly to be able to play. The point of the arduino is so the player has a minigame to play through when they attack an opponents ship location. This minigames rules are as follows, This minigame only uses the 3 right LEDs. Press and hold a lit LED's button when they turn on until the LED turns off. Each successful button press increases your score by 1. For a successful ship hit get above 5 score on Easy, above 10 on Medium or Hard. Your score will update on screen. Press leftmost fire button when ready - the leftmost green LED will stay on during the game The game lasts 10 seconds.

This version of battleship also has three difficulties (easy medium and hard). 
Where easy mode you go first both sides have the same amount of ships(5). 
Medium mode the bot goes first and they start with (7) ships while you still have the same (5). 
Hard mode the bot goes first and they take two turns for every turn you take. 
All of these diffuculties include the minigame difficulties too ie you get less time to complete the minigame 10-15 seconds.


Included Files:
    * battleship.cpp
    * README
    * Makefile
    * read_int.h
    * arduinoSetup.jpg (picture of the setup)

Accessories:
  - 560 Ohm (Greenn Blue Brown) resistor x 5
  - LED (Grn) x 4
  - LED (Red) x 1
  - Arduino Mega Board (AMG)
  - Button x 4

Wiring Instructions:

  Arduino Pin 13 <--> Longer LED lead |LED| Shorter LED lead <--> Resistor <--> GND

  Arduino Pin 12 <--> Longer LED lead |RED LED| Shorter LED lead <--> Resistor <--> GND

  Arduino Pin 11 <--> Longer LED lead |LED| Shorter LED lead <--> Resistor <--> GND

  Arduino Pin 10 <--> Longer LED lead |LED| Shorter LED lead <--> Resistor <--> GND

  Arduino Pin 9 <--> Longer LED lead |LED| Shorter LED lead <--> Resistor <--> GND

  Arduino Pin 7 <--> Button lead |Button| Button lead <--> GND

  Arduino Pin 6 <--> Button lead |Button| Button lead <--> GND

  Arduino Pin 5 <--> Button lead |Button| Button lead <--> GND

  Arduino Pin 4 <--> Button lead |Button| Button lead <--> GND

Running Instructions:
    1) Make sure your serial-mon is in full screen or else the visuals of the game will not show up properly
    2) enter the file directory and type "make upload && serial-mon" into the terminal
    3) when prompted a difficulty type in the appropriate diffuculty for user press enter
    4) press enter again when prompted to start the game
    5) input the coordinates you wish to attack
    6) further instructions will be displayed on serial-mon once you get passed Running Instructions 1)

Notes:
    1) sometimes when you run after inputing a diffuculty and entering the game will freeze if it does just reset the game. By pressing the red reset buttom on arduino

Sources:

  function void aiPath() line 238
  https://forum.arduino.cc/index.php?topic=345964.0
  user johnwasser

  function Minigame() line 69
  https://arduino.stackexchange.com/questions/22272/how-do-i-run-a-loop-for-a-specific-amount-of-time
  user JRobert
  
  Game as a whole is based on the hit game Battleship by Hasbro.
