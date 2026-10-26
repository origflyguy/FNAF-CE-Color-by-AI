==============================================================
   FNAF CE COLOR  -  for the TI-84 Plus CE
==============================================================
A full-color port of the first Five Nights at Freddy's for the
TI-84 Plus CE, written in C. All five nights, the 6th night and
the custom night, with the original game's AI rules, color
cameras, jumpscares and endings.

***This game was with a lot of help by AI but the game was still tested and checked against the real game for as close to 100% of the mechanics of the Original FNAF 1 by a human*** 
*a lot more work went into it then just a prompt*

Version: 1.0
Author:  Origflyguy

--------------------------------------------------------------
REQUIREMENTS
--------------------------------------------------------------
- TI-84 Plus CE (tested on real hardware)
- About 740 KB free archive memory
- The CE C libraries (clibs.8xg). Get the latest from
  https://github.com/CE-Programming/libraries/releases
- OS 5.5 or newer: you need arTIfiCE to run assembly/C programs
  (https://yvantt.github.io/arTIfiCE/). On OS 5.4 or older,
  Asm(prgmFNAFCE) works directly.

--------------------------------------------------------------
INSTALLING
--------------------------------------------------------------
1. Send clibs.8xg to the calculator (skip this if you already
   have it).
2. Send FNAFCE.8xp and ALL 18 appvars (.8xv) with TI Connect CE.
   Put the appvars in ARCHIVE (they are already marked archived).
3. Run FNAFCE (through arTIfiCE on OS 5.5+).

If an appvar is missing, the game tells you which one.

The 18 appvars:
  FNAFVAR2                        font, text, map
  FNAFVAR4 FNAFVAR5 FNAFVAR6 FNAFVAR7   cameras
  FNAFVAR9                        office
  FNAFSC1 - FNAFSC6               jumpscares, game over
  FNAFSC8                         newspaper
  FNAFSC9                         custom night icons
  FNAFSC10                        title screen
  FNAFSC11 FNAFSC12 FNAFSC13      endings

Updating from a test version? Delete FNAFVAR1, FNAFVAR3,
FNAFVAR8 and FNAFSC7: they are no longer used.

--------------------------------------------------------------
CONTROLS
--------------------------------------------------------------
In the office
  Left / Right    look around
  alpha           light (only at the far left or far right)
  2nd             door  (only at the far left or far right)
  Up              raise the monitor

On the cameras
  )  1A Show Stage       2  2B West Hall Corner
  (  1B Dining Area      4  3  Supply Closet
  7  1C Pirate Cove      6  4A East Hall
  5  2A West Hall        3  4B East Hall Corner
  ,  5  Backstage        *  7  Restrooms
  -  6  Kitchen (audio only)
  Down            lower the monitor

During a night
  mode            WHERE IS EVERYONE? (pauses the night)
  graph           skip to the next night
  clear           quit (works on any screen)

Title screen
  Up / Down, enter   New Game, Continue, 6th Night, Custom Night
  trace           switch pace: FAST <-> NORMAL (saved)
  graph           choose the night Continue starts at
  stat            statistics (deaths by each animatronic)
  y= / mode       tutorial
  zoom            list of all the buttons

--------------------------------------------------------------
TWO PACES
--------------------------------------------------------------
NORMAL  The original game: 8:55 nights (89 s per hour), the
        original AI intervals, levels and timers. Foxy runs
        for 25 s after leaving the cove, and gets to you about
        1.7 s after you see him in 2A.
FAST    (default) A 4:00 night, quicker Bonnie and Chica,
        +1 AI level. Foxy runs for 12 s, and 4 s once seen.

--------------------------------------------------------------
HOW IT PLAYS (the original's rules)
--------------------------------------------------------------
- Bonnie comes to the LEFT door, Chica to the RIGHT. Check with
  the lights: you will see them in the doorway.
- If a door is open when they try to get in, they get IN: that
  side's door and light stop working, and they get you the
  next time the monitor goes down.
- Foxy can't move while the monitor is up. Wait too long between
  looks and he leaves Pirate Cove for the left door. A shut door
  stops him but costs power (1%, then 6%, 11%, ...).
- Freddy only moves while the monitor is down. Watching his
  camera holds him. At 4B, watching 4B keeps him out of the
  office (camera stalling).
- No sound on a calculator, so sound cues show as text:
  "* Freddy laughs *" and "* footsteps *".
- Run out of power and Freddy comes for you. Make it to 6 AM
  first and you survive.

--------------------------------------------------------------
NOT INCLUDED
--------------------------------------------------------------
- Sound (the calculator has no speaker)
- Golden Freddy and the rare random camera images

--------------------------------------------------------------
CREDITS
--------------------------------------------------------------
- Five Nights at Freddy's by Scott Cawthon. All characters,
  pictures and story belong to him.
- Original FNAF textures collected by The2AndOnly
  ("Fnaf 1 Textures Organized").
- Based on the TI-83+/84+ Axe FNAF by Haobo.
- Built with the CE C/C++ Toolchain (CE-Programming).

This is a free, non-commercial fan game, not affiliated with
Scott Cawthon or Scottgames. Do not sell it.
