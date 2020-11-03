# Mario Super Stars Baseball Modding Project
This is a collaborative project attempting to mod the Mario Super Stars Baseball game, on the Nintendo GameCube.

In this README, you can find instructions on [how to mod](#howto) the game as well as [download links](#tools) and brief explanations on the tools needed.

---

## <a id="howto">How to use</a>
Locate the [Start.dol](#start) file and bring that file to the same location as the DolTool.exe
and run the tool via command prompt to convert .dol to .elf.

Next, follow the intructions under the
Languages folder section above. Finally, run Ghidra and make sure to select the
PowerPC 32 bit big endian Gekko/Broadway variant when asked to choose a language.

After running, Ghidra will ask if you want to analyze the code, select yes then
the decompiled code should display in Ghidra.

1. If you want to test the game in dolphin, you will need [GCRebuilder](#gcrebuilder).
2. Obtain the Game's iso file and open it using GCRebuilder and extract the files.
3. Locate the [Start.dol](#start) file under the &&systemdata folder under the root folder.
4. Replace your custom [Start.dol](#start) file with the existing one, then rebuild the iso.
5. Next, move the iso to your [Dolphin's](#dolphin) game directory and run the game.

---
## <a id="tools">Tools Needed</a>

### Dolphin download

[Dolphin](https://dolphin-emu.org/download/) is an emulator for both the GameCube and Wii.

Dolphin is how you can test if your modifications have worked.

### Ghidra Download

[Ghidra](https://ghidra-sre.org/) is used to decompile the game's executable code.

__Important:__ make sure you extract the folder to your local disc,
and make sure you have the latest version of JDK installed.

### Languages folder:
Copy all the files from the data/languages folder to
Ghidra/Processors/PowerPC/data/languages of your Ghidra installation.
To use the language, select it in the language selection menu which is
PowerPC 32 bit big endian Gekko/Broadway variant. Upon using the language,
the .sla file should be compiled automatically.

### <a id="gcrebuilder">GCRebuilder</a>
[GCRebuilder](https://www.romhacking.net/utilities/619/) is used to extract and rebuild the game iso

### DolTool
DolTool is used to convert the game's Start.dol file to .elf format.

Run the program from the command prompt and make sure the .dol file is in the same location

### <a id="start">Start.dol</a>
The game's executable code (from the extracted iso)
