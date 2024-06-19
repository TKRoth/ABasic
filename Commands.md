# Commands

### `BEEP`

Makes a beep.

### `CHDIR / CD directory`

Change the actuelly directory. The new directory must be a string.

### `CIRLE x radius,y radius`

Draw a circle with x and y radius.

### `CLEAR`

Erase all variables.

### `CLG`

Clear the graphic display.

### `CLS`

Clear the text screen and set the text cursor at the left top of the screen.

### `CURSOR state`

Turn on the cursor if state unequal zero. Otherwise the cursor will be hide.

### `DEC variable`

Decrease the value of the given variable. The variable type must be a numeric.

### `DELAY time`

Let the program time*0.1 seconds wait. At this time you can't break the program. AFTER and EVERY does not work.

### `DIR directory / CAT directory`

List the directory that be in the given string.

### `DISC x radius,y radius`

Draw a filled circle with x and y radius in the seted color.

### `END`

Stop the program and return to the enviroment.

### `ERROR error`

Solves an error with given number. If the number greater then error exist it print 'Unknown error'.

### `EXPLICIT`

After this command all variables must declared with the DIM command.

### `FOR variable=start TO end {STEP size}`

Open a counter loop. The specified variable receives the counter value from start to end. The step size can be change with the optional STEP command. Normally it's 1. The FOR command must be close with the NEXT statement.

### `FOREVER`

Close an opening REPEAT loop and let execute the commands within it over and over again.

### `GCOLOR / GCOL color{,mode}`

Set the color for graphic operations. With optional parameter mode it can be define a graphic mode. Without this parameter it will be set to 0.

### `GOSUB adress / jump label`

Calls a subroutine at the adress or at the jump label. You can leave the subroutine with RETURN command.

> [!WARNING]
***Use only jump labels or SELFLINE. If your address not the begin a program line, ABasic crash.***

### `GOTO address / jump label`

Jump to the given address or to a jump label. With SELFLINE you can jump at the same line that now runs.

> [!WARNING]
***Use only jump labels or SELFLINE. If your address not the begin a program line, ABasic crash.***

### `GPRINT / GP parameter{;/,}{parameter}...`

Print a parameter at the graphik position with seted graphik color. With ';' you can print any parameter directly behind each other. ',' allows to print any parameter at the next tabulators (each 8 columns).

### `HOME`

Set the text cursor at left top of the screen.

### `IF condition THEN true commands {ELSE false commands}`

Execute the true commands if the condition unequal zero. If the conditional zero the ELSE part will be execute.

### `INC variable`

Increase the value of the given variable. The variable type must be a numeric.

### `INK color,palette`

Set the color to a palette color from 0 to 63.

### `KILL file/directory`

Kill a file or a directory. The parameter must be a string.

### `LINE x,y`

Draw a line to x,y.

### `LOCATE X,Y`

Set the text cursor to the x/y-position. The left top position start with 1,1.

### `MKDIR / MD directory`

Create a new directory. The directory must be a string.

### `MODE mode`

Set the screen mode. To show the differnt modes view [Screen modes](https://github.com/AgonConsole8/agon-docs/blob/main/docs/vdp/Screen-Modes.md).

### `MOS command`

Call the given MOS command.

### `MOVE x,y`

Set the graphic cursor to x,y.

### `ORIGIN x,y`

Set a new zero point of the graphic screen.

### `PALRGB color,red,gree,blue`

Set the color with the given RGB color. Any ground color can be 0 to 255.

### `PIXELMODE state`

Activates the physical coordinate system when the state is TRUE. This has a resolution dependent from the mode. Here start the x/y-counting at left top. To deactivated the physical coordinate system the state must be false. 
 
### `PLOT x,y`

Plot a point at x,y.

### `POKE adress,byte`

Writing a byte with 8 bit to the given address.

### `POKEI adress,integer`

Writing an integer with 24 bit to the given address.

### `POKEW adress,word`

Writing a word with 16 bit to the given address.

### `PRINT / ? {#channel,}parameter{;/,}{parameter}...`

Print a parameter at the given channel. If not channel given it will be print on the screen. With ';' you can print any parameter directly behind each other. ',' allows to print any parameter at the next tabulators (each 8 columns).

### `RECTANGLE / RECT width,height`

Draw a filled rectangle with size of width and height in the seted color.

### `REM / '`

Define the rest of the line as comment. The interpreter ignore this text and continue with next line.

### `REPEAT`

Open a loop. If the loop closed by FOREVER the loop will run over and over again while not BREAK or LEAVE command executes. UNTIL let the loop run until the condition are true.

### `RESET`

Reset the Agon computer and restart the MOS.

### `RETURN`

Leave a subroutine and go to after the calling GOSUB command.

### `SWAP variable 1,variable 2`

Swap the values of the variables. Both variables must be the same type.

### `TRIANGLE width,height`

Draw a filled triangle with width and height in the seted color.

### `QUIT`

Leave the A(gon)Basic developer enviroment and returns to MOS.
