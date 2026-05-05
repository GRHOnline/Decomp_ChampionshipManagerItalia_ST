# Decomp_ChampionshipManagerItalia_ST

This is currently incomplete as I am still working on the main .asm file to get 100% compatability, I will upload it once it is done.

A decompilation of the Atari ST game Championship Manager Italia. This is the hard drive install of the game and not the floppy disk based version. It still has working DRM which requires you to type in football scores from the manual. I have not removed that, YET.

The program contains a sndh file within it which is the same as the one used by Championship Manager 93 ( written by Matt Furniss ) a copy is provided for comparison.

Taken from SNDH Atari ST YM2149 Collection website https://sndh.atari.org

The SNDH file format contains code to play itself and needs to be activated, I have not decompiled this just copied the relevant block of data into a .bin file.

The image data used ( intelek.pic, picture1.pic, title.pic) are a non compressed type which is copied exactly as it is to the screen and provides no palette data.

This is my first full decompilation and was done using a combination of Ghidra and Fred's dissasembler ( https://atari-forum.com/viewtopic.php?t=14540 )

The code is assembled using VASM\VBCC ( http://www.compilers.de/vasm.html ) with the following commands :-

C:\STFM\VCC\vbcc\bin\vasmm68k_mot decomp.asm -m68000 -Ftos -devpac -o C:\STFM\HD\ITALIA\recomp.tos
