# Scott Adams Dat File Breakdowns

This repository contains:
1. A collection of detailed, human readable versions of the first thirteen Scott Adams Adventure Game files.
2. Transformed and decoded versions of the Hint Sheets for Scott Adam's Grand Adventuresl, which can be found on the [donwloads page for Scott Adam's own website](https://www.msadams.com/downloads.htm).
3. Game maps PNG generated from DAT files
4. Game map DOT file - a file containing a [GraphViz](https://graphviz.org) definition for the map file.

## Game Maps
These show the room connections (e.g. NORTH, SOUTH etc), and some user inputs which can cause movement between rooms (e.g. GO HOLE). Not all use inputs are shown due to the way game actions are constructed, e.g. in Pyramid of Doom a player can only move between rooms if a ladder is present - the associated action checks to see if the ladder is in the room with the player, and is placed in the room by an unrelated action. I can see no way of getting round this.

Notes:
* A solid gray border is the starter room
* A thick blue border is the treasure room
