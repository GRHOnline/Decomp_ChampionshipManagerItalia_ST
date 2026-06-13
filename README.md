# Championship Manager Italia, Atari ST decompilation

A decompilation of the Atari ST game Championship Manager Italia. This is the hard drive install of the game and not the floppy disk based version.
I have added a version which bypasses the copy protection it is called "nocheck.prg" it is located in the game folder. It may have some bugs if so please let me know if you find any.
Also I have added a version for Championship Manager '93 ( English not Italian version ) in the CMAN93 folder.

This is my first full decompilation and was done using a combination of Ghidra and Fred's dissasembler ( https://atari-forum.com/viewtopic.php?t=14540 )
The code is assembled using VASM\VBCC ( http://www.compilers.de/vasm.html ) with the following commands :-
C:\STFM\VCC\vbcc\bin\vasmm68k_mot decomp.asm -m68000 -Ftos -devpac -o C:\STFM\HD\ITALIA\recomp.prg

The program can be compiled and run but it is not 100% accurate to the original. I have tested it with the Hatari emulator and found no problems.
The code has been cleaned up so it can be assembled with RMAC, just comment out lines ending with VASM and re-instate the lines ending with RMAC

Completion ratio
--------------------
100% DRI / GST File header 

 99% .TEXT section / code
 
100% .DATA section

100% .BSS section / undefined variables

100% Fix up Information / Relocation Table
  

I have commented out the code which will enable you to skip the Copy Protection / Manual check you just need to re-enable them in the PRE_DRM_CHECK00 section.

Asset information
---------------------
The program contains a sndh file within it which is the same as the one used by Championship Manager 93 ( written by Matt Furniss ) a copy is provided for comparison.
Taken from SNDH Atari ST YM2149 Collection website https://sndh.atari.org
The SNDH file format contains code to play itself and needs to be activated, I have not decompiled this just copied the relevant block of data into a .bin file.

The image data used ( intelek.pic, picture1.pic, title.pic) are a non compressed type which is copied exactly as it is to the screen and provides no palette data.

