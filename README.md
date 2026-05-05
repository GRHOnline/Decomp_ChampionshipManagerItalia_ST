# Decomp_ChampionshipManagerItalia_ST
An assembler decompilation of the Atari ST game Championship Manager Italia. This is the hard drive install of the game and not the floppy disk based version.

The program contains a sndh file within it which is the same as the one used by Championship Manager 93 ( written by Matt Furniss ) a copy is provided for comparison.
Taken from SNDH Atari ST YM2149 Collection website https://sndh.atari.org
The SNDH file format contains code to play itself and needs to be activated, I have not decompiled this just copied the relevant block of data into a .bin file.

The image data used ( intelek.pic, picture1.pic, title.pic) are a non compressed type which is copied exactly as it is to the screen and provides no palette data.
