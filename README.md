# A(gon)Basic
A(gon)Basic is a Basic interpreter for develope und run basic programs in my own created basic. It runs at the Agon light 2 computer with MOS 1.04 RC 3 & VDP 1.04 or an Agon Console8 with MOS 2.1.0 & VDP 2.3.0.

To load and run ABasic type in MOS `LOAD ABASIC.BIN` and then `RUN`. You must be in the directory where your ABasic is.


## Commands


### BEEP
Makes a beep.


### CLEAR
Erase all variables.


### CLG
Clear the graphic display.


### CLS
Clear the text screen and set the text cursor at the left top of the screen.


### DELAY time
Let the program time*0.1 seconds wait. At this time yoe can't break the program. AFTER and EVERY doeas not work.


### END
Stop the program and return to the enviroment.


### GOTO adress / jump label
Jump to the given adress or to a jump label. With SELFLINE you can jump at the same line that now runs.

***Use only jump labels or SELFLINE. If your adress not the begin a program line, ABasic crash.***


### HOME
Set the text cursor at left top of the screen.


### MODE mode
Set the screen mode. To show the differnt modes view (https://github.com/AgonConsole8/agon-docs/blob/main/docs/vdp/Screen-Modes.md).


### PRINT {#channel,}parameter{;/,}{parameter}...
Print a parameter at the given channel. If not channel given it will be print on the screen. With ';' you can print any parameter directly behind each other. ',' allows to print any parameter at the next tabulators (each 8 columns).


### REM / '
Define the rest of the line as comment. The interpreter ignore this text and continue with next line.


### RESET
Reset the Agon computer and restart the MOS.


### QUIT
Leave the A(gon)Basic developer enviroment and returns to MOS.


## Functions


### FALSE
Send the false value = $000000.


### FREE
Result the free user RAM.


### GETCOLORS
Result the count of colors you can use in the actually screen mode.


### GETMODE
Result the actually screen mode.


### GRAPHWIDH
Result the width resolution of the graphic screen.


### GRAPHHEIGHT
Result the height resolution of the graphic screen.


### PAPER color
Set the backgrund color.


### PEN color
Set the text foreground color.


### RAWKEY
Result the vKey value if available. Otherwise it send zero.


### SELFLINE
Result the adress of the line that run now.


### TEXTCOLS
Result the maximen columns of the textscreen.


### TEXTROWS
Result the maximum rows of the thextscreen.


### TRUE
Send the true value = $FFFFFF.
