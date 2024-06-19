# Functions

## `@variable`

Is the short version from the VARPTR function.

## `ASC(string)`

Get the first char in the string and result the ascii number. An empty string generate an error.

## `BIN$(number)`

Result a string with the binary value of the given nummber.

## `CHR$(ascii)`

Result a string with a character with the the given ascii number.

## `DAY`

Result the day from the internel RTC.

## `FALSE`

Send the false value = $000000.

## `FREE`

Result the free user RAM.

## `GETCOLORS`

Result the count of colors you can use in the actually screen mode.

## `GETMODE`

Result the actually screen mode.

## `GRAPHWIDH`

Result the width resolution of the graphic screen.

## `GRAPHHEIGHT`

Result the height resolution of the graphic screen.

## `HEX$(number)`

Result a string with the hexadezimal value of the given nummber.

## `HIMEM`

Result the maximum adress of the user RAM.

## `HOUR`

Result the hour from the internal RTC.

## `INSTR(string,ascii)`

Search the ascii char in the string and result the position if found. If not found the function results 0.

## `LEN(string)`

Calculate the length of the string and result it.

## `LEFT$(string,size)`

Result size chars from the left of the string.

## `LOWER$(string)`

Converts the string to lowercase.

## `LTRIM$(string)`

Erase the spaces from left of the string.

## `MID$(string,start,length)`

Result string that a cut from start with length chars.

## `MINUTE`

Result the minute from the internal RTC.

## `MONTH`

Result the month from the internal RTC.

## `NOT(value)`

Invert the value.

## `NUMBER(string)`

Check if the string has a changeable number. Result TRUE if is it. Otherwise FALSE.

## `PEEK(address)`

Read a byte with 8 bit from the given address.

## `PEEKI(address)`

Read a integer with 24 bit from given address.

## `PEEKW(address)`

Read a word with 16 bit from given address.

## `RANGE(value,minimum,maximum)`

Check whether the value is between the minimum and the maximum.

## `RAWKEY`

Result the vKey value if available. Otherwise it send zero.

## `RIGHT$(string,size)`

Result size chars from the right of the string.

## `RTRIM$(string)`

Erase the spaces from right of the string.

## `SECOND`

Result the second from the internal RTC.

## `SELFLINE`

Result the address of the line that run now.

## `STR$(number)`

Create a string with the number.

## `STRING$(count,substring)`

Create a string that has count times of the substring.

## `TEXTCOLS`

Result the maximen columns of the textscreen.

## `TEXTROWS`

Result the maximum rows of the thextscreen.

## `TIMER`

Result the value of the internal timer. But only 24 bit.

## `TRIM$(string)`

Erase the spaces from both sides from the string.

## `TRUE`

Send the true value = $FFFFFF.

## `UPPER$(string)`

Converts the string to uppercase.

## `VAL(string)`

Get the binary number from the string. The number must be the first in the string. If not changeable it result 0.

## `VARPTR(variable)`

Result the adress of the data area from the variable.

## `XPOS`

Result the position from the x position of the text cursor.

## `YEAR`

Return the year from the internal RTC.

## `YPOS`

Result the position from the y position of the text cursor.
