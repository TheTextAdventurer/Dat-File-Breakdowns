# Secret Mission DatFile
*Table of Contents*
-[Header](#Header)
-[Actions](#Actions)
-[Verbs](#Verbs)
-[Nouns](#Nouns)
-[Rooms](#Rooms)
-[Messages](#Messages)
-[Items](#Items)
## Header
| Property| Value |
| --------| ----- |
| adventureNumber| 3 |
| Unknown| 5963 |
| numItems| 54 |
| numActions| 162 |
| numNounVerbs| 65 |
| numRooms| 24 |
| maxCarry| 7 |
| startRoom| 2 |
| totalTreasures| 0 |
| wordLength| 3 |
| lightDuration| 10000 |
| numMessages| 82 |
| treasureRoom| 1 |
## Actions
### Action 0 - WIRE CUT BOOM SOON - Probability: 15 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15, 594, 180, 0, 0, 0, 8850, 0|  |
| Probability| 15%|  |
| Condition| ConditionID 13 ArgID 29| item 'Red wire going from bomb into wall(index:29)' not in game |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
### Action 1 - BOOOM SOON - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 194, 206, 40, 200, 0, 8853, 674|  |
| Probability| 100%|  |
| Condition| ConditionID 13 ArgID 9| item 'Surgically implanted bomb detector glows green \(bomb's \-safe\-\)(index:9)' not in game |
| Condition| ConditionID 5 ArgID 10| item 'Bomb detector glowing red \(final countdown active\)(index:10)' not carried |
| Action| ActionID 59 ArgID 2| Item 'Bomb detector flashing yellow (bomb is now armed)(index:2)' is removed from the game (put in room 0) |
| Action| ActionID 3 | Print message 'My bomb detector' |
| Action| ActionID 4 | Print message 'wails ALARMINGLY\!' |
| Action| ActionID 74 ArgID 10| take item 'Bomb detector glowing red (final countdown active)(index:10)', no check done to see if can carry |
### Action 2 - STEAL TAPE PLAYER - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 72, 854, 60, 77, 0, 8850, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 11 ArgID 3| item 'Large tape recorder(index:3)' not carried or in room with player |
| Condition| ConditionID 13 ArgID 42| item 'Dead saboteur(index:42)' not in game |
| Condition| ConditionID 16 ArgID 3| object 'Large tape recorder(index:3)' in initial location |
| Action| ActionID 59 ArgID 3| Item 'Large tape recorder(index:3)' is removed from the game (put in room 0) |
### Action 3 - DEC COUNTER - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 0, 0, 0, 0, 0, 11550, 0|  |
| Probability| 100%|  |
| Action| ActionID 77 | decrement current counter |
### Action 4 - BOOOM - Probability: 9 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9, 201, 0, 0, 0, 0, 10566, 1863|  |
| Probability| 9%|  |
| Condition| ConditionID 0 ArgID 10| item 'Bomb detector glowing red \(final countdown active\)(index:10)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 66 | output inventory |
| Action| ActionID 12 | Print message '\*   B O O O O O O O O O M \! \* \* \* \* \* \*' |
| Action| ActionID 63 | game over |
### Action 5 - MSG DOOM - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 815, 16, 206, 0, 0, 18528, 18600|  |
| Probability| 100%|  |
| Condition| ConditionID 14 ArgID 40| current counter less than 40 |
| Condition| ConditionID 15 ArgID 0| current counter greater than '0' |
| Condition| ConditionID 5 ArgID 10| item 'Bomb detector glowing red \(final countdown active\)(index:10)' not carried |
| Action| ActionID 123 | Print message 'Final countdown starts in' |
| Action| ActionID 78 | output current counter |
| Action| ActionID 124 | Print message 'turns\!' |
### Action 6 - FIRST IN - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 249, 240, 6000, 0, 0, 5218, 8779|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 12| bitflag 12 is false |
| Action| ActionID 34 | Print message 'Welcome to Adventure number 3 `MISSION IMPOSSIBLE` by Scott Adams, Dedicated to Maegen Adams\. ' |
| Action| ActionID 118 | Print message 'A minute ago someone ran out of this room\! By the way I seem to be carrying something\! ' |
| Action| ActionID 58 ArgID 12| set 12 flag |
| Action| ActionID 79 ArgID 300| set current counter value 300 |
### Action 7 - SABETOUR - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 854, 207, 840, 200, 5515, 9350, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 13 ArgID 42| item 'Dead saboteur(index:42)' not in game |
| Condition| ConditionID 6 ArgID 10| player not in room 10 |
| Condition| ConditionID 14 ArgID 275| current counter less than 275 |
| Action| ActionID 62 ArgID 42, 10| item 'Dead saboteur(index:42)' is moved to room 10 |
| Action| ActionID 50 | Print message 'In the distance you hear a dull thud; as if someone fell or dropped something heavy\.' |
### Action 8 - SABETOUR - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 854, 87, 840, 80, 5515, 9350, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 13 ArgID 42| item 'Dead saboteur(index:42)' not in game |
| Condition| ConditionID 6 ArgID 4| player not in room 4 |
| Condition| ConditionID 14 ArgID 275| current counter less than 275 |
| Action| ActionID 62 ArgID 42, 4| item 'Dead saboteur(index:42)' is moved to room 4 |
| Action| ActionID 50 | Print message 'In the distance you hear a dull thud; as if someone fell or dropped something heavy\.' |
### Action 9 - SABETOUR - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 854, 67, 840, 60, 5515, 9350, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 13 ArgID 42| item 'Dead saboteur(index:42)' not in game |
| Condition| ConditionID 6 ArgID 3| player not in room 3 |
| Condition| ConditionID 14 ArgID 275| current counter less than 275 |
| Action| ActionID 62 ArgID 42, 3| item 'Dead saboteur(index:42)' is moved to room 3 |
| Action| ActionID 50 | Print message 'In the distance you hear a dull thud; as if someone fell or dropped something heavy\.' |
### Action 10 - VOICE - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 204, 0, 0, 0, 0, 2719, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 11 - RAN IN AND LEFT - Probability: 15 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15, 854, 0, 0, 0, 0, 17850, 0|  |
| Probability| 15%|  |
| Condition| ConditionID 13 ArgID 42| item 'Dead saboteur(index:42)' not in game |
| Action| ActionID 119 | Print message 'Someone came in the room, he saw me and ran out\!' |
### Action 12 - SHOW AUTHORIZATION - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 184, 0, 0, 0, 0, 2719, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 13 - SHOW AUTHORIZATION - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 224, 0, 0, 0, 0, 2719, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 14 - TV - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 264, 268, 0, 0, 0, 16800, 0|  |
| Probability| 80%|  |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 112 | Print message 'TV camera is slow scanning the window area\.' |
### Action 15 - TV - Probability: 40 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 40, 264, 269, 0, 0, 0, 16950, 0|  |
| Probability| 40%|  |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 113 | Print message 'TV camera is powered down\. ' |
### Action 16 - ALREADY SET DETECTOR - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 181, 20, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 0 ArgID 9| item 'Surgically implanted bomb detector glows green \(bomb's \-safe\-\)(index:9)' carried |
| Action| ActionID 60 ArgID 1| set 1 flag |
### Action 17 - DITTO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 48, 41, 40, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Condition| ConditionID 0 ArgID 2| item 'Bomb detector flashing yellow \(bomb is now armed\)(index:2)' carried |
| Action| ActionID 60 ArgID 2| set 2 flag |
### Action 18 - SET GREEN - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 180, 193, 40, 20, 522, 2160|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 12 ArgID 9| item 'Surgically implanted bomb detector glows green \(bomb's \-safe\-\)(index:9)' in game |
| Action| ActionID 3 | Print message 'My bomb detector' |
| Action| ActionID 72 ArgID 9, 2| swap item locations 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' and 'Bomb detector flashing yellow (bomb is now armed)(index:2)' |
| Action| ActionID 14 | Print message 'politely beeps\.\.\. ' |
| Action| ActionID 60 ArgID 1| set 1 flag |
### Action 19 - SET YELLO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 48, 193, 180, 40, 40, 522, 2310|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Condition| ConditionID 12 ArgID 9| item 'Surgically implanted bomb detector glows green \(bomb's \-safe\-\)(index:9)' in game |
| Action| ActionID 3 | Print message 'My bomb detector' |
| Action| ActionID 72 ArgID 9, 2| swap item locations 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' and 'Bomb detector flashing yellow (bomb is now armed)(index:2)' |
| Action| ActionID 15 | Print message 'angrily buzzes\.\.\. ' |
| Action| ActionID 60 ArgID 2| set 2 flag |
### Action 20 - PAIL - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 424, 481, 480, 600, 0, 10831, 7050|  |
| Probability| 80%|  |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 0 ArgID 24| item 'Water filled plastic pail(index:24)' carried |
| Action| ActionID 72 ArgID 24, 30| swap item locations 'Water filled plastic pail(index:24)' and 'Strange lump of glowing plastic(index:30)' |
| Action| ActionID 31 | Print message 'The radiation did something to my pail\!' |
| Action| ActionID 47 | Print message 'the water soaks into the floor' |
### Action 21 - NO SUIT - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 424, 541, 0, 0, 0, 4833, 9450|  |
| Probability| 80%|  |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 0 ArgID 27| item 'Anti\-radiation suit(index:27)' carried |
| Action| ActionID 32 | Print message 'Holding a Radiation Suit' |
| Action| ActionID 33 | Print message 'doesn't provide much protection for me as I fall down retching I hear/FEEL THE BOMB explode\! ' |
| Action| ActionID 63 | game over |
### Action 22 - NO SUIT - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 424, 553, 0, 0, 0, 5283, 9450|  |
| Probability| 80%|  |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 12 ArgID 27| item 'Anti\-radiation suit(index:27)' in game |
| Action| ActionID 35 | Print message 'A business suit' |
| Action| ActionID 33 | Print message 'doesn't provide much protection for me as I fall down retching I hear/FEEL THE BOMB explode\! ' |
| Action| ActionID 63 | game over |
### Action 23 - BOMB TRIGGED - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 15, 180, 0, 0, 0, 8850, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
### Action 24 - . - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 25 - NEED SAB TOO - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 264, 852, 823, 268, 0, 2720, 18150|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 11 ArgID 42| item 'Dead saboteur(index:42)' not carried or in room with player |
| Condition| ConditionID 2 ArgID 41| item 'Picture of saboteur stamped \-window maintance\-(index:41)' carried or in room with player |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 20 | Print message '`Authorization INSUFFICIENT for access` ' |
| Action| ActionID 121 | Print message '`Owner of badge is not present\!`' |
### Action 26 - . - Input: REA LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3652, 983, 0, 0, 0, 0, 10622, 0|  |
| Verb| 24| REA |
| Noun| 52| LEA |
| Condition| ConditionID 2 ArgID 49| item 'A leaflet(index:49)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 122 | Print message 'Hi\! Look for Adventure number 4: `VOODOO CASTLE` at your favorite computer store\! \(Now back to our current program\.\)' |
### Action 27 - . - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 28 - . - Input: FRI MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8142, 323, 234, 220, 0, 0, 8001, 0|  |
| Verb| 54| FRI |
| Noun| 42| MOP |
| Condition| ConditionID 2 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried or in room with player |
| Condition| ConditionID 13 ArgID 11| item 'Blue key(index:11)' not in game |
| Action| ActionID 53 ArgID 11| drops item 'Blue key(index:11)' into current room |
| Action| ActionID 51 | Print message 'Something fell to the floor\.' |
### Action 29 - . - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 30 - . - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6470, 307, 0, 0, 0, 0, 907, 2550|  |
| Verb| 43| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 6 ArgID 15| player not in room 15 |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 7 | Print message 'It appears locked' |
| Action| ActionID 17 | Print message 'Most doors & windows are under automated security control\.' |
### Action 31 - GIVE BADGES - Input: PRE WHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3760, 186, 122, 20, 20, 0, 8754, 10955|  |
| Verb| 25| PRE |
| Noun| 10| WHI |
| Condition| ConditionID 5 ArgID 9| item 'Surgically implanted bomb detector glows green \(bomb's \-safe\-\)(index:9)' not carried |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 54 ArgID 1| move room 1 |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 5 | Print message 'CLICK\!' |
### Action 32 - SECURITY BADGE - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 22, 20, 80, 100, 0, 9354, 1650|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' in room with player |
| Action| ActionID 62 ArgID 1, 4| item 'Picture of me stamped -security-(index:1)' is moved to room 4 |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 11 | Print message 'There's a Bright flash & I hear something fall to the floor\. I can't see what it is from here though\. ' |
### Action 33 - MAINTANCE BADGE - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 162, 160, 80, 100, 0, 9354, 1650|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' in room with player |
| Action| ActionID 62 ArgID 8, 4| item 'Picture of me stamped -maintenance-(index:8)' is moved to room 4 |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 11 | Print message 'There's a Bright flash & I hear something fall to the floor\. I can't see what it is from here though\. ' |
### Action 34 - VISITOR BADGE - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 142, 140, 80, 100, 0, 9354, 1650|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 7| item 'Picture of me stamped: \-visitor\-(index:7)' in room with player |
| Action| ActionID 62 ArgID 7, 4| item 'Picture of me stamped: -visitor-(index:7)' is moved to room 4 |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 11 | Print message 'There's a Bright flash & I hear something fall to the floor\. I can't see what it is from here though\. ' |
### Action 35 - NO PIC - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 24, 100, 0, 0, 0, 8102, 2400|  |
| Probability| 0%|  |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 2 | Print message 'Nothing happened' |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
### Action 36 - Input: CLE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1950, 323, 233, 0, 0, 0, 17552, 0|  |
| Verb| 13| CLE |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried or in room with player |
| Condition| ConditionID 12 ArgID 11| item 'Blue key(index:11)' in game |
| Action| ActionID 117 | Print message 'HUH?' |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 37 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4800, 324, 180, 0, 0, 0, 15612, 9450|  |
| Verb| 32| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Action| ActionID 104 | Print message 'Oh Boy\.\.\.I think I did something\.\.\.' |
| Action| ActionID 12 | Print message '\*   B O O O O O O O O O M \! \* \* \* \* \* \*' |
| Action| ActionID 63 | game over |
### Action 38 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 39 - Input: LOO MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6042, 323, 234, 0, 0, 0, 15750, 0|  |
| Verb| 40| LOO |
| Noun| 42| MOP |
| Condition| ConditionID 2 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried or in room with player |
| Condition| ConditionID 13 ArgID 11| item 'Blue key(index:11)' not in game |
| Action| ActionID 105 | Print message 'It made an odd sound\.' |
### Action 40 - DANGER - Input: PRE RED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3759, 122, 40, 46, 0, 0, 8705, 0|  |
| Verb| 25| PRE |
| Noun| 9| RED |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 5 ArgID 2| item 'Bomb detector flashing yellow \(bomb is now armed\)(index:2)' not carried |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 5 | Print message 'CLICK\!' |
### Action 41 - . - Input: UNL BUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5569, 0, 0, 0, 0, 0, 7200, 0|  |
| Verb| 37| UNL |
| Noun| 19| BUT |
| Action| ActionID 48 | Print message 'say again & use a color\!' |
### Action 42 - LOCKED - Input: PRE BLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3761, 89, 122, 0, 0, 0, 907, 0|  |
| Verb| 25| PRE |
| Noun| 11| BLU |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 7 | Print message 'It appears locked' |
### Action 43 - LOCKED - Input: PRE YEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3762, 69, 122, 0, 0, 0, 907, 0|  |
| Verb| 25| PRE |
| Noun| 12| YEL |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 7 | Print message 'It appears locked' |
### Action 44 - MOVE PICTURE - Input: PRE BLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3761, 122, 34, 20, 20, 0, 9305, 0|  |
| Verb| 25| PRE |
| Noun| 11| BLU |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 13 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' not in game |
| Action| ActionID 62 ArgID 1, 1| item 'Picture of me stamped -security-(index:1)' is moved to room 1 |
| Action| ActionID 5 | Print message 'CLICK\!' |
### Action 45 - Input: PRE BUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3769, 0, 0, 0, 0, 0, 7200, 0|  |
| Verb| 25| PRE |
| Noun| 19| BUT |
| Action| ActionID 48 | Print message 'say again & use a color\!' |
### Action 46 - MOVE PIC - Input: PRE YEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3762, 122, 174, 160, 20, 0, 9305, 0|  |
| Verb| 25| PRE |
| Noun| 12| YEL |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 13 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' not in game |
| Action| ActionID 62 ArgID 8, 1| item 'Picture of me stamped -maintenance-(index:8)' is moved to room 1 |
| Action| ActionID 5 | Print message 'CLICK\!' |
### Action 47 - CLICK? - Input: PRE RED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3759, 122, 180, 41, 0, 0, 809, 0|  |
| Verb| 25| PRE |
| Noun| 9| RED |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 0 ArgID 2| item 'Bomb detector flashing yellow \(bomb is now armed\)(index:2)' carried |
| Action| ActionID 5 | Print message 'CLICK\!' |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
### Action 48 - . - Input: PRE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 122, 0, 0, 0, 0, 750, 0|  |
| Verb| 25| PRE |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Action| ActionID 5 | Print message 'CLICK\!' |
### Action 49 - STAND UP - Input: ACT UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8555, 104, 80, 0, 0, 0, 8170, 9600|  |
| Verb| 57| ACT |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 54 ArgID 4| move room 4 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 50 - TAPE - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 63, 60, 0, 0, 0, 7800, 0|  |
| Verb| 10| GET |
| Noun| 7| TAP |
| Condition| ConditionID 2 ArgID 3| item 'Large tape recorder(index:3)' carried or in room with player |
| Action| ActionID 52 ArgID 3| get item 'Large tape recorder(index:3)', check if can carry |
### Action 51 - STAND UP - Input: GET UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1505, 104, 80, 0, 0, 0, 8170, 9600|  |
| Verb| 10| GET |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 54 ArgID 4| move room 4 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 52 - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 750, 553, 0, 0, 0, 0, 10566, 0|  |
| Verb| 5| INV |
| Noun| 0| ANY |
| Condition| ConditionID 12 ArgID 27| item 'Anti\-radiation suit(index:27)' in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 66 | output inventory |
### Action 53 - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 750, 554, 0, 0, 0, 0, 10566, 5400|  |
| Verb| 5| INV |
| Noun| 0| ANY |
| Condition| ConditionID 13 ArgID 27| item 'Anti\-radiation suit(index:27)' not in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 66 | output inventory |
| Action| ActionID 36 | Print message 'I'm WEARING an anti\-radiation suit\.' |
### Action 54 - Input: LOO TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6007, 63, 0, 0, 0, 0, 16350, 0|  |
| Verb| 40| LOO |
| Noun| 7| TAP |
| Condition| ConditionID 2 ArgID 3| item 'Large tape recorder(index:3)' carried or in room with player |
| Action| ActionID 109 | Print message 'Try starting it\.' |
### Action 55 - Input: SAV GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7363, 0, 0, 0, 0, 0, 10650, 0|  |
| Verb| 49| SAV |
| Noun| 13| GAM |
| Action| ActionID 71 | save game |
### Action 56 - Input: QUI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7500, 0, 0, 0, 0, 0, 1863, 0|  |
| Verb| 50| QUI |
| Noun| 0| ANY |
| Action| ActionID 12 | Print message '\*   B O O O O O O O O O M \! \* \* \* \* \* \*' |
| Action| ActionID 63 | game over |
### Action 57 - Input: LOO SAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6039, 843, 0, 0, 0, 0, 17510, 0|  |
| Verb| 40| LOO |
| Noun| 39| SAB |
| Condition| ConditionID 2 ArgID 42| item 'Dead saboteur(index:42)' carried or in room with player |
| Action| ActionID 116 | Print message 'I see nothing special\.' |
| Action| ActionID 110 | Print message 'Maybe I should FRISK him?' |
### Action 58 - MOVIE - Input: PRE GRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3796, 302, 413, 0, 0, 0, 4066, 4229|  |
| Verb| 25| PRE |
| Noun| 46| GRE |
| Condition| ConditionID 1 ArgID 15| item 'Panel of buttons \-white green\-(index:15)' in room with player |
| Condition| ConditionID 12 ArgID 20| item 'Empty movie projector(index:20)' in game |
| Action| ActionID 27 | Print message 'Click\! Room lights dim and a screen drops from the ceiling\. You hear a hidden projector start\.' |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 28 | Print message 'The screen illuminates for awhile, but no movie\!?' |
| Action| ActionID 29 | Print message 'The projector stops, the screen rises, and the lights return\.' |
### Action 59 - MOVIE - Input: PRE GRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3796, 302, 414, 0, 0, 0, 10527, 4529|  |
| Verb| 25| PRE |
| Noun| 46| GRE |
| Condition| ConditionID 1 ArgID 15| item 'Panel of buttons \-white green\-(index:15)' in room with player |
| Condition| ConditionID 13 ArgID 20| item 'Empty movie projector(index:20)' not in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 27 | Print message 'Click\! Room lights dim and a screen drops from the ceiling\. You hear a hidden projector start\.' |
| Action| ActionID 30 | Print message 'A movie runs telling about the reactor and its construction interesting highlights: 1\) Plastic DEFORMS strangely in radiation 2\) Even short exposure to HIGH radiation is LETHAL, so suit up ' |
| Action| ActionID 29 | Print message 'The projector stops, the screen rises, and the lights return\.' |
### Action 60 - Input: ACT TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8557, 63, 0, 0, 0, 0, 10501, 1950|  |
| Verb| 57| ACT |
| Noun| 7| TAP |
| Condition| ConditionID 2 ArgID 3| item 'Large tape recorder(index:3)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 1 | Print message 'Good morning Mr\. Phelps\. Your Mission \(should you decide to accept it\) is to prevent this automated nuclear reactor from being destroyed by a saboteur's TIME BOMB\! ' |
| Action| ActionID 13 | Print message 'The saboteur \(who also rewired the security system\) is a heart patient\. He plans to SUICIDE with the reactor\! He is still loosein the building\. You'll find Security keys & a map in the manila envelope lying next to the tape player\.' |
### Action 61 - Input: UNL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5550, 122, 223, 80, 89, 0, 8709, 1200|  |
| Verb| 37| UNL |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 2 ArgID 11| item 'Blue key(index:11)' carried or in room with player |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 58 ArgID 4| set 4 flag |
| Action| ActionID 9 | Print message 'Blue' |
| Action| ActionID 8 | Print message 'button is now unlocked' |
### Action 62 - UNLOCK - Input: UNL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5550, 122, 243, 60, 69, 0, 8710, 1200|  |
| Verb| 37| UNL |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 6| item 'Row of 4 buttons \-red white blue yellow\-(index:6)' in room with player |
| Condition| ConditionID 2 ArgID 12| item 'Yellow key(index:12)' carried or in room with player |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 58 ArgID 3| set 3 flag |
| Action| ActionID 10 | Print message 'Yellow' |
| Action| ActionID 8 | Print message 'button is now unlocked' |
### Action 63 - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1547, 553, 0, 0, 0, 0, 10566, 0|  |
| Verb| 10| GET |
| Noun| 47| INV |
| Condition| ConditionID 12 ArgID 27| item 'Anti\-radiation suit(index:27)' in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 66 | output inventory |
### Action 64 - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1547, 554, 0, 0, 0, 0, 10566, 5400|  |
| Verb| 10| GET |
| Noun| 47| INV |
| Condition| ConditionID 13 ArgID 27| item 'Anti\-radiation suit(index:27)' not in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 66 | output inventory |
| Action| ActionID 36 | Print message 'I'm WEARING an anti\-radiation suit\.' |
### Action 65 - Input: PRE WHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3760, 264, 180, 0, 0, 0, 804, 3150|  |
| Verb| 25| PRE |
| Noun| 10| WHI |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Action| ActionID 5 | Print message 'CLICK\!' |
| Action| ActionID 54 ArgID 9| move room 9 |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
### Action 66 - Input: PRE YEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3762, 284, 200, 0, 0, 0, 10505, 3204|  |
| Verb| 25| PRE |
| Noun| 12| YEL |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 5 | Print message 'CLICK\!' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 10| move room 10 |
### Action 67 - BOOM SOON - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 171, 342, 268, 180, 320, 0, 8904, 10564|  |
| Verb| 1| GO |
| Noun| 21| WIN |
| Condition| ConditionID 1 ArgID 17| item 'Empty window frame(index:17)' in room with player |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 68 - THRU WINDOW SAFE - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 171, 342, 269, 320, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 21| WIN |
| Condition| ConditionID 1 ArgID 17| item 'Empty window frame(index:17)' in room with player |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 69 - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 171, 324, 260, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 21| WIN |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Action| ActionID 54 ArgID 13| move room 13 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 70 - Input: PRE BLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3761, 304, 220, 0, 0, 0, 10505, 3204|  |
| Verb| 25| PRE |
| Noun| 11| BLU |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 5 | Print message 'CLICK\!' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 11| move room 11 |
### Action 71 - Input: LOA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4350, 443, 403, 400, 420, 440, 10859, 10564|  |
| Verb| 29| LOA |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 22| item 'Movie film cartridge(index:22)' carried or in room with player |
| Condition| ConditionID 2 ArgID 20| item 'Empty movie projector(index:20)' carried or in room with player |
| Action| ActionID 72 ArgID 20, 21| swap item locations 'Empty movie projector(index:20)' and 'Movie projector with film cartridge(index:21)' |
| Action| ActionID 59 ArgID 22| Item 'Movie film cartridge(index:22)' is removed from the game (put in room 0) |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 72 - UNLOAD MOVIE - Input: UNL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5550, 423, 440, 420, 400, 0, 7872, 10564|  |
| Verb| 37| UNL |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 21| item 'Movie projector with film cartridge(index:21)' carried or in room with player |
| Action| ActionID 52 ArgID 22| get item 'Movie film cartridge(index:22)', check if can carry |
| Action| ActionID 72 ArgID 21, 20| swap item locations 'Movie projector with film cartridge(index:21)' and 'Empty movie projector(index:20)' |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 73 - Input: BRE BOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6779, 563, 160, 0, 0, 0, 3658, 0|  |
| Verb| 45| BRE |
| Noun| 29| BOM |
| Condition| ConditionID 2 ArgID 28| item 'Very large time bomb(index:28)' carried or in room with player |
| Action| ActionID 24 | Print message 'Tell me with what? Example: `WITH FIST`' |
| Action| ActionID 58 ArgID 8| set 8 flag |
### Action 74 - END IS NEAR - Input: WIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 168, 160, 180, 563, 0, 9105, 8954|  |
| Verb| 15| WIT |
| Noun| 0| ANY |
| Condition| ConditionID 7 ArgID 8| bitflag 8 is set |
| Condition| ConditionID 2 ArgID 28| item 'Very large time bomb(index:28)' carried or in room with player |
| Action| ActionID 60 ArgID 8| set 8 flag |
| Action| ActionID 105 | Print message 'It made an odd sound\.' |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
| Action| ActionID 104 | Print message 'Oh Boy\.\.\.I think I did something\.\.\.' |
### Action 75 - Input: GET BOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1529, 562, 594, 560, 0, 0, 7800, 0|  |
| Verb| 10| GET |
| Noun| 29| BOM |
| Condition| ConditionID 1 ArgID 28| item 'Very large time bomb(index:28)' in room with player |
| Condition| ConditionID 13 ArgID 29| item 'Red wire going from bomb into wall(index:29)' not in game |
| Action| ActionID 52 ArgID 28| get item 'Very large time bomb(index:28)', check if can carry |
### Action 76 - Input: CHA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3300, 0, 0, 0, 0, 0, 18000, 0|  |
| Verb| 22| CHA |
| Noun| 0| ANY |
| Action| ActionID 120 | Print message 'I see no one here\.' |
### Action 77 - Input: GET BOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1529, 562, 874, 0, 0, 0, 6, 15450|  |
| Verb| 10| GET |
| Noun| 29| BOM |
| Condition| ConditionID 1 ArgID 28| item 'Very large time bomb(index:28)' in room with player |
| Condition| ConditionID 13 ArgID 43| item 'Loose red wire going into wall(index:43)' not in game |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 103 | Print message 'its still connected' |
### Action 78 - BOOM NEAR - Input: DRO BOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2729, 561, 180, 560, 0, 0, 15809, 15653|  |
| Verb| 18| DRO |
| Noun| 29| BOM |
| Condition| ConditionID 0 ArgID 28| item 'Very large time bomb(index:28)' carried |
| Action| ActionID 105 | Print message 'It made an odd sound\.' |
| Action| ActionID 59 ArgID 9| Item 'Surgically implanted bomb detector glows green (bomb's -safe-)(index:9)' is removed from the game (put in room 0) |
| Action| ActionID 104 | Print message 'Oh Boy\.\.\.I think I did something\.\.\.' |
| Action| ActionID 53 ArgID 28| drops item 'Very large time bomb(index:28)' into current room |
### Action 79 - Input: POU ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 384, 483, 563, 0, 0, 10544, 6813|  |
| Verb| 6| POU |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Condition| ConditionID 2 ArgID 24| item 'Water filled plastic pail(index:24)' carried or in room with player |
| Condition| ConditionID 2 ArgID 28| item 'Very large time bomb(index:28)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 44 | Print message 'the water spills on the bomb and' |
| Action| ActionID 45 | Print message 'the control panel which immediately shorts out triggering the bomb' |
| Action| ActionID 63 | game over |
### Action 80 - WON!!! - Input: POU ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 404, 483, 563, 0, 0, 6646, 9450|  |
| Verb| 6| POU |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 2 ArgID 24| item 'Water filled plastic pail(index:24)' carried or in room with player |
| Condition| ConditionID 2 ArgID 28| item 'Very large time bomb(index:28)' carried or in room with player |
| Action| ActionID 44 | Print message 'the water spills on the bomb and' |
| Action| ActionID 46 | Print message 'defuses it\! FANTASTIC, You completed an IMPOSSIBLE mission\!' |
| Action| ActionID 63 | game over |
### Action 81 - Input: BRE WIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6781, 582, 523, 860, 580, 40, 10858, 10564|  |
| Verb| 45| BRE |
| Noun| 31| WIR |
| Condition| ConditionID 1 ArgID 29| item 'Red wire going from bomb into wall(index:29)' in room with player |
| Condition| ConditionID 2 ArgID 26| item 'Wire cutters(index:26)' carried or in room with player |
| Action| ActionID 72 ArgID 43, 29| swap item locations 'Loose red wire going into wall(index:43)' and 'Red wire going from bomb into wall(index:29)' |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 82 - Input: DRO MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2742, 321, 234, 320, 0, 0, 2505, 7950|  |
| Verb| 18| DRO |
| Noun| 42| MOP |
| Condition| ConditionID 0 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried |
| Condition| ConditionID 13 ArgID 11| item 'Blue key(index:11)' not in game |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 105 | Print message 'It made an odd sound\.' |
| Action| ActionID 53 ArgID 16| drops item 'Old fashioned yarn mop(index:16)' into current room |
### Action 83 - Input: POU ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 483, 480, 460, 0, 0, 10847, 0|  |
| Verb| 6| POU |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 24| item 'Water filled plastic pail(index:24)' carried or in room with player |
| Action| ActionID 72 ArgID 24, 23| swap item locations 'Water filled plastic pail(index:24)' and 'Empty plastic pail(index:23)' |
| Action| ActionID 47 | Print message 'the water soaks into the floor' |
### Action 84 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 184, 141, 260, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 0 ArgID 7| item 'Picture of me stamped: \-visitor\-(index:7)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 13| move room 13 |
### Action 85 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 184, 161, 260, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 0 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 13| move room 13 |
### Action 86 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 184, 21, 260, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 0 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 13| move room 13 |
### Action 87 - Input: DRO MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2742, 321, 233, 320, 0, 0, 7950, 0|  |
| Verb| 18| DRO |
| Noun| 42| MOP |
| Condition| ConditionID 0 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried |
| Condition| ConditionID 12 ArgID 11| item 'Blue key(index:11)' in game |
| Action| ActionID 53 ArgID 16| drops item 'Old fashioned yarn mop(index:16)' into current room |
### Action 88 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 204, 21, 280, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Condition| ConditionID 0 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 14| move room 14 |
### Action 89 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 204, 161, 280, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Condition| ConditionID 0 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 14| move room 14 |
### Action 90 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 224, 21, 300, 0, 0, 2828, 3204|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Condition| ConditionID 0 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' carried |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 128 | Print message '`ACCEPTED`' |
| Action| ActionID 21 | Print message 'The door opens just long enough for me to scurry through\.' |
| Action| ActionID 54 ArgID 15| move room 15 |
### Action 91 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 204, 0, 0, 0, 0, 10518, 3000|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 20 | Print message '`Authorization INSUFFICIENT for access` ' |
### Action 92 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 184, 0, 0, 0, 0, 10518, 3000|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 20 | Print message '`Authorization INSUFFICIENT for access` ' |
### Action 93 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 224, 0, 0, 0, 0, 10518, 3000|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 20 | Print message '`Authorization INSUFFICIENT for access` ' |
### Action 94 - Input: CLE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1950, 323, 234, 0, 0, 0, 15705, 0|  |
| Verb| 13| CLE |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried or in room with player |
| Condition| ConditionID 13 ArgID 11| item 'Blue key(index:11)' not in game |
| Action| ActionID 104 | Print message 'Oh Boy\.\.\.I think I did something\.\.\.' |
| Action| ActionID 105 | Print message 'It made an odd sound\.' |
### Action 95 - Input: BRE WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6771, 282, 140, 200, 63, 0, 3658, 8700|  |
| Verb| 45| BRE |
| Noun| 21| WIN |
| Condition| ConditionID 1 ArgID 14| item 'Plate glass window with embeded red wires(index:14)' in room with player |
| Condition| ConditionID 2 ArgID 3| item 'Large tape recorder(index:3)' carried or in room with player |
| Action| ActionID 24 | Print message 'Tell me with what? Example: `WITH FIST`' |
| Action| ActionID 58 ArgID 7| set 7 flag |
| Action| ActionID 58 ArgID 10| set 10 flag |
### Action 96 - BREAK WINDOW - Input: WIT TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2257, 282, 63, 148, 60, 20, 11012, 10526|  |
| Verb| 15| WIT |
| Noun| 7| TAP |
| Condition| ConditionID 1 ArgID 14| item 'Plate glass window with embeded red wires(index:14)' in room with player |
| Condition| ConditionID 2 ArgID 3| item 'Large tape recorder(index:3)' carried or in room with player |
| Condition| ConditionID 7 ArgID 7| bitflag 7 is set |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 62 ArgID 3, 1| item 'Large tape recorder(index:3)' is moved to room 1 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 26 | Print message 'Recorder goes flying thru the glass landing in the control room\.Boy what a MESS\! ' |
### Action 97 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 140, 40, 340, 280, 260, 9058, 10858|  |
| Probability| 0%|  |
| Action| ActionID 60 ArgID 7| set 7 flag |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 72 ArgID 17, 14| swap item locations 'Empty window frame(index:17)' and 'Plate glass window with embeded red wires(index:14)' |
| Action| ActionID 58 ArgID 13| set 13 flag |
### Action 98 - Input: GET CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1533, 0, 0, 0, 0, 0, 937, 0|  |
| Verb| 10| GET |
| Noun| 33| CHA |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 99 - Input: LOO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6021, 264, 0, 0, 0, 0, 3300, 0|  |
| Verb| 40| LOO |
| Noun| 21| WIN |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Action| ActionID 22 | Print message 'I'm on the 2nd floor\. Below I see the control room surronding the reactor core\. There's a wide ledge just under the window\.' |
### Action 100 - Input: SCO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 0, 0, 0, 0, 0, 10523, 0|  |
| Verb| 51| SCO |
| Noun| 0| ANY |
| Action| ActionID 70 | clear screen |
| Action| ActionID 23 | Print message 'In this Adventure there's NO score\. Either you make it or \.\.\. ' |
### Action 101 - Input: SIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5400, 102, 100, 0, 0, 0, 10554, 9600|  |
| Verb| 36| SIT |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 5| item 'Chair bolted to floor(index:5)' in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 64 | look |
### Action 102 - Input: OPE WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6471, 0, 0, 0, 0, 0, 907, 2550|  |
| Verb| 43| OPE |
| Noun| 21| WIN |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 7 | Print message 'It appears locked' |
| Action| ActionID 17 | Print message 'Most doors & windows are under automated security control\.' |
### Action 103 - Input: BRE MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6792, 323, 200, 220, 0, 0, 8758, 3600|  |
| Verb| 45| BRE |
| Noun| 42| MOP |
| Condition| ConditionID 2 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried or in room with player |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 58 ArgID 11| set 11 flag |
| Action| ActionID 24 | Print message 'Tell me with what? Example: `WITH FIST`' |
### Action 104 - Input: WIT CUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2282, 523, 228, 220, 200, 220, 8001, 9060|  |
| Verb| 15| WIT |
| Noun| 32| CUT |
| Condition| ConditionID 2 ArgID 26| item 'Wire cutters(index:26)' carried or in room with player |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Action| ActionID 53 ArgID 11| drops item 'Blue key(index:11)' into current room |
| Action| ActionID 51 | Print message 'Something fell to the floor\.' |
| Action| ActionID 60 ArgID 10| set 10 flag |
| Action| ActionID 60 ArgID 11| set 11 flag |
### Action 105 - Input: UNL WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5571, 0, 0, 0, 0, 0, 317, 0|  |
| Verb| 37| UNL |
| Noun| 21| WIN |
| Action| ActionID 2 | Print message 'Nothing happened' |
| Action| ActionID 17 | Print message 'Most doors & windows are under automated security control\.' |
### Action 106 - AUT - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 107 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 843, 260, 264, 823, 0, 9018, 15900|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 2 ArgID 42| item 'Dead saboteur(index:42)' carried or in room with player |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 2 ArgID 41| item 'Picture of saboteur stamped \-window maintance\-(index:41)' carried or in room with player |
| Action| ActionID 60 ArgID 13| set 13 flag |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 106 | Print message '`TV deactivated` ' |
### Action 108 - Input: GO CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 183, 84, 0, 0, 0, 0, 17100, 0|  |
| Verb| 1| GO |
| Noun| 33| CHA |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 114 | Print message 'It seems safe\. Shall I sit down?' |
### Action 109 - . - Input: LOO CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6033, 84, 0, 0, 0, 0, 17100, 0|  |
| Verb| 40| LOO |
| Noun| 33| CHA |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 114 | Print message 'It seems safe\. Shall I sit down?' |
### Action 110 - Input: LOO BOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6029, 563, 0, 0, 0, 0, 16650, 0|  |
| Verb| 40| LOO |
| Noun| 29| BOM |
| Condition| ConditionID 2 ArgID 28| item 'Very large time bomb(index:28)' carried or in room with player |
| Action| ActionID 111 | Print message 'Its a seamless box with 1 small hole for the red wire\.' |
### Action 111 - Input: LOO DET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6030, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 40| LOO |
| Noun| 30| DET |
| Action| ActionID 66 | output inventory |
### Action 112 - Input: DRO SUI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2748, 554, 540, 0, 0, 0, 7950, 0|  |
| Verb| 18| DRO |
| Noun| 48| SUI |
| Condition| ConditionID 13 ArgID 27| item 'Anti\-radiation suit(index:27)' not in game |
| Action| ActionID 53 ArgID 27| drops item 'Anti-radiation suit(index:27)' into current room |
### Action 113 - Input: DRO SUI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2748, 541, 540, 0, 0, 0, 7950, 0|  |
| Verb| 18| DRO |
| Noun| 48| SUI |
| Condition| ConditionID 0 ArgID 27| item 'Anti\-radiation suit(index:27)' carried |
| Action| ActionID 53 ArgID 27| drops item 'Anti-radiation suit(index:27)' into current room |
### Action 114 - Input: LOO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6021, 444, 0, 0, 0, 0, 10549, 0|  |
| Verb| 40| LOO |
| Noun| 21| WIN |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 49 | Print message 'I'm looking into the control room\. I notice that the door is blocked by some debris\.' |
### Action 115 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1528, 463, 502, 460, 480, 0, 10800, 0|  |
| Verb| 10| GET |
| Noun| 28| WAT |
| Condition| ConditionID 2 ArgID 23| item 'Empty plastic pail(index:23)' carried or in room with player |
| Condition| ConditionID 1 ArgID 25| item 'Vat of heavy water(index:25)' in room with player |
| Action| ActionID 72 ArgID 23, 24| swap item locations 'Empty plastic pail(index:23)' and 'Water filled plastic pail(index:24)' |
### Action 116 - PUT ON SUIT - Input: WEA SUI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7848, 543, 540, 0, 0, 0, 8850, 0|  |
| Verb| 52| WEA |
| Noun| 48| SUI |
| Condition| ConditionID 2 ArgID 27| item 'Anti\-radiation suit(index:27)' carried or in room with player |
| Action| ActionID 59 ArgID 27| Item 'Anti-radiation suit(index:27)' is removed from the game (put in room 0) |
### Action 117 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 662, 0, 0, 0, 0, 937, 0|  |
| Verb| 10| GET |
| Noun| 7| TAP |
| Condition| ConditionID 1 ArgID 33| item 'Metal door jammed partially open by remains of a tape recorder(index:33)' in room with player |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 118 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6470, 662, 0, 0, 0, 0, 937, 0|  |
| Verb| 43| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 33| item 'Metal door jammed partially open by remains of a tape recorder(index:33)' in room with player |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 119 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 170, 662, 561, 0, 0, 0, 5700, 0|  |
| Verb| 1| GO |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 33| item 'Metal door jammed partially open by remains of a tape recorder(index:33)' in room with player |
| Condition| ConditionID 0 ArgID 28| item 'Very large time bomb(index:28)' carried |
| Action| ActionID 38 | Print message 'Something won't fit thru the door\.' |
### Action 120 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 170, 662, 300, 0, 0, 0, 10554, 9600|  |
| Verb| 1| GO |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 33| item 'Metal door jammed partially open by remains of a tape recorder(index:33)' in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 64 | look |
### Action 121 - OPE - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6470, 702, 0, 0, 0, 0, 2439, 6037|  |
| Verb| 43| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 39 | Print message 'I turn the knob and push' |
| Action| ActionID 40 | Print message 'gently on the door' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 122 - Input: PRE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3770, 702, 0, 0, 0, 0, 2439, 6037|  |
| Verb| 25| PRE |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 39 | Print message 'I turn the knob and push' |
| Action| ActionID 40 | Print message 'gently on the door' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 123 - Input: PRE HAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3801, 702, 725, 720, 0, 0, 5891, 6353|  |
| Verb| 25| PRE |
| Noun| 51| HAR |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Condition| ConditionID 4 ArgID 36| item 'The door is partially open(index:36)' not in room with player |
| Action| ActionID 39 | Print message 'I turn the knob and push' |
| Action| ActionID 41 | Print message 'hard on the door' |
| Action| ActionID 42 | Print message 'it opens slightly' |
| Action| ActionID 53 ArgID 36| drops item 'The door is partially open(index:36)' into current room |
### Action 124 - Input: PRE HAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3801, 702, 722, 0, 0, 0, 2439, 6187|  |
| Verb| 25| PRE |
| Noun| 51| HAR |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Condition| ConditionID 1 ArgID 36| item 'The door is partially open(index:36)' in room with player |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 39 | Print message 'I turn the knob and push' |
| Action| ActionID 41 | Print message 'hard on the door' |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 125 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 170, 702, 722, 380, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Condition| ConditionID 1 ArgID 36| item 'The door is partially open(index:36)' in room with player |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 126 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 170, 702, 725, 0, 0, 0, 943, 0|  |
| Verb| 1| GO |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Condition| ConditionID 4 ArgID 36| item 'The door is partially open(index:36)' not in room with player |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 43 | Print message 'its closed' |
### Action 127 - Input: KIC DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4670, 702, 725, 720, 0, 0, 19092, 7950|  |
| Verb| 31| KIC |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Plain metal door with sign \-control room\-(index:35)' in room with player |
| Condition| ConditionID 4 ArgID 36| item 'The door is partially open(index:36)' not in room with player |
| Action| ActionID 127 | Print message 'OW\! That HURT\! Anyway' |
| Action| ActionID 42 | Print message 'it opens slightly' |
| Action| ActionID 53 ArgID 36| drops item 'The door is partially open(index:36)' into current room |
### Action 128 - Input: CLO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6320, 0, 0, 0, 0, 0, 5550, 0|  |
| Verb| 42| CLO |
| Noun| 20| DOO |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 129 - Input: SUI UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4955, 543, 540, 0, 0, 0, 8850, 0|  |
| Verb| 33| SUI |
| Noun| 5| UP |
| Condition| ConditionID 2 ArgID 27| item 'Anti\-radiation suit(index:27)' carried or in room with player |
| Action| ActionID 59 ArgID 27| Item 'Anti-radiation suit(index:27)' is removed from the game (put in room 0) |
### Action 130 - Input: SHO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 264, 268, 0, 0, 0, 2720, 0|  |
| Verb| 34| SHO |
| Noun| 14| PIC |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 20 | Print message '`Authorization INSUFFICIENT for access` ' |
### Action 131 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5570, 0, 0, 0, 0, 0, 317, 0|  |
| Verb| 37| UNL |
| Noun| 20| DOO |
| Action| ActionID 2 | Print message 'Nothing happened' |
| Action| ActionID 17 | Print message 'Most doors & windows are under automated security control\.' |
### Action 132 - Input: FRI SAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8139, 843, 794, 780, 800, 820, 8003, 8023|  |
| Verb| 54| FRI |
| Noun| 39| SAB |
| Condition| ConditionID 2 ArgID 42| item 'Dead saboteur(index:42)' carried or in room with player |
| Condition| ConditionID 13 ArgID 39| item 'Empty manila envelope(index:39)' not in game |
| Action| ActionID 53 ArgID 39| drops item 'Empty manila envelope(index:39)' into current room |
| Action| ActionID 53 ArgID 40| drops item 'Piece of yarn(index:40)' into current room |
| Action| ActionID 53 ArgID 41| drops item 'Picture of saboteur stamped -window maintance-(index:41)' into current room |
| Action| ActionID 73 | continue with next action |
### Action 133 - FRISKING SABOTEUR - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 740, 980, 0, 0, 8003, 7703|  |
| Probability| 0%|  |
| Action| ActionID 53 ArgID 0| drops item 'Torn up map(index:0)' into current room |
| Action| ActionID 53 ArgID 37| drops item 'Empty pill case(index:37)' into current room |
| Action| ActionID 51 | Print message 'Something fell to the floor\.' |
| Action| ActionID 53 ArgID 49| drops item 'A leaflet(index:49)' into current room |
### Action 134 - RETURN STOLEN TAPE TOO - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 74, 60, 0, 0, 0, 7950, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 3| item 'Large tape recorder(index:3)' not in game |
| Action| ActionID 53 ArgID 3| drops item 'Large tape recorder(index:3)' into current room |
### Action 135 - Input: KNO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 184, 0, 0, 0, 0, 10518, 2850|  |
| Verb| 53| KNO |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 136 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1350, 0, 0, 0, 0, 0, 17250, 0|  |
| Verb| 9| HEL |
| Noun| 0| ANY |
| Action| ActionID 115 | Print message 'Only help I can think of is to: `Examine everything closely\!` ' |
### Action 137 - Input: PUL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5250, 0, 0, 0, 0, 0, 5550, 0|  |
| Verb| 35| PUL |
| Noun| 0| ANY |
| Action| ActionID 37 | Print message 'It won't budge\!' |
### Action 138 - Input: PRE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 0, 0, 0, 0, 0, 300, 0|  |
| Verb| 25| PRE |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 139 - Input: KNO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 204, 0, 0, 0, 0, 10518, 2850|  |
| Verb| 53| KNO |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 140 - Input: KNO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 224, 0, 0, 0, 0, 10518, 2850|  |
| Verb| 53| KNO |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Metallic voice says:' |
| Action| ActionID 19 | Print message '`Show authorization please` ' |
### Action 141 - Input: KNO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 0, 0, 0, 0, 0, 300, 0|  |
| Verb| 53| KNO |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 142 - Input: WIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 209, 0, 0, 0, 0, 17550, 0|  |
| Verb| 15| WIT |
| Noun| 0| ANY |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 117 | Print message 'HUH?' |
### Action 143 - . - Input: WIT HAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2303, 208, 200, 0, 0, 0, 9127, 300|  |
| Verb| 15| WIT |
| Noun| 53| HAN |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 60 ArgID 10| set 10 flag |
| Action| ActionID 127 | Print message 'OW\! That HURT\! Anyway' |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 144 - Input: FRI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8100, 0, 0, 0, 0, 0, 300, 0|  |
| Verb| 54| FRI |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 145 - Input: KIC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 0, 0, 0, 0, 0, 19052, 0|  |
| Verb| 31| KIC |
| Noun| 0| ANY |
| Action| ActionID 127 | Print message 'OW\! That HURT\! Anyway' |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 146 - Input: SHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5100, 0, 0, 0, 0, 0, 2402, 0|  |
| Verb| 34| SHO |
| Noun| 0| ANY |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 2 | Print message 'Nothing happened' |
### Action 147 - Input: REA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 0, 0, 0, 0, 0, 1002, 0|  |
| Verb| 24| REA |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 102 | Print message 'its unreadable' |
### Action 148 - Input: FIN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 0, 0, 0, 0, 0, 1007, 0|  |
| Verb| 38| FIN |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'I can't do that' |
| Action| ActionID 107 | Print message 'I don't know where to look' |
### Action 149 - Input: BRE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6750, 200, 0, 0, 0, 0, 3658, 0|  |
| Verb| 45| BRE |
| Noun| 0| ANY |
| Action| ActionID 24 | Print message 'Tell me with what? Example: `WITH FIST`' |
| Action| ActionID 58 ArgID 10| set 10 flag |
### Action 150 - Input: WIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 208, 200, 0, 0, 0, 9016, 325|  |
| Verb| 15| WIT |
| Noun| 0| ANY |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 60 ArgID 10| set 10 flag |
| Action| ActionID 16 | Print message 'Strange\.\.\.' |
| Action| ActionID 2 | Print message 'Nothing happened' |
| Action| ActionID 25 | Print message 'Be sure I'm carrying it\!' |
### Action 151 - Input: ACT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8550, 0, 0, 0, 0, 0, 16200, 0|  |
| Verb| 57| ACT |
| Noun| 0| ANY |
| Action| ActionID 108 | Print message 'Tell me how?' |
### Action 152 - Input: WAI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4200, 600, 0, 0, 0, 0, 12575, 0|  |
| Verb| 28| WAI |
| Noun| 0| ANY |
| Action| ActionID 83 | subtract from current counter |
| Action| ActionID 125 | Print message 'Some time passes\.\.\.' |
### Action 153 - Input: UNA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2400, 0, 0, 0, 0, 0, 16200, 0|  |
| Verb| 16| UNA |
| Noun| 0| ANY |
| Action| ActionID 108 | Print message 'Tell me how?' |
### Action 154 - Input: LOO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6052, 983, 0, 0, 0, 0, 18900, 0|  |
| Verb| 40| LOO |
| Noun| 52| LEA |
| Condition| ConditionID 2 ArgID 49| item 'A leaflet(index:49)' carried or in room with player |
| Action| ActionID 126 | Print message 'There is something written there' |
### Action 155 - Input: LOO CAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6037, 264, 268, 0, 0, 0, 16800, 0|  |
| Verb| 40| LOO |
| Noun| 37| CAM |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 112 | Print message 'TV camera is slow scanning the window area\.' |
### Action 156 - Input: LOO CAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6037, 264, 269, 0, 0, 0, 16950, 0|  |
| Verb| 40| LOO |
| Noun| 37| CAM |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 113 | Print message 'TV camera is powered down\. ' |
### Action 157 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 158 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 159 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 160 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 161 - Input: LOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6000, 0, 0, 0, 0, 0, 17476, 0|  |
| Verb| 40| LOO |
| Noun| 0| ANY |
| Action| ActionID 116 | Print message 'I see nothing special\.' |
| Action| ActionID 76 | look |
### Action 163 - Take for item Torn up map - Input: GET MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 43| MAP |
| Condition| ConditionID 1 ArgID 0| item 'Torn up map(index:0)' in room with player |
| Action| ActionID 52 ArgID 0| get item 'Torn up map(index:0)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 164 - Drop for item Torn up map - Input: DRO MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 43| MAP |
| Condition| ConditionID 0 ArgID 0| item 'Torn up map(index:0)' carried |
| Action| ActionID 53 ArgID 0| drops item 'Torn up map(index:0)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 165 - Take for item Picture of me stamped -security- - Input: GET PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| PIC |
| Condition| ConditionID 1 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' in room with player |
| Action| ActionID 52 ArgID 1| get item 'Picture of me stamped -security-(index:1)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 166 - Drop for item Picture of me stamped -security- - Input: DRO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| PIC |
| Condition| ConditionID 0 ArgID 1| item 'Picture of me stamped \-security\-(index:1)' carried |
| Action| ActionID 53 ArgID 1| drops item 'Picture of me stamped -security-(index:1)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 167 - Take for item Large tape recorder - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 7| TAP |
| Condition| ConditionID 1 ArgID 3| item 'Large tape recorder(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Large tape recorder(index:3)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 168 - Drop for item Large tape recorder - Input: DRO TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 7| TAP |
| Condition| ConditionID 0 ArgID 3| item 'Large tape recorder(index:3)' carried |
| Action| ActionID 53 ArgID 3| drops item 'Large tape recorder(index:3)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 169 - Take for item Picture of me stamped: -visitor- - Input: GET PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| PIC |
| Condition| ConditionID 1 ArgID 7| item 'Picture of me stamped: \-visitor\-(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Picture of me stamped: -visitor-(index:7)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 170 - Drop for item Picture of me stamped: -visitor- - Input: DRO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| PIC |
| Condition| ConditionID 0 ArgID 7| item 'Picture of me stamped: \-visitor\-(index:7)' carried |
| Action| ActionID 53 ArgID 7| drops item 'Picture of me stamped: -visitor-(index:7)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 171 - Take for item Picture of me stamped -maintenance- - Input: GET PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| PIC |
| Condition| ConditionID 1 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' in room with player |
| Action| ActionID 52 ArgID 8| get item 'Picture of me stamped -maintenance-(index:8)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 172 - Drop for item Picture of me stamped -maintenance- - Input: DRO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| PIC |
| Condition| ConditionID 0 ArgID 8| item 'Picture of me stamped \-maintenance\-(index:8)' carried |
| Action| ActionID 53 ArgID 8| drops item 'Picture of me stamped -maintenance-(index:8)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 173 - Take for item Blue key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| KEY |
| Condition| ConditionID 1 ArgID 11| item 'Blue key(index:11)' in room with player |
| Action| ActionID 52 ArgID 11| get item 'Blue key(index:11)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 174 - Drop for item Blue key - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 34| KEY |
| Condition| ConditionID 0 ArgID 11| item 'Blue key(index:11)' carried |
| Action| ActionID 53 ArgID 11| drops item 'Blue key(index:11)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 175 - Take for item Yellow key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| KEY |
| Condition| ConditionID 1 ArgID 12| item 'Yellow key(index:12)' in room with player |
| Action| ActionID 52 ArgID 12| get item 'Yellow key(index:12)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 176 - Drop for item Yellow key - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 34| KEY |
| Condition| ConditionID 0 ArgID 12| item 'Yellow key(index:12)' carried |
| Action| ActionID 53 ArgID 12| drops item 'Yellow key(index:12)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 177 - Take for item Old fashioned yarn mop - Input: GET MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 42| MOP |
| Condition| ConditionID 1 ArgID 16| item 'Old fashioned yarn mop(index:16)' in room with player |
| Action| ActionID 52 ArgID 16| get item 'Old fashioned yarn mop(index:16)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 178 - Drop for item Old fashioned yarn mop - Input: DRO MOP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 42| MOP |
| Condition| ConditionID 0 ArgID 16| item 'Old fashioned yarn mop(index:16)' carried |
| Action| ActionID 53 ArgID 16| drops item 'Old fashioned yarn mop(index:16)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 179 - Take for item Broken glass - Input: GET WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 21| WIN |
| Condition| ConditionID 1 ArgID 19| item 'Broken glass(index:19)' in room with player |
| Action| ActionID 52 ArgID 19| get item 'Broken glass(index:19)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 180 - Drop for item Broken glass - Input: DRO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 21| WIN |
| Condition| ConditionID 0 ArgID 19| item 'Broken glass(index:19)' carried |
| Action| ActionID 53 ArgID 19| drops item 'Broken glass(index:19)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 181 - Take for item Movie film cartridge - Input: GET FIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 24| FIL |
| Condition| ConditionID 1 ArgID 22| item 'Movie film cartridge(index:22)' in room with player |
| Action| ActionID 52 ArgID 22| get item 'Movie film cartridge(index:22)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 182 - Drop for item Movie film cartridge - Input: DRO FIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 24| FIL |
| Condition| ConditionID 0 ArgID 22| item 'Movie film cartridge(index:22)' carried |
| Action| ActionID 53 ArgID 22| drops item 'Movie film cartridge(index:22)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 183 - Take for item Empty plastic pail - Input: GET PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| PAI |
| Condition| ConditionID 1 ArgID 23| item 'Empty plastic pail(index:23)' in room with player |
| Action| ActionID 52 ArgID 23| get item 'Empty plastic pail(index:23)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 184 - Drop for item Empty plastic pail - Input: DRO PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| PAI |
| Condition| ConditionID 0 ArgID 23| item 'Empty plastic pail(index:23)' carried |
| Action| ActionID 53 ArgID 23| drops item 'Empty plastic pail(index:23)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 185 - Take for item Water filled plastic pail - Input: GET PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| PAI |
| Condition| ConditionID 1 ArgID 24| item 'Water filled plastic pail(index:24)' in room with player |
| Action| ActionID 52 ArgID 24| get item 'Water filled plastic pail(index:24)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 186 - Drop for item Water filled plastic pail - Input: DRO PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| PAI |
| Condition| ConditionID 0 ArgID 24| item 'Water filled plastic pail(index:24)' carried |
| Action| ActionID 53 ArgID 24| drops item 'Water filled plastic pail(index:24)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 187 - Take for item Wire cutters - Input: GET CUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 32| CUT |
| Condition| ConditionID 1 ArgID 26| item 'Wire cutters(index:26)' in room with player |
| Action| ActionID 52 ArgID 26| get item 'Wire cutters(index:26)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 188 - Drop for item Wire cutters - Input: DRO CUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 32| CUT |
| Condition| ConditionID 0 ArgID 26| item 'Wire cutters(index:26)' carried |
| Action| ActionID 53 ArgID 26| drops item 'Wire cutters(index:26)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 189 - Take for item Anti-radiation suit - Input: GET SUI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 48| SUI |
| Condition| ConditionID 1 ArgID 27| item 'Anti\-radiation suit(index:27)' in room with player |
| Action| ActionID 52 ArgID 27| get item 'Anti-radiation suit(index:27)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 190 - Drop for item Anti-radiation suit - Input: DRO SUI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 48| SUI |
| Condition| ConditionID 0 ArgID 27| item 'Anti\-radiation suit(index:27)' carried |
| Action| ActionID 53 ArgID 27| drops item 'Anti-radiation suit(index:27)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 191 - Take for item Strange lump of glowing plastic - Input: GET PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| PAI |
| Condition| ConditionID 1 ArgID 30| item 'Strange lump of glowing plastic(index:30)' in room with player |
| Action| ActionID 52 ArgID 30| get item 'Strange lump of glowing plastic(index:30)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 192 - Drop for item Strange lump of glowing plastic - Input: DRO PAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| PAI |
| Condition| ConditionID 0 ArgID 30| item 'Strange lump of glowing plastic(index:30)' carried |
| Action| ActionID 53 ArgID 30| drops item 'Strange lump of glowing plastic(index:30)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 193 - Take for item Empty pill case - Input: GET CAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 27| CAS |
| Condition| ConditionID 1 ArgID 37| item 'Empty pill case(index:37)' in room with player |
| Action| ActionID 52 ArgID 37| get item 'Empty pill case(index:37)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 194 - Drop for item Empty pill case - Input: DRO CAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 27| CAS |
| Condition| ConditionID 0 ArgID 37| item 'Empty pill case(index:37)' carried |
| Action| ActionID 53 ArgID 37| drops item 'Empty pill case(index:37)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 195 - Take for item Empty manila envelope - Input: GET ENV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 35| ENV |
| Condition| ConditionID 1 ArgID 39| item 'Empty manila envelope(index:39)' in room with player |
| Action| ActionID 52 ArgID 39| get item 'Empty manila envelope(index:39)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 196 - Drop for item Empty manila envelope - Input: DRO ENV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 35| ENV |
| Condition| ConditionID 0 ArgID 39| item 'Empty manila envelope(index:39)' carried |
| Action| ActionID 53 ArgID 39| drops item 'Empty manila envelope(index:39)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 197 - Take for item Piece of yarn - Input: GET YAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 23| YAR |
| Condition| ConditionID 1 ArgID 40| item 'Piece of yarn(index:40)' in room with player |
| Action| ActionID 52 ArgID 40| get item 'Piece of yarn(index:40)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 198 - Drop for item Piece of yarn - Input: DRO YAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 23| YAR |
| Condition| ConditionID 0 ArgID 40| item 'Piece of yarn(index:40)' carried |
| Action| ActionID 53 ArgID 40| drops item 'Piece of yarn(index:40)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 199 - Take for item Picture of saboteur stamped -window maintance- - Input: GET PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| PIC |
| Condition| ConditionID 1 ArgID 41| item 'Picture of saboteur stamped \-window maintance\-(index:41)' in room with player |
| Action| ActionID 52 ArgID 41| get item 'Picture of saboteur stamped -window maintance-(index:41)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 200 - Drop for item Picture of saboteur stamped -window maintance- - Input: DRO PIC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| PIC |
| Condition| ConditionID 0 ArgID 41| item 'Picture of saboteur stamped \-window maintance\-(index:41)' carried |
| Action| ActionID 53 ArgID 41| drops item 'Picture of saboteur stamped -window maintance-(index:41)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 201 - Take for item Dead saboteur - Input: GET SAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 39| SAB |
| Condition| ConditionID 1 ArgID 42| item 'Dead saboteur(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Dead saboteur(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 202 - Drop for item Dead saboteur - Input: DRO SAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 39| SAB |
| Condition| ConditionID 0 ArgID 42| item 'Dead saboteur(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Dead saboteur(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 203 - Take for item A leaflet - Input: GET LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 52| LEA |
| Condition| ConditionID 1 ArgID 49| item 'A leaflet(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item 'A leaflet(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 204 - Drop for item A leaflet - Input: DRO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 52| LEA |
| Condition| ConditionID 0 ArgID 49| item 'A leaflet(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item 'A leaflet(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 205 - Manually added load game action - Input: LOA GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 29| LOA |
| Noun| 13| GAM |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUT| 0|  |
| GO| 1| ENT, WAL, RUN |
| INV| 5|  |
| POU| 6| SPI, EMP |
| HEL| 9|  |
| GET| 10| TAK, MOV |
| CLE| 13| MOP |
| WIT| 15|  |
| UNA| 16| DIS |
| DRO| 18| PUT, LEA, REM |
| CHA| 22| FOL |
| REA| 24|  |
| PRE| 25| TOU, PUS |
| WAI| 28|  |
| LOA| 29| INS |
| KIC| 31|  |
| JUM| 32|  |
| SUI| 33|  |
| SHO| 34|  |
| PUL| 35|  |
| SIT| 36|  |
| UNL| 37|  |
| FIN| 38| LOC |
| LOO| 40| EXA |
| CLO| 42|  |
| OPE| 43|  |
| \.| 44|  |
| BRE| 45| SMA, CUT, UNB |
| SAV| 49|  |
| QUI| 50|  |
| SCO| 51|  |
| WEA| 52|  |
| KNO| 53|  |
| FRI| 54| SEA, SHA |
| ACT| 57| STA, PLA |
| | 60|  |
| | 61|  |
| | 62|  |
| | 63|  |
| | 64|  |
### Nouns
| Word| Index| Aliases |
| ----| -----| ------- |
| ANY| 0|  |
| NORTH| 1|  |
| SOUTH| 2|  |
| EAST| 3|  |
| WEST| 4|  |
| UP| 5|  |
| DOWN| 6|  |
| TAP| 7| REC |
| RED| 9|  |
| WHI| 10|  |
| BLU| 11|  |
| YEL| 12|  |
| GAM| 13|  |
| PIC| 14| PAS, BAD, AUT |
| ARO| 18|  |
| BUT| 19|  |
| DOO| 20|  |
| WIN| 21| GLA |
| YAR| 23|  |
| FIL| 24| CAR |
| PRO| 26|  |
| CAS| 27|  |
| WAT| 28|  |
| BOM| 29|  |
| DET| 30|  |
| WIR| 31|  |
| CUT| 32|  |
| CHA| 33|  |
| KEY| 34|  |
| ENV| 35| MAN |
| CAM| 37| BOX |
| SAB| 39| HIM, THE |
| MOP| 42|  |
| MAP| 43|  |
| PAI| 44| PLA |
| GRE| 46|  |
| INV| 47|  |
| SUI| 48| ANT, RAD |
| HAR| 51|  |
| LEA| 52|  |
| HAN| 53| FIS, FOO, FEE |
| FLO| 57| WAL |
| VAT| 59|  |
| DIA| 60| GAU |
| DEB| 62|  |
| | 63|  |
| | 64|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| |  |
| 2| briefing room| West: 3 |
| 3| long sloping grey corridor| North: 8, South: 4, East: 2, West: 12, Up: 6, Down: 7 |
| 4| grey room| North: 3 |
| 5| \*I'm sitting in a grey chair there's a box pointing at me|  |
| 6| twisting white hallway| North: 9, East: 8, Down: 3 |
| 7| twisting yellow hallway| North: 10, Up: 3 |
| 8| twisting blue hallway| North: 11, South: 3, West: 6 |
| 9| white room| South: 6 |
| 10| yellow room| South: 7 |
| 11| blue room| South: 8 |
| 12| maintenance room 1| East: 3 |
| 13| large white visitors room|  |
| 14| yellow corridor| West: 17 |
| 15| blue anteroom| West: 23, Up: 22 |
| 16| \*I'm on a ledge outside of a window high above the reactor core|  |
| 17| maintenance room 2| East: 14, Up: 18 |
| 18| projectionist room| Down: 17 |
| 19| Control room surronding the reactor core| East: 20, Down: 21 |
| 20| break room| West: 19 |
| 21| reactor core| Up: 19 |
| 22| small viewing room| Down: 15 |
| 23| storage room| East: 15 |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| Good morning Mr\. Phelps\. Your Mission \(should you decide to accept it\) is to prevent this automated nuclear reactor from being destroyed by a saboteur's TIME BOMB\!  |
| 2| Nothing happened |
| 3| My bomb detector |
| 4| wails ALARMINGLY\! |
| 5| CLICK\! |
| 6| I can't do that |
| 7| It appears locked |
| 8| button is now unlocked |
| 9| Blue |
| 10| Yellow |
| 11| There's a Bright flash & I hear something fall to the floor\. I can't see what it is from here though\.  |
| 12| \*   B O O O O O O O O O M \! \* \* \* \* \* \* |
| 13| The saboteur \(who also rewired the security system\) is a heart patient\. He plans to SUICIDE with the reactor\! He is still loosein the building\. You'll find Security keys & a map in the manila envelope lying next to the tape player\. |
| 14| politely beeps\.\.\.  |
| 15| angrily buzzes\.\.\.  |
| 16| Strange\.\.\. |
| 17| Most doors & windows are under automated security control\. |
| 18| Metallic voice says: |
| 19| `Show authorization please`  |
| 20| `Authorization INSUFFICIENT for access`  |
| 21| The door opens just long enough for me to scurry through\. |
| 22| I'm on the 2nd floor\. Below I see the control room surronding the reactor core\. There's a wide ledge just under the window\. |
| 23| In this Adventure there's NO score\. Either you make it or \.\.\.  |
| 24| Tell me with what? Example: `WITH FIST` |
| 25| Be sure I'm carrying it\! |
| 26| Recorder goes flying thru the glass landing in the control room\.Boy what a MESS\!  |
| 27| Click\! Room lights dim and a screen drops from the ceiling\. You hear a hidden projector start\. |
| 28| The screen illuminates for awhile, but no movie\!? |
| 29| The projector stops, the screen rises, and the lights return\. |
| 30| A movie runs telling about the reactor and its construction interesting highlights: 1\) Plastic DEFORMS strangely in radiation 2\) Even short exposure to HIGH radiation is LETHAL, so suit up  |
| 31| The radiation did something to my pail\! |
| 32| Holding a Radiation Suit |
| 33| doesn't provide much protection for me as I fall down retching I hear/FEEL THE BOMB explode\!  |
| 34| Welcome to Adventure number 3 `MISSION IMPOSSIBLE` by Scott Adams, Dedicated to Maegen Adams\.  |
| 35| A business suit |
| 36| I'm WEARING an anti\-radiation suit\. |
| 37| It won't budge\! |
| 38| Something won't fit thru the door\. |
| 39| I turn the knob and push |
| 40| gently on the door |
| 41| hard on the door |
| 42| it opens slightly |
| 43| its closed |
| 44| the water spills on the bomb and |
| 45| the control panel which immediately shorts out triggering the bomb |
| 46| defuses it\! FANTASTIC, You completed an IMPOSSIBLE mission\! |
| 47| the water soaks into the floor |
| 48| say again & use a color\! |
| 49| I'm looking into the control room\. I notice that the door is blocked by some debris\. |
| 50| In the distance you hear a dull thud; as if someone fell or dropped something heavy\. |
| 51| Something fell to the floor\. |
| 52| its unreadable |
| 53| its still connected |
| 54| Oh Boy\.\.\.I think I did something\.\.\. |
| 55| It made an odd sound\. |
| 56| `TV deactivated`  |
| 57| I don't know where to look |
| 58| Tell me how? |
| 59| Try starting it\. |
| 60| Maybe I should FRISK him? |
| 61| Its a seamless box with 1 small hole for the red wire\. |
| 62| TV camera is slow scanning the window area\. |
| 63| TV camera is powered down\.  |
| 64| It seems safe\. Shall I sit down? |
| 65| Only help I can think of is to: `Examine everything closely\!`  |
| 66| I see nothing special\. |
| 67| HUH? |
| 68| A minute ago someone ran out of this room\! By the way I seem to be carrying something\!  |
| 69| Someone came in the room, he saw me and ran out\! |
| 70| I see no one here\. |
| 71| `Owner of badge is not present\!` |
| 72| Hi\! Look for Adventure number 4: `VOODOO CASTLE` at your favorite computer store\! \(Now back to our current program\.\) |
| 73| Final countdown starts in |
| 74| turns\! |
| 75| Some time passes\.\.\. |
| 76| There is something written there |
| 77| OW\! That HURT\! Anyway |
| 78| `ACCEPTED` |
| 79|  |
| 80|  |
| 81|  |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Torn up map| MAP| 0 |
| 1| Picture of me stamped \-security\-| PIC| 0 |
| 2| Bomb detector flashing yellow \(bomb is now armed\)| | 1 |
| 3| Large tape recorder| TAP| 2 |
| 4| Box with apparatus pointing at chair| | 4 |
| 5| Chair bolted to floor| | 4 |
| 6| Row of 4 buttons \-red white blue yellow\-| | 5 |
| 7| Picture of me stamped: \-visitor\-| PIC| 1 |
| 8| Picture of me stamped \-maintenance\-| PIC| 0 |
| 9| Surgically implanted bomb detector glows green \(bomb's \-safe\-\)| | -1 |
| 10| Bomb detector glowing red \(final countdown active\)| | 0 |
| 11| Blue key| KEY| 0 |
| 12| Yellow key| KEY| 16 |
| 13| Closed white door with tv camera mounted over it| | 9 |
| 14| Plate glass window with embeded red wires| | 13 |
| 15| Panel of buttons \-white green\-| | 13 |
| 16| Old fashioned yarn mop| MOP| 17 |
| 17| Empty window frame| | 0 |
| 18| Tv camera mounted over window| | 13 |
| 19| Broken glass| WIN| 16 |
| 20| Empty movie projector| | 18 |
| 21| Movie projector with film cartridge| | 0 |
| 22| Movie film cartridge| FIL| 19 |
| 23| Empty plastic pail| PAI| 12 |
| 24| Water filled plastic pail| PAI| 0 |
| 25| Vat of heavy water| | 23 |
| 26| Wire cutters| CUT| 17 |
| 27| Anti\-radiation suit| SUI| 23 |
| 28| Very large time bomb| | 21 |
| 29| Red wire going from bomb into wall| | 21 |
| 30| Strange lump of glowing plastic| PAI| 0 |
| 31| Sign `No beverages, Please use Break Room\.`| | 19 |
| 32| Yellow door with tv camera over it| | 10 |
| 33| Metal door jammed partially open by remains of a tape recorder| | 19 |
| 34| Blue door with tv camera over it| | 11 |
| 35| Plain metal door with sign \-control room\-| | 15 |
| 36| The door is partially open| | 0 |
| 37| Empty pill case| CAS| 0 |
| 38| 6 inch window| | 22 |
| 39| Empty manila envelope| ENV| 0 |
| 40| Piece of yarn| YAR| 0 |
| 41| Picture of saboteur stamped \-window maintance\-| PIC| 0 |
| 42| Dead saboteur| SAB| 0 |
| 43| Loose red wire going into wall| | 0 |
| 44| Steps leading down into the reactor core| | 19 |
| 45| Yellow button| | 14 |
| 46| Blue button| | 15 |
| 47| Keyholes under buttons| | 5 |
| 48| Exposed dials and gauges everywhere| | 19 |
| 49| A leaflet| LEA| 0 |
| 50| | | 0 |
| 51| | | 0 |
| 52| | | 0 |
| 53| | | 0 |