# A(gon)Basic
A(gon)Basic is a Basic interpreter for develop und run basic programs in my own created basic. It runs on the Agon light 2 computer with MOS 1.04 RC 3 & VDP 1.04 or on Agon Console8 with MOS 2.1.0 & VDP 2.3.0.

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
Let the program time*0.1 seconds wait. At this time you can't break the program. AFTER and EVERY does not work.

### END
Stop the program and return to the enviroment.

### GCOLOR color{,mode}
Set the color for graphic operations. With optional parameter mode it can be define a graphic mode. Without this parameter it will be set to 0.

### GOTO address / jump label
Jump to the given address or to a jump label. With SELFLINE you can jump at the same line that now runs.
***Use only jump labels or SELFLINE. If your address not the begin a program line, ABasic crash.***

### HOME
Set the text cursor at left top of the screen.

### LOCATE X,Y{,CURSOR}
Set the text cursor to the x/y-position. The left top position start with 1,1. Optional you can control the cursor. Values unequal zero activated the cursor. Zero deactivated the cursor.

### MODE mode
Set the screen mode. To show the differnt modes view (https://github.com/AgonConsole8/agon-docs/blob/main/docs/vdp/Screen-Modes.md).

### POKE adress,byte
Writing a byte with 8 bit to the given address.

### POKEI adress,integer
Writing an integer with 24 bit to the given address.

### POKEW adress,word
Writing a word with 16 bit to the given address.

### PRINT / ? {#channel,}parameter{;/,}{parameter}...
Print a parameter at the given channel. If not channel given it will be print on the screen. With ';' you can print any parameter directly behind each other. ',' allows to print any parameter at the next tabulators (each 8 columns).

### REM / '
Define the rest of the line as comment. The interpreter ignore this text and continue with next line.

### RESET
Reset the Agon computer and restart the MOS.

### QUIT
Leave the A(gon)Basic developer enviroment and returns to MOS.

## Functions

### ASC(string)
Get the first char in the string and result the ascii number. An empty string generate an error.

### CHR$(ascii)
Result a string with a character with the the given ascii number.

### DAY
Result the day from the internel RTC.

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

### HIMEM
Result the maximum adress of the user RAM.

### HOUR
Result the hour from the internal RTC.

### LEN(string)
Calculate the length of the string and result it.

### MINUTE
Result the minute from the internal RTC.

### MONTH
Result the month from the internal RTC.

### NUMBER(string)
Check if the string has a changeable number. Result TRUE if is it. Otherwise FALSE.

### PEEK(address)
Read a byte with 8 bit from the given address.

### PEEKI(address)
Read a integer with 24 bit from given address.

### PEEKW(address)
Read a word with 16 bit from given address.

### PAPER color
Set the backgrund color.

### PEN color
Set the text foreground color.

### RAWKEY
Result the vKey value if available. Otherwise it send zero.

### SECOND
Result the second from the internal RTC.

### SELFLINE
Result the address of the line that run now.

### STR$(number)
Create a string with the number.

### STRING$(count,substring)
Create a string that has count times of the substring.

### TEXTCOLS
Result the maximen columns of the textscreen.

### TEXTROWS
Result the maximum rows of the thextscreen.

### TIMER
Result the value of the internal timer. But only 24 bit.

### TRUE
Send the true value = $FFFFFF.

### VAL(string)
Get the binary number from the string. The number must be the first in the string. If not changeable it result 0.

### XPOS
Result the position from the x position of the text cursor.

### YEAR
Return the year from the internal RTC.

### YPOS
Result the position from the y position of the text cursor.
