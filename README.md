# Binaries

## MoveDelay.zip

A small utility to be used for uci chess engines that move instantly. This will add a delay to the move.

Usage:<br/>
- Put this file in the same folder as the engine you want to use exist.
- For most GUI:<br/>
  Create a new file in this folder with the name *MoveDelay.ini*<br/>
  Edit this file and and put these lines in it:<br/>
    ```
    [Engine]
    Path = <filename_of_your_engine>
    ```
- For some GUI:<br/>
    Add the engines filename to the end of the pathline when you install the engine. Ex. *MoveDelay.exe MyEngine.exe*
- Install the MoveDelay.exe as you normaly would install the engine.
  
In the option parameters (configuration) for your engine in the GUI you will see a new option **Movedelay** with the choices: None, Fast, Normal, and Slow
  
I have only tested it with Dragon 2.6.1 with limited strength.
 
For some moves it will still move instantly, these moves like bookmoves, obvious recapture etc.. If you try it and it don't recognize book moves for your engine, please report it as an *Issue*. Other problem/info could be put under *Discussion*.
 
There is a sample *MoveDelay.ini* in the .zip file that you can use as a start. If you don't need it you can delete it. The command line argument are checked first anyway.

For more details on how it works, you can take a peek into the source: https://github.com/OGMalin/Polarchess/tree/master/MoveDelay

History:<br/>
24. jan. 2022 - First release<br/>
25. jan. 2022 - Fixed some time management
17. feb. 2022 - Set the current directory to MoveDelay directory. This help in some cases where the GUI don't do this automatic.
