# A(gon)Basic
A(gon)Basic is a Basic interpreter for develop und run basic programs in my own created basic. It runs on the Agon light 2 computer with MOS 1.04 RC 3 & VDP 1.04 or on Agon Console8 with MOS 2.1.0 & VDP 2.3.0.


![Edit menu from A(gon)Basic](/../main/PICS/ABasic1.jpg)

![Demo JUMPTABLE.BAS](/../main/PICS/ABasic2.jpg)

![Running Demo NUMBER_BENCH.BAS](/../main/PICS/ABasic3.jpg)


To load and run ABasic type in MOS `LOAD ABASIC.BIN` and then `RUN`. You must be in the directory where your ABasic is.

> [!NOTE]
***ABasic at time is still in work. Some functions are still being planned and have no function yet.***


## The menu structure

- File
  - New: Clears the program in editor
  - Load: Load a binary basic file.
  - Save: Save the binary basic file with known name. If name unknown it call "Save as"
  - Directory: Show the current directory in a window
  - Load ascii: Load a basic program that's a text file
  - Save ascii: Save a basic program as a text file
  - Quit ABasic: Exit ABasic

- Edit
  - Start mark: Set the start of edit marker
  - End mark: Set the end of edit marker
  - Copy: Copy the marked lines to the clipboard
  - Cut: Cut of the marked lines and save they in clipboard
  - Paste: Insert the clipboard in editor
  - Insert file: Insert a basic file in the editor
  - Find: Search a word in editor
  - Excanche: Exchange one or more words in the editor
  - Printer setup: Set some parameter for the printer
  - Print: Print the actually program
  - Jump to top: Jump to the first line in the editor
  - Jump to end: Jump to the end line in the editor
  - Cut empty lines: Erase all empty lines from the program
  - Delete line: Erase the actually programm line
  - Insert line: Insert a empty line in the program. Lines after this line will be scroll down

- Execute
  - Run: Run the actually program in editor
  - Breakpoint: Stop the running program at marked line
  - Labels/SUBs/FUNCs: Show then labels, SUBs and FUNCs in the program.

- Tools
  - Options: Open a window to change some ABasic parameter
  - Colors: (Re)define the color sheme
  - Change colors: Switch to next color sheme
  - Number changer: Show a tool to convert numbers in decimal, hexadecimal or binary

- Help
  - Show help: Open the help window
  - Help for: Open the help window and search for the entry where the cursor is
  - Information: Show the program information

### Shortcuts

Any menu entrys have shortcuts. That allows fast execute the function.

|**Keys**|**Menu**|
|--------|--------|
|`[F1]`|Show help|
|`[F2]`|Load|
|`[F3]`|Save|
|`[F4]`|Breakpoint|
|`[F5]`|Run|
|`[F6]`|Load ascii|
|`[F7]`|Save ascii|
|`[F9]`|Labels/SUBs/FUNCs|
|`[F11]`|Help for|
|`[F12]`|Change colors|
|`[CTRL]+[A]`|Save as|
|`[CTRL]+[B]`|Start mark|
|`[CTRL]+[C]`|Copy|
|`[CTRL]+[D]`|Directory|
|`[CTRL]+[E]`|End mark|
|`[CTRL]+[F]`|Find|
|`[CTRL]+[K]`|Cut|
|`[CTRL]+[N]`|Number changer|
|`[CTRL]+[P]`|Print|
|`[CTRL]+[Q]`|Quit ABasic|
|`[CTRL]+[S]`|Exchange|
|`[CTRL]+[U]`|Paste|
|`[CTRL]+[X]`|Delete line|
|`[CTRL]+[Y]`|Insert Line|


## Statements

ABasic has an extensive range of commands. You can view these in the files below.

[Commands](/Commands.md)

[Functions](/Functions.md)

[Operands](/Operands.md)

[Errors](/Errors.md)


## Vriable types

Variables can defined with an ID character. This is the last char of the vraiable name and define with type the variable is. Without a character it define the variable as integer.

|**ID**|**Type**|**Data size**|**Range**|
|------|--------|-------------|---------|
|Vertival line|Byte [^1]|1|0 - 255|
|§|Word [^1]|2|0 - 65535|
|%|Integer|3|0 - 16777215|
|!|Floating point [^1]|4|-1e-38 - 1e37|
|$|String|2 + Length of string|0 - 255 chars|
[^1]: This data format is not yet implemented


## Memory map

A(gon)Basic uses any memory areas. In the follow table you can see which areas are exist:

|**Adress**|**Name**|**Function**|
|----------|--------|------------|
| &40000 | ABasic.bin | A(gon)Basic itself |
| Varying | Jumps | Jump data for labels, procedures and functions |
| Varying | Variables | Data or reference for variables |
| Varying | Heap | Free memory are reserved for heap data |
| &AEC00 | Call | Call stack for nested loops and subroutines |
| &AF000 | Argument | Stack for parameters and evalute formula |
