Ghidra Download
used to decompile the game's executable code
https://ghidra-sre.org/
important: make sure you extract the folder to your local disc, 
and make sure you have the latest version of JDK installed.

Languages folder:
Copy all the files from the data/languages folder to 
Ghidra/Processors/PowerPC/data/languages of your Ghidra installation. 
To use the language, select it in the language selection menu which is 
PowerPC 32 bit big endian Gekko/Broadway variant. Upon using the language, 
the .sla file should be compiled automatically.

GCRebuilder
used to extract and rebuild the game iso
https://www.romhacking.net/utilities/619/

DolTool
used to convert the game's Start.dol file to .elf format
run the program from the command prompt and make sure the .dol file is 
in the same location

Star.dol
The game's executable code (from the extracted iso)

---------------------------------------------------------------------------------

How to use
Locate the Start.dol file Bring that file to the same location as the DolTool.exe 
and run the tool via command prompt to convert .dol to .elf. Next, follow the intructions under the 
Languages folder section above. Finally, run Ghidra and make sure to select the 
PowerPC 32 bit big endian Gekko/Broadway variant when asked to choose a language. 
After running, Ghidra will ask if you want to analyze the code, select yes then 
the decompiled code should display in Ghidra.

If you want to test the game in dolphin, you will need GCRebuilder. Obtain the Game's
iso file and open it using GCRebuilder and extract the files. Locate the Start.dol
file under the &&systemdata folder under the root folder. Replace your custom Start.dol
file with the existing one, then rebuild the iso. Next, move the iso to your dolphin's
game directory and run the game.