# Binaries

MoveDelay.zip

A small utility to be used for chess engines that move instantly. This will add a delay to the move.
Usage:

- Put this file in the same folder as the engine you want to use exist.
- For most GUI:
  Create a new file in this folder with the name MoveDelay.ini
  Edit this file and and put these lines in it:
    [Engine]
    Path = <filename of your engine>
  For some GUI:
    Add the engines filename to the end of the pathline when you install the engine. Ex. MoveDelay.exe MyEngine.exe
- Install the MoveDelay.exe as you normaly would install the engine.
  
In the option parameters (configuration) for your engine in the GUI you will see a new option MoveDelay with the choices: None, Fast, Normal, and Slow
  
I have only tested it with Dragon 2.6.1 with limited strength.
 
For some moves it will still move instantly, these moves are bookmoves and where there is only one legal move. If you try it and it don't recognize book moves, please report it as an Issue.
