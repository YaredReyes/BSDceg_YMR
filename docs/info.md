<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

 It is a BCD to 7-segment display decoder. It converts a 4-bit binary number, set with switches, into the matching decimal digit on the display.

## How to test

Setup

Wire the decoder between INPUT and OUTPUT as in the diagram, and remove the old direct wires.
Set all 8 DIP switches to OFF.
Press the green play button to start the simulation.

## External hardware

Then my guess was right: it is Wokwi's digital editor, with Tiny Tapeout-style INPUT and OUTPUT blocks. That changes one important thing: in Wokwi you have to build the decoder yourself out of gates, because the block between INPUT and OUTPUT can't be imported as an image.

Delete the 8 direct wires between INPUT and OUTPUT.
Add NOT, AND and OR gates from the parts menu (the + button).
Build the 7 functions below, one per segment.
Connect IN0 to IN3 to the inputs and the outputs a-g to OUT0 to OUT6, as in the diagram.
Connect OUT7 to ground and leave IN4 to IN7 unused.
