These programs were written by Jim Dunion, Erann Gat (who now goes by Ron Garret), and Hal Gilliam, under the auspices of the American Museum of Science & Energy in Oak Ridge, Tennessee.  The programs were the interactive component of The Energy Arcade, a traveling museum exhibit, which appeared at the Center of Science and Industry (COSI) in Columbus, Ohio between October 1980 and May 1981.

The programs are:
  - Driving for Dollars
  - Conservation Hangman
  - Energy Hangman
  - Energy Arcade
  - Energy Quiz

Conservation Hangman is credited to Jim Dunion and Erann Gat, 21-Dec-1979.  Energy Hangman is credited to Jim Dunion, Erann Gat, and Hal Gilliam, 21-Nov-1980.  The other programs lack specific credit or identifying dates.  Energy Quiz appears to be an earlier version of Energy Arcade, mentioning "through October of last year" vs "through February of this year".  Additionally, Energy Arcade has a few extra POKE commands to fully control an external lamp driver.

The target platform was the Commodore PET with 16K of RAM and upgrade ROMs (Conservation Hangman will work with original ROMs as well).  The programs were loaded daily from tape and ran completely from RAM once loaded; no disk drive was required.  An external amplified speaker was attached to the CB2 pin on the User Port to play sound effects and music.

Part of the physical installation was a bank of "marquee lights" implemented as 8 strings of small 110VAC incandescent bulbs interleaved such that the first bulb was wired to the ninth bulb, the second bulb to the tenth bulb, etc., up, over, and around a niche containing two of the PET computers.  One of them had a driver board with eight TRIACs connected to the User Port.  Under program control, the byte written to the User Port would control which bulbs were on and off, allowing for chase light effects.  Inspection of the code shows that while there are User Port POKE commands in Energy Quiz, the port address isn't given so the program just writes values to memory location 0 (which is harmless on the PET).  Energy Arcade has the same POKE commands as Energy Quiz plus a few more, and _does_ define the address of the User Port.

Owing to the method of backing up these programs up in 1980, four of the five programs are complete, but Energy Hangman was not fully saved.  The BASIC code is intact, but the machine language routines to draw and animate shapes were lost.  Efforts to reconstruct the missing shapes and animate them with the subroutines from Driving for Dollars are underway.
