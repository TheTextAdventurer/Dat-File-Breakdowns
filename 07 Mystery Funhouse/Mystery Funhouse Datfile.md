# Mystery Funhouse
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
| adventureNumber| 7 |
| Unknown| 5223 |
| numItems| 75 |
| numActions| 210 |
| numNounVerbs| 90 |
| numRooms| 36 |
| maxCarry| 6 |
| startRoom| 1 |
| totalTreasures| 0 |
| wordLength| 4 |
| lightDuration| 500 |
| numMessages| 100 |
| treasureRoom| 0 |
## Actions
### Action 0 - INTRO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 29, 12000, 20, 0, 0, 11908, 2766|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 1| bitflag 1 is false |
| Action| ActionID 79 ArgID 600| set current counter value 600 |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 18 | Print message 'Welcome to ADVENTURE 7, `MYSTERY FUN HOUSE` by Scott Adams Dedicated to Marin Computer Center\.' |
| Action| ActionID 66 | output inventory |
### Action 1 - DECREMENT COUNTER - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 16, 0, 0, 0, 0, 11550, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 15 ArgID 0| current counter greater than '0' |
| Action| ActionID 77 | decrement current counter |
### Action 2 - PARK IS CLOSING - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 815, 0, 0, 0, 0, 2478, 2550|  |
| Probability| 100%|  |
| Condition| ConditionID 14 ArgID 40| current counter less than 40 |
| Action| ActionID 16 | Print message 'The park is closing in' |
| Action| ActionID 78 | output current counter |
| Action| ActionID 17 | Print message 'turns' |
### Action 3 - AIR BLAST - Probability: 40 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 40, 64, 149, 0, 0, 0, 20700, 0|  |
| Probability| 40%|  |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Condition| ConditionID 8 ArgID 7| bitflag 7 is false |
| Action| ActionID 138 | Print message 'Gentle air blast blows up my leg\.' |
### Action 4 - WALL CLOSES - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 204, 109, 100, 0, 0, 8834, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Condition| ConditionID 8 ArgID 5| bitflag 5 is false |
| Action| ActionID 58 ArgID 5| set 5 flag |
| Action| ActionID 134 | Print message 'Wall closed behind me' |
### Action 5 - WALL RESET - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 207, 100, 0, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 6 ArgID 10| player not in room 10 |
| Action| ActionID 60 ArgID 5| set 5 flag |
### Action 6 - HEEL LOOSE - Probability: 5 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5, 83, 494, 0, 0, 0, 18150, 0|  |
| Probability| 5%|  |
| Condition| ConditionID 2 ArgID 4| item 'which I'm wearing(index:4)' carried or in room with player |
| Condition| ConditionID 13 ArgID 24| item 'Bottom of heel(index:24)' not in game |
| Action| ActionID 121 | Print message 'My shoe heel is loose' |
### Action 7 - WALL - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 84, 109, 100, 0, 0, 8700, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Condition| ConditionID 8 ArgID 5| bitflag 5 is false |
| Action| ActionID 58 ArgID 5| set 5 flag |
### Action 8 - AUTHORIZE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 44, 80, 0, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 9 - LOUD CALIOPE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 622, 0, 0, 0, 0, 6300, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 31| item 'LOUD Steam Calliope(index:31)' in room with player |
| Action| ActionID 42 | Print message 'Calliope is so LOUD I can't hear clearly\!' |
### Action 10 - AIR BLAST HARD - Probability: 40 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 40, 64, 148, 0, 0, 0, 20911, 0|  |
| Probability| 40%|  |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Condition| ConditionID 7 ArgID 7| bitflag 7 is set |
| Action| ActionID 139 | Print message 'Hard blast of air rips my body apart' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 11 - CLOSE PARK - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 15, 89, 20, 0, 0, 1554, 11400|  |
| Probability| 100%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 10 | Print message 'Bouncer throws me out' |
| Action| ActionID 54 ArgID 1| move room 1 |
| Action| ActionID 76 | look |
### Action 12 - DOLLAR BILL - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1362, 24, 1360, 0, 0, 8855, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 68| item '5 Dollar Bill(index:68)' in room with player |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 59 ArgID 68| Item '5 Dollar Bill(index:68)' is removed from the game (put in room 0) |
| Action| ActionID 5 | Print message 'Ticket lady rips up bill & says `$5 grocery bill ain't money bub\!`' |
### Action 13 - NO SHOES THROWN OUT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 86, 44, 20, 0, 0, 13288, 1554|  |
| Probability| 100%|  |
| Condition| ConditionID 5 ArgID 4| item 'which I'm wearing(index:4)' not carried |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 10 | Print message 'Bouncer throws me out' |
| Action| ActionID 54 ArgID 1| move room 1 |
### Action 14 - NO TICKET THROW OUT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 466, 44, 20, 0, 0, 13288, 1554|  |
| Probability| 100%|  |
| Condition| ConditionID 5 ArgID 23| item 'Ticket(index:23)' not carried |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 10 | Print message 'Bouncer throws me out' |
| Action| ActionID 54 ArgID 1| move room 1 |
### Action 15 - COMB - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 562, 542, 1180, 1040, 560, 10819, 8850|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 28| item 'Comb(index:28)' in room with player |
| Condition| ConditionID 1 ArgID 27| item 'Mermaid(index:27)' in room with player |
| Action| ActionID 72 ArgID 59, 52| swap item locations 'Bottom of stairs(index:59)' and 'Bottom of slide(index:52)' |
| Action| ActionID 19 | Print message 'She thanks me & turns a hidden knob' |
| Action| ActionID 59 ArgID 28| Item 'Comb(index:28)' is removed from the game (put in room 0) |
### Action 16 - REMOVE STAIR - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1193, 1185, 1180, 1040, 0, 10800, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 12 ArgID 59| item 'Bottom of stairs(index:59)' in game |
| Condition| ConditionID 4 ArgID 59| item 'Bottom of stairs(index:59)' not in room with player |
| Action| ActionID 72 ArgID 59, 52| swap item locations 'Bottom of stairs(index:59)' and 'Bottom of slide(index:52)' |
### Action 17 - PERSON IN ROOM END GAME - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 704, 0, 0, 0, 0, 9450, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 35| player in room 35 |
| Action| ActionID 63 | game over |
### Action 18 - GIVE DOLLAR - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1082, 1080, 460, 24, 0, 7409, 11100|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 54| item 'Silver Dollar(index:54)' in room with player |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 49 | Print message 'She hands me a ticket' |
| Action| ActionID 59 ArgID 54| Item 'Silver Dollar(index:54)' is removed from the game (put in room 0) |
| Action| ActionID 74 ArgID 23| take item 'Ticket(index:23)', no check done to see if can carry |
### Action 19 - HEMP FALL - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 444, 34, 0, 0, 0, 6600, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 13 ArgID 1| item 'Rope hanging from ceiling(index:1)' not in game |
| Action| ActionID 44 | Print message 'Tiny piece of hemp falls on my head and vanishes\!' |
### Action 20 - VALVE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 702, 662, 680, 700, 0, 8009, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 35| item 'Valve handle with no valve(index:35)' in room with player |
| Condition| ConditionID 1 ArgID 33| item 'Valve on a large warm pipe(index:33)' in room with player |
| Action| ActionID 53 ArgID 34| drops item 'Handle is on valve(index:34)' into current room |
| Action| ActionID 59 ArgID 35| Item 'Valve handle with no valve(index:35)' is removed from the game (put in room 0) |
### Action 21 - FUSE GUM - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1142, 753, 745, 740, 0, 7950, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 57| item 'Soft chewing gum(index:57)' in room with player |
| Condition| ConditionID 12 ArgID 37| item 'Fuse is stuck in gum(index:37)' in game |
| Condition| ConditionID 4 ArgID 37| item 'Fuse is stuck in gum(index:37)' not in room with player |
| Action| ActionID 53 ArgID 37| drops item 'Fuse is stuck in gum(index:37)' into current room |
### Action 22 - FUSE GUM - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1141, 753, 740, 0, 0, 11100, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 57| item 'Soft chewing gum(index:57)' carried |
| Condition| ConditionID 12 ArgID 37| item 'Fuse is stuck in gum(index:37)' in game |
| Action| ActionID 74 ArgID 37| take item 'Fuse is stuck in gum(index:37)', no check done to see if can carry |
### Action 23 - AUTHORIZ AREA - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 144, 80, 0, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 7| player in room 7 |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 24 - SHOOTING GALLERY - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 504, 280, 0, 0, 0, 8173, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 54 ArgID 14| move room 14 |
| Action| ActionID 73 | continue with next action |
### Action 25 - SHOT - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1285, 500, 0, 0, 0, 17730, 8163|  |
| Probability| 0%|  |
| Condition| ConditionID 4 ArgID 64| item 'Sign(index:64)' not in room with player |
| Action| ActionID 118 | Print message 'POP' |
| Action| ActionID 30 | Print message 'Someone shot me\!' |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 63 | game over |
### Action 26 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 500, 0, 0, 0, 0, 8100, 0|  |
| Probability| 0%|  |
| Action| ActionID 54 ArgID 25| move room 25 |
### Action 27 - WON - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1341, 0, 0, 0, 0, 21213, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 67| item 'Missing top secret plans(index:67)' carried |
| Action| ActionID 141 | Print message 'HURRAH\! You've done it\!' |
| Action| ActionID 63 | game over |
### Action 28 - DARK - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 684, 309, 0, 0, 0, 8476, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 34| player in room 34 |
| Condition| ConditionID 8 ArgID 15| bitflag 15 is false |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 76 | look |
### Action 29 - LIGHT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 524, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 30 - LIGHT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 504, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 31 - GUM HARDENS - Probability: 5 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5, 1134, 1120, 1140, 754, 0, 10800, 0|  |
| Probability| 5%|  |
| Condition| ConditionID 13 ArgID 56| item 'Hard dry chewing gum(index:56)' not in game |
| Condition| ConditionID 13 ArgID 37| item 'Fuse is stuck in gum(index:37)' not in game |
| Action| ActionID 72 ArgID 56, 57| swap item locations 'Hard dry chewing gum(index:56)' and 'Soft chewing gum(index:57)' |
### Action 32 - OUTSIDE PARK - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 24, 80, 0, 0, 0, 8700, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 33 - SOGGY FUSE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 3, 723, 720, 1480, 0, 10800, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 2 ArgID 0| item 'Closed drain\. Water(index:0)' carried or in room with player |
| Condition| ConditionID 2 ArgID 36| item 'Short fuse(index:36)' carried or in room with player |
| Action| ActionID 72 ArgID 36, 74| swap item locations 'Short fuse(index:36)' and 'Soggy fuse(index:74)' |
### Action 34 - . - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 444, 22, 660, 128, 0, 10501, 8100|  |
| Verb| 66| JUMP |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 1 ArgID 1| item 'Rope hanging from ceiling(index:1)' in room with player |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Action| ActionID 70 | clear screen |
| Action| ActionID 1 | Print message 'Good thing this ropes not too long' |
| Action| ActionID 54 ArgID 33| move room 33 |
### Action 35 - Input: GO ROPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 157, 444, 22, 0, 0, 0, 4035, 0|  |
| Verb| 1| GO |
| Noun| 7| ROPE |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 1 ArgID 1| item 'Rope hanging from ceiling(index:1)' in room with player |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 135 | Print message 'Too high for me' |
### Action 36 - Input: GO SLID
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 102, 773, 100, 80, 0, 8202, 16108|  |
| Verb| 1| GO |
| Noun| 24| SLID |
| Condition| ConditionID 1 ArgID 5| item 'Slippery Slide\. Sign on slide(index:5)' in room with player |
| Condition| ConditionID 12 ArgID 38| item 'Open Drain(index:38)' in game |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 102 | Print message 'Ouch' |
| Action| ActionID 107 | Print message 'Too hard' |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 37 - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 444, 129, 0, 0, 0, 20537, 9150|  |
| Verb| 66| JUMP |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 8 ArgID 6| bitflag 6 is false |
| Action| ActionID 136 | Print message 'Moving ride throws me off balance' |
| Action| ActionID 137 | Print message 'I fell' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 38 - Input: PULL BLUE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5271, 204, 460, 0, 0, 0, 22013, 8176|  |
| Verb| 35| PULL |
| Noun| 21| BLUE |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 146 | Print message 'Click\!' |
| Action| ActionID 113 | Print message 'Wall swings me around & I'm elsewhere\.\.\.' |
| Action| ActionID 54 ArgID 23| move room 23 |
| Action| ActionID 76 | look |
### Action 39 - Input: PULL YELL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5270, 204, 480, 0, 0, 0, 22013, 2004|  |
| Verb| 35| PULL |
| Noun| 20| YELL |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 146 | Print message 'Click\!' |
| Action| ActionID 113 | Print message 'Wall swings me around & I'm elsewhere\.\.\.' |
| Action| ActionID 13 | Print message 'There's strange music playing' |
| Action| ActionID 54 ArgID 24| move room 24 |
### Action 40 - Input: PULL GREE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5269, 204, 160, 0, 0, 0, 22013, 8176|  |
| Verb| 35| PULL |
| Noun| 19| GREE |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 146 | Print message 'Click\!' |
| Action| ActionID 113 | Print message 'Wall swings me around & I'm elsewhere\.\.\.' |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 41 - Input: LOOK UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6605, 444, 20, 0, 0, 0, 8026, 300|  |
| Verb| 44| LOOK |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Action| ActionID 53 ArgID 1| drops item 'Rope hanging from ceiling(index:1)' into current room |
| Action| ActionID 76 | look |
| Action| ActionID 2 | Print message 'OK' |
### Action 42 - Input: LIST ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 282, 0, 0, 0, 0, 314, 0|  |
| Verb| 31| LIST |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 14| item 'Ladder going down(index:14)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 14 | Print message 'Sounds like a space opera' |
### Action 43 - Input: GO TRAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 165, 362, 540, 0, 0, 0, 380, 8176|  |
| Verb| 1| GO |
| Noun| 15| TRAM |
| Condition| ConditionID 1 ArgID 18| item 'Small Trampoline(index:18)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 54 ArgID 27| move room 27 |
| Action| ActionID 76 | look |
### Action 44 - Input: LOOK MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6610, 42, 943, 0, 0, 0, 1808, 0|  |
| Verb| 44| LOOK |
| Noun| 10| MIRR |
| Condition| ConditionID 1 ArgID 2| item 'Strange Mirror(index:2)' in room with player |
| Condition| ConditionID 2 ArgID 47| item 'which I'm wearing(index:47)' carried or in room with player |
| Action| ActionID 12 | Print message 'I can see myself thin,fat & tall' |
| Action| ActionID 8 | Print message 'I see a hidden door in it' |
### Action 45 - Input: GET OFF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1567, 544, 0, 0, 0, 0, 380, 11400|  |
| Verb| 10| GET |
| Noun| 67| OFF |
| Condition| ConditionID 3 ArgID 27| player in room 27 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 76 | look |
### Action 46 - Input: GO COUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 200, 0, 24, 0, 0, 0, 7200, 0|  |
| Verb| 1| GO |
| Noun| 50| COUN |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 48 | Print message 'Ticket lady asks me what I want' |
### Action 47 - Input: LIST ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 484, 0, 0, 0, 0, 2100, 0|  |
| Verb| 31| LIST |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Action| ActionID 14 | Print message 'Sounds like a space opera' |
### Action 48 - Input: LOOK MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6610, 42, 952, 0, 0, 0, 1800, 0|  |
| Verb| 44| LOOK |
| Noun| 10| MIRR |
| Condition| ConditionID 1 ArgID 2| item 'Strange Mirror(index:2)' in room with player |
| Condition| ConditionID 11 ArgID 47| item 'which I'm wearing(index:47)' not carried or in room with player |
| Action| ActionID 12 | Print message 'I can see myself thin,fat & tall' |
### Action 49 - Input: GET DOWN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1506, 544, 0, 0, 0, 0, 380, 11400|  |
| Verb| 10| GET |
| Noun| 6| DOWN |
| Condition| ConditionID 3 ArgID 27| player in room 27 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 76 | look |
### Action 50 - Input: COMB HAIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9365, 563, 545, 0, 0, 0, 300, 0|  |
| Verb| 62| COMB |
| Noun| 65| HAIR |
| Condition| ConditionID 2 ArgID 28| item 'Comb(index:28)' carried or in room with player |
| Condition| ConditionID 4 ArgID 27| item 'Mermaid(index:27)' not in room with player |
| Action| ActionID 2 | Print message 'OK' |
### Action 51 - Input: LOOK WIND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6651, 1242, 553, 0, 0, 0, 4200, 0|  |
| Verb| 44| LOOK |
| Noun| 51| WIND |
| Condition| ConditionID 1 ArgID 62| item 'Window in tank(index:62)' in room with player |
| Condition| ConditionID 12 ArgID 27| item 'Mermaid(index:27)' in game |
| Action| ActionID 28 | Print message 'A mermaid swims by and waves' |
### Action 52 - Input: GO SLID
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 102, 774, 100, 80, 0, 654, 11458|  |
| Verb| 1| GO |
| Noun| 24| SLID |
| Condition| ConditionID 1 ArgID 5| item 'Slippery Slide\. Sign on slide(index:5)' in room with player |
| Condition| ConditionID 13 ArgID 38| item 'Open Drain(index:38)' not in game |
| Action| ActionID 4 | Print message 'Splash, Oh no I am all washed up\!' |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 53 - Input: LOOK MERM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6631, 1242, 113, 573, 0, 0, 21, 0|  |
| Verb| 44| LOOK |
| Noun| 31| MERM |
| Condition| ConditionID 1 ArgID 62| item 'Window in tank(index:62)' in room with player |
| Condition| ConditionID 12 ArgID 5| item 'Slippery Slide\. Sign on slide(index:5)' in game |
| Condition| ConditionID 12 ArgID 28| item 'Comb(index:28)' in game |
| Action| ActionID 21 | Print message 'She's pretty, but has really snarled hair\!' |
### Action 54 - Input: LIGH FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6078, 1386, 0, 0, 0, 0, 3909, 0|  |
| Verb| 40| LIGH |
| Noun| 78| FUSE |
| Condition| ConditionID 5 ArgID 69| item 'Match(index:69)' not carried |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 9 | Print message 'I've no match\!' |
### Action 55 - Input: GO LADD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 177, 282, 320, 80, 0, 0, 8176, 8746|  |
| Verb| 1| GO |
| Noun| 27| LADD |
| Condition| ConditionID 1 ArgID 14| item 'Ladder going down(index:14)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 4| set 4 flag |
| Action| ActionID 46 | Print message 'Fire ladder retracts and leaves me here\!' |
### Action 56 - Input: BREA BOUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7271, 0, 0, 0, 0, 0, 3600, 0|  |
| Verb| 48| BREA |
| Noun| 71| BOUN |
| Action| ActionID 24 | Print message 'Not here\!' |
### Action 57 - Input: DANC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11850, 0, 0, 0, 0, 0, 300, 0|  |
| Verb| 79| DANC |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
### Action 58 - Input: GO EXIT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 166, 802, 0, 0, 0, 0, 4037, 18900|  |
| Verb| 1| GO |
| Noun| 16| EXIT |
| Condition| ConditionID 1 ArgID 40| item 'Exit(index:40)' in room with player |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 137 | Print message 'I fell' |
| Action| ActionID 126 | Print message 'flat on my face\!' |
### Action 59 - Input: READ SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7088, 24, 0, 0, 0, 0, 1650, 0|  |
| Verb| 47| READ |
| Noun| 38| SIGN |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 11 | Print message 'Park closes at midnight\. Shoes required at all times\. Management NOT responsible for accidents\!\! CAUTION this park is DANGERous\! ' |
### Action 60 - Input: BLOW BUBB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3522, 1143, 0, 0, 0, 0, 17700, 0|  |
| Verb| 23| BLOW |
| Noun| 72| BUBB |
| Condition| ConditionID 2 ArgID 57| item 'Soft chewing gum(index:57)' carried or in room with player |
| Action| ActionID 118 | Print message 'POP' |
### Action 61 - Input: BLOW BUBB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3522, 1123, 0, 0, 0, 0, 16307, 0|  |
| Verb| 23| BLOW |
| Noun| 72| BUBB |
| Condition| ConditionID 2 ArgID 56| item 'Hard dry chewing gum(index:56)' carried or in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 107 | Print message 'Too hard' |
### Action 62 - Input: LOOK SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6609, 63, 494, 0, 0, 0, 18150, 0|  |
| Verb| 44| LOOK |
| Noun| 9| SHOE |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Condition| ConditionID 13 ArgID 24| item 'Bottom of heel(index:24)' not in game |
| Action| ActionID 121 | Print message 'My shoe heel is loose' |
### Action 63 - Input: REMO HEEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3787, 63, 494, 480, 780, 0, 374, 8023|  |
| Verb| 25| REMO |
| Noun| 37| HEEL |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Condition| ConditionID 13 ArgID 24| item 'Bottom of heel(index:24)' not in game |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 74 ArgID 24| take item 'Bottom of heel(index:24)', no check done to see if can carry |
| Action| ActionID 53 ArgID 39| drops item 'Letter(index:39)' into current room |
| Action| ActionID 73 | continue with next action |
### Action 64 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 720, 0, 0, 0, 0, 18353, 0|  |
| Probability| 0%|  |
| Action| ActionID 122 | Print message 'Something fell out' |
| Action| ActionID 53 ArgID 36| drops item 'Short fuse(index:36)' into current room |
### Action 65 - Input: SWIM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7500, 2, 0, 0, 0, 0, 3750, 0|  |
| Verb| 50| SWIM |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 0| item 'Closed drain\. Water(index:0)' in room with player |
| Action| ActionID 25 | Print message 'I am' |
### Action 66 - Input: SWIM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7500, 5, 0, 0, 0, 0, 3600, 0|  |
| Verb| 50| SWIM |
| Noun| 0| ANY |
| Condition| ConditionID 4 ArgID 0| item 'Closed drain\. Water(index:0)' not in room with player |
| Action| ActionID 24 | Print message 'Not here\!' |
### Action 67 - Input: CRAW ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11400, 224, 300, 0, 0, 0, 354, 11400|  |
| Verb| 76| CRAW |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 76 | look |
### Action 68 - Input: LOOK WIND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6651, 1262, 0, 0, 0, 0, 450, 0|  |
| Verb| 44| LOOK |
| Noun| 51| WIND |
| Condition| ConditionID 1 ArgID 63| item 'Window\. Gun pointing into & mounted by window(index:63)' in room with player |
| Action| ActionID 3 | Print message 'I see a bunch of clay pigeons' |
### Action 69 - Input: LOOK MERM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6631, 542, 0, 0, 0, 0, 3150, 0|  |
| Verb| 44| LOOK |
| Noun| 31| MERM |
| Condition| ConditionID 1 ArgID 27| item 'Mermaid(index:27)' in room with player |
| Action| ActionID 21 | Print message 'She's pretty, but has really snarled hair\!' |
### Action 70 - Input: GET MERM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1531, 542, 0, 0, 0, 0, 3450, 0|  |
| Verb| 10| GET |
| Noun| 31| MERM |
| Condition| ConditionID 1 ArgID 27| item 'Mermaid(index:27)' in room with player |
| Action| ActionID 23 | Print message 'She's too fast for me' |
### Action 71 - Input: LOOK TREE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6663, 1062, 1114, 1174, 0, 0, 16350, 0|  |
| Verb| 44| LOOK |
| Noun| 63| TREE |
| Condition| ConditionID 1 ArgID 53| item 'Dead tree(index:53)' in room with player |
| Condition| ConditionID 13 ArgID 55| item 'Broken branch(index:55)' not in game |
| Condition| ConditionID 13 ArgID 58| item 'Stick with gum on end(index:58)' not in game |
| Action| ActionID 109 | Print message 'Only thing left is one bare branch' |
### Action 72 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12011, 262, 260, 200, 0, 0, 10802, 0|  |
| Verb| 80| OPEN |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 13| item 'Closed flood door(index:13)' in room with player |
| Action| ActionID 72 ArgID 13, 10| swap item locations 'Closed flood door(index:13)' and 'Open flood door(index:10)' |
| Action| ActionID 2 | Print message 'OK' |
### Action 73 - Input: CLOS DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7811, 202, 260, 200, 0, 0, 10802, 0|  |
| Verb| 52| CLOS |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 10| item 'Open flood door(index:10)' in room with player |
| Action| ActionID 72 ArgID 13, 10| swap item locations 'Closed flood door(index:13)' and 'Open flood door(index:10)' |
| Action| ActionID 2 | Print message 'OK' |
### Action 74 - Input: GO DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 161, 202, 260, 0, 0, 0, 8176, 300|  |
| Verb| 1| GO |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 10| item 'Open flood door(index:10)' in room with player |
| Action| ActionID 54 ArgID 13| move room 13 |
| Action| ActionID 76 | look |
| Action| ActionID 2 | Print message 'OK' |
### Action 75 - . - Input: SHOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2400, 1262, 0, 0, 0, 0, 340, 0|  |
| Verb| 16| SHOO |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 63| item 'Window\. Gun pointing into & mounted by window(index:63)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 40 | Print message 'I shot a clay pigeon\!' |
### Action 76 - Input: LOOK SHEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6664, 322, 194, 1334, 0, 0, 18750, 0|  |
| Verb| 44| LOOK |
| Noun| 64| SHEL |
| Condition| ConditionID 1 ArgID 16| item 'Open door with small shelves beyond(index:16)' in room with player |
| Condition| ConditionID 13 ArgID 9| item 'Lit Flashlight(index:9)' not in game |
| Condition| ConditionID 13 ArgID 66| item 'Flashlight(index:66)' not in game |
| Action| ActionID 125 | Print message 'Flashlight there' |
### Action 77 - Input: GET FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1508, 194, 322, 1320, 0, 0, 7802, 0|  |
| Verb| 10| GET |
| Noun| 8| FLAS |
| Condition| ConditionID 13 ArgID 9| item 'Lit Flashlight(index:9)' not in game |
| Condition| ConditionID 1 ArgID 16| item 'Open door with small shelves beyond(index:16)' in room with player |
| Action| ActionID 52 ArgID 66| get item 'Flashlight(index:66)', check if can carry |
| Action| ActionID 2 | Print message 'OK' |
### Action 78 - Input: GET FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1508, 1322, 1320, 0, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 8| FLAS |
| Condition| ConditionID 1 ArgID 66| item 'Flashlight(index:66)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 66| get item 'Flashlight(index:66)', check if can carry |
### Action 79 - Input: LIGH MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6054, 1383, 1380, 0, 0, 0, 359, 13237|  |
| Verb| 40| LIGH |
| Noun| 54| MATC |
| Condition| ConditionID 2 ArgID 69| item 'Match(index:69)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 59 ArgID 69| Item 'Match(index:69)' is removed from the game (put in room 0) |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 37 | Print message 'its out' |
### Action 80 - Input: GET FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1508, 182, 180, 0, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 8| FLAS |
| Condition| ConditionID 1 ArgID 9| item 'Lit Flashlight(index:9)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 9| get item 'Lit Flashlight(index:9)', check if can carry |
### Action 81 - Input: HELP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4500, 0, 0, 0, 0, 0, 17250, 0|  |
| Verb| 30| HELP |
| Noun| 0| ANY |
| Action| ActionID 115 | Print message 'Try EXAMINING things\!' |
### Action 82 - Input: OPEN ROPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12007, 0, 0, 0, 0, 0, 16250, 0|  |
| Verb| 80| OPEN |
| Noun| 7| ROPE |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 50 | Print message 'Its too tight' |
### Action 83 - Input: GO TREE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 213, 1062, 0, 0, 0, 0, 16200, 0|  |
| Verb| 1| GO |
| Noun| 63| TREE |
| Condition| ConditionID 1 ArgID 53| item 'Dead tree(index:53)' in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
### Action 84 - Input: STIC GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6359, 1141, 0, 0, 0, 0, 5100, 0|  |
| Verb| 42| STIC |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 57| item 'Soft chewing gum(index:57)' carried |
| Action| ActionID 34 | Print message 'On what?' |
### Action 85 - Input: ON FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11178, 1143, 740, 723, 720, 0, 353, 8850|  |
| Verb| 74| ON |
| Noun| 78| FUSE |
| Condition| ConditionID 2 ArgID 57| item 'Soft chewing gum(index:57)' carried or in room with player |
| Condition| ConditionID 2 ArgID 36| item 'Short fuse(index:36)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 53 ArgID 37| drops item 'Fuse is stuck in gum(index:37)' into current room |
| Action| ActionID 59 ArgID 36| Item 'Short fuse(index:36)' is removed from the game (put in room 0) |
### Action 86 - Input: GO POLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 163, 1222, 440, 80, 0, 0, 354, 6658|  |
| Verb| 1| GO |
| Noun| 13| POLE |
| Condition| ConditionID 1 ArgID 61| item 'Pole coming out of horse's back(index:61)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 22| move room 22 |
| Action| ActionID 44 | Print message 'Tiny piece of hemp falls on my head and vanishes\!' |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 87 - Input: LIGH FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6008, 1323, 180, 1320, 0, 0, 372, 11400|  |
| Verb| 40| LIGH |
| Noun| 8| FLAS |
| Condition| ConditionID 2 ArgID 66| item 'Flashlight(index:66)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 72 ArgID 9, 66| swap item locations 'Lit Flashlight(index:9)' and 'Flashlight(index:66)' |
| Action| ActionID 76 | look |
### Action 88 - Input: UNLI FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9158, 183, 180, 1320, 0, 0, 372, 11400|  |
| Verb| 61| UNLI |
| Noun| 8| FLAS |
| Condition| ConditionID 2 ArgID 9| item 'Lit Flashlight(index:9)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 72 ArgID 9, 66| swap item locations 'Lit Flashlight(index:9)' and 'Flashlight(index:66)' |
| Action| ActionID 76 | look |
### Action 89 - Input: SAY TICK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8435, 24, 0, 0, 0, 0, 385, 15450|  |
| Verb| 56| SAY |
| Noun| 35| TICK |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 103 | Print message 'She says: `That'll be a dollar`' |
### Action 90 - Input: USE BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5757, 49, 1022, 1103, 0, 0, 16611, 0|  |
| Verb| 38| USE |
| Noun| 57| BRAN |
| Condition| ConditionID 8 ArgID 2| bitflag 2 is false |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Condition| ConditionID 2 ArgID 55| item 'Broken branch(index:55)' carried or in room with player |
| Action| ActionID 110 | Print message 'Doesn't work' |
| Action| ActionID 111 | Print message 'I just push it around' |
### Action 91 - Input: GUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 0, 0, 0, 0, 0, 5850, 0|  |
| Verb| 15| GUM |
| Noun| 0| ANY |
| Action| ActionID 39 | Print message 'Try: `STICK GUM`' |
### Action 92 - Input: FIX HEEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12937, 63, 494, 0, 0, 0, 300, 0|  |
| Verb| 86| FIX |
| Noun| 37| HEEL |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Condition| ConditionID 13 ArgID 24| item 'Bottom of heel(index:24)' not in game |
| Action| ActionID 2 | Print message 'OK' |
### Action 93 - Input: GO MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 42, 0, 0, 0, 0, 402, 4050|  |
| Verb| 1| GO |
| Noun| 10| MIRR |
| Condition| ConditionID 1 ArgID 2| item 'Strange Mirror(index:2)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 102 | Print message 'Ouch' |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 94 - Input: OPEN GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12047, 0, 0, 0, 0, 0, 3900, 0|  |
| Verb| 80| OPEN |
| Noun| 47| GRAT |
| Action| ActionID 26 | Print message 'How?' |
### Action 95 - Input: READ SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7088, 102, 0, 0, 0, 0, 18450, 0|  |
| Verb| 47| READ |
| Noun| 38| SIGN |
| Condition| ConditionID 1 ArgID 5| item 'Slippery Slide\. Sign on slide(index:5)' in room with player |
| Action| ActionID 123 | Print message 'AUTHORIZED PERSONNEL ONLY\!' |
### Action 96 - Input: LOOK GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6647, 1022, 49, 0, 0, 0, 404, 20080|  |
| Verb| 44| LOOK |
| Noun| 47| GRAT |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Condition| ConditionID 8 ArgID 2| bitflag 2 is false |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 104 | Print message 'I see a shiny COIN at the bottom of the drain\!' |
| Action| ActionID 133 | Print message '2' |
| Action| ActionID 130 | Print message 'big bolts hold it down' |
### Action 97 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12011, 601, 162, 160, 320, 0, 8303, 0|  |
| Verb| 80| OPEN |
| Noun| 11| DOOR |
| Condition| ConditionID 0 ArgID 30| item 'Rusty key(index:30)' carried |
| Condition| ConditionID 1 ArgID 8| item 'Locked door(index:8)' in room with player |
| Action| ActionID 55 ArgID 8| Item 'Locked door(index:8)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 16| drops item 'Open door with small shelves beyond(index:16)' into current room |
### Action 98 - Input: GET DOLL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1560, 1094, 1022, 0, 0, 0, 4005, 0|  |
| Verb| 10| GET |
| Noun| 60| DOLL |
| Condition| ConditionID 13 ArgID 54| item 'Silver Dollar(index:54)' not in game |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 105 | Print message 'I can't reach it, my arm is too short\!' |
### Action 99 - Input: GET DOLL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1560, 1082, 1080, 0, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 60| DOLL |
| Condition| ConditionID 1 ArgID 54| item 'Silver Dollar(index:54)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 54| get item 'Silver Dollar(index:54)', check if can carry |
### Action 100 - Input: OPEN DRAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12042, 760, 0, 540, 2, 0, 10831, 8323|  |
| Verb| 80| OPEN |
| Noun| 42| DRAI |
| Condition| ConditionID 1 ArgID 0| item 'Closed drain\. Water(index:0)' in room with player |
| Action| ActionID 72 ArgID 38, 0| swap item locations 'Open Drain(index:38)' and 'Closed drain. Water(index:0)' |
| Action| ActionID 31 | Print message 'All the water ran out' |
| Action| ActionID 55 ArgID 27| Item 'Mermaid(index:27)' is removed from the game (put in room 0) |
| Action| ActionID 73 | continue with next action |
### Action 101 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 602, 600, 0, 0, 0, 8250, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 30| item 'Rusty key(index:30)' in room with player |
| Action| ActionID 55 ArgID 30| Item 'Rusty key(index:30)' is removed from the game (put in room 0) |
### Action 102 - Input: TOUC PIPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4106, 662, 0, 0, 0, 0, 402, 21600|  |
| Verb| 27| TOUC |
| Noun| 56| PIPE |
| Condition| ConditionID 1 ArgID 33| item 'Valve on a large warm pipe(index:33)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 102 | Print message 'Ouch' |
| Action| ActionID 144 | Print message 'too hot' |
### Action 103 - Input: CLOS DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7811, 322, 160, 320, 0, 0, 8005, 300|  |
| Verb| 52| CLOS |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 16| item 'Open door with small shelves beyond(index:16)' in room with player |
| Action| ActionID 53 ArgID 8| drops item 'Locked door(index:8)' into current room |
| Action| ActionID 55 ArgID 16| Item 'Open door with small shelves beyond(index:16)' is removed from the game (put in room 0) |
| Action| ActionID 2 | Print message 'OK' |
### Action 104 - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 363, 0, 0, 0, 0, 3925, 21450|  |
| Verb| 66| JUMP |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 18| item 'Small Trampoline(index:18)' carried or in room with player |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 25 | Print message 'I am' |
| Action| ActionID 143 | Print message 'not on it' |
### Action 105 - Input: STIC GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6359, 1123, 0, 0, 0, 0, 16307, 0|  |
| Verb| 42| STIC |
| Noun| 59| GUM |
| Condition| ConditionID 2 ArgID 56| item 'Hard dry chewing gum(index:56)' carried or in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 107 | Print message 'Too hard' |
### Action 106 - . - Input: LOOK WATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6640, 503, 0, 0, 0, 0, 11717, 2250|  |
| Verb| 44| LOOK |
| Noun| 40| WATC |
| Condition| ConditionID 2 ArgID 25| item 'Watch(index:25)' carried or in room with player |
| Action| ActionID 78 | output current counter |
| Action| ActionID 17 | Print message 'turns' |
| Action| ActionID 15 | Print message 'till midnight' |
### Action 107 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 108 - Input: ON BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11157, 1143, 1103, 1100, 1160, 0, 372, 0|  |
| Verb| 74| ON |
| Noun| 57| BRAN |
| Condition| ConditionID 2 ArgID 57| item 'Soft chewing gum(index:57)' carried or in room with player |
| Condition| ConditionID 2 ArgID 55| item 'Broken branch(index:55)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 72 ArgID 55, 58| swap item locations 'Broken branch(index:55)' and 'Stick with gum on end(index:58)' |
### Action 109 - Input: USE BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5757, 1163, 49, 1022, 1080, 40, 374, 15958|  |
| Verb| 38| USE |
| Noun| 57| BRAN |
| Condition| ConditionID 2 ArgID 58| item 'Stick with gum on end(index:58)' carried or in room with player |
| Condition| ConditionID 8 ArgID 2| bitflag 2 is false |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 74 ArgID 54| take item 'Silver Dollar(index:54)', no check done to see if can carry |
| Action| ActionID 106 | Print message 'Got it\!' |
| Action| ActionID 58 ArgID 2| set 2 flag |
### Action 110 - Input: LOOK MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6610, 1422, 0, 0, 0, 0, 21300, 0|  |
| Verb| 44| LOOK |
| Noun| 10| MIRR |
| Condition| ConditionID 1 ArgID 71| item '1 way mirror(index:71)' in room with player |
| Action| ActionID 142 | Print message 'I see into the mirror room' |
### Action 111 - Input: GET BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1557, 1162, 1160, 0, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 58| item 'Stick with gum on end(index:58)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 58| get item 'Stick with gum on end(index:58)', check if can carry |
### Action 112 - Input: CHEW GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8309, 1121, 1120, 1140, 0, 0, 372, 6750|  |
| Verb| 55| CHEW |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 56| item 'Hard dry chewing gum(index:56)' carried |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 72 ArgID 56, 57| swap item locations 'Hard dry chewing gum(index:56)' and 'Soft chewing gum(index:57)' |
| Action| ActionID 45 | Print message 'Tastes HORRIBLE\!' |
### Action 113 - Input: CHEW GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8309, 1141, 0, 0, 0, 0, 345, 0|  |
| Verb| 55| CHEW |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 57| item 'Soft chewing gum(index:57)' carried |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 45 | Print message 'Tastes HORRIBLE\!' |
### Action 114 - Input: EAT GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8159, 1121, 1120, 0, 0, 0, 359, 6750|  |
| Verb| 54| EAT |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 56| item 'Hard dry chewing gum(index:56)' carried |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 59 ArgID 56| Item 'Hard dry chewing gum(index:56)' is removed from the game (put in room 0) |
| Action| ActionID 45 | Print message 'Tastes HORRIBLE\!' |
### Action 115 - Input: GET BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1557, 1062, 1114, 1100, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 53| item 'Dead tree(index:53)' in room with player |
| Condition| ConditionID 13 ArgID 55| item 'Broken branch(index:55)' not in game |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 55| get item 'Broken branch(index:55)', check if can carry |
### Action 116 - Input: GET BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1557, 1102, 1100, 0, 0, 0, 352, 0|  |
| Verb| 10| GET |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 55| item 'Broken branch(index:55)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 55| get item 'Broken branch(index:55)', check if can carry |
### Action 117 - Input: GET GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1547, 0, 0, 0, 0, 0, 3900, 0|  |
| Verb| 10| GET |
| Noun| 47| GRAT |
| Action| ActionID 26 | Print message 'How?' |
### Action 118 - Input: EAT GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8159, 1141, 1140, 0, 0, 0, 359, 6750|  |
| Verb| 54| EAT |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 57| item 'Soft chewing gum(index:57)' carried |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 59 ArgID 57| Item 'Soft chewing gum(index:57)' is removed from the game (put in room 0) |
| Action| ActionID 45 | Print message 'Tastes HORRIBLE\!' |
### Action 119 - Input: BREA BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7257, 1062, 1114, 1100, 0, 0, 352, 0|  |
| Verb| 48| BREA |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 53| item 'Dead tree(index:53)' in room with player |
| Condition| ConditionID 13 ArgID 55| item 'Broken branch(index:55)' not in game |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 52 ArgID 55| get item 'Broken branch(index:55)', check if can carry |
### Action 120 - Input: GET SKEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1512, 142, 140, 880, 0, 0, 8303, 6150|  |
| Verb| 10| GET |
| Noun| 12| SKEL |
| Condition| ConditionID 1 ArgID 7| item 'Skeleton(index:7)' in room with player |
| Action| ActionID 55 ArgID 7| Item 'Skeleton(index:7)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 44| drops item 'Pile of bones(index:44)' into current room |
| Action| ActionID 41 | Print message 'It collapsed into a pile of bones' |
### Action 121 - Input: LOOK MACH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6633, 963, 0, 0, 0, 0, 19350, 0|  |
| Verb| 44| LOOK |
| Noun| 33| MACH |
| Condition| ConditionID 2 ArgID 48| item 'Fortune telling machine(index:48)' carried or in room with player |
| Action| ActionID 129 | Print message 'There's a red button' |
### Action 122 - Input: GO ROPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 157, 982, 440, 0, 0, 0, 354, 0|  |
| Verb| 1| GO |
| Noun| 7| ROPE |
| Condition| ConditionID 1 ArgID 49| item 'Rope hanging down(index:49)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 22| move room 22 |
### Action 123 - Input: ON GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11147, 1143, 862, 1140, 1000, 0, 8903, 10950|  |
| Verb| 74| ON |
| Noun| 47| GRAT |
| Condition| ConditionID 2 ArgID 57| item 'Soft chewing gum(index:57)' carried or in room with player |
| Condition| ConditionID 1 ArgID 43| item 'Large grate welded over hole(index:43)' in room with player |
| Action| ActionID 59 ArgID 57| Item 'Soft chewing gum(index:57)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 50| drops item 'Gum is stuck to grate(index:50)' into current room |
| Action| ActionID 73 | continue with next action |
### Action 124 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 741, 740, 0, 0, 0, 7950, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 0 ArgID 37| item 'Fuse is stuck in gum(index:37)' carried |
| Action| ActionID 53 ArgID 37| drops item 'Fuse is stuck in gum(index:37)' into current room |
### Action 125 - Input: PRES ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5400, 962, 0, 0, 0, 0, 21118, 16500|  |
| Verb| 36| PRES |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 48| item 'Fortune telling machine(index:48)' in room with player |
| Action| ActionID 140 | Print message 'Machine lights up and says' |
| Action| ActionID 118 | Print message 'POP' |
| Action| ActionID 110 | Print message 'Doesn't work' |
### Action 126 - . - Input: READ SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7088, 342, 0, 0, 0, 0, 18450, 0|  |
| Verb| 47| READ |
| Noun| 38| SIGN |
| Condition| ConditionID 1 ArgID 17| item 'Sign on ladder(index:17)' in room with player |
| Action| ActionID 123 | Print message 'AUTHORIZED PERSONNEL ONLY\!' |
### Action 127 - Input: GO SLID
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 1042, 2, 0, 0, 0, 904, 0|  |
| Verb| 1| GO |
| Noun| 24| SLID |
| Condition| ConditionID 1 ArgID 52| item 'Bottom of slide(index:52)' in room with player |
| Condition| ConditionID 1 ArgID 0| item 'Closed drain\. Water(index:0)' in room with player |
| Action| ActionID 6 | Print message 'Too steep' |
| Action| ActionID 4 | Print message 'Splash, Oh no I am all washed up\!' |
### Action 128 - . - Input: GO STAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 182, 1182, 60, 80, 0, 0, 354, 11460|  |
| Verb| 1| GO |
| Noun| 32| STAI |
| Condition| ConditionID 1 ArgID 59| item 'Bottom of stairs(index:59)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 3| move room 3 |
| Action| ActionID 76 | look |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 129 - Input: READ LETT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7116, 783, 0, 0, 0, 0, 17100, 0|  |
| Verb| 47| READ |
| Noun| 66| LETT |
| Condition| ConditionID 2 ArgID 39| item 'Letter(index:39)' carried or in room with player |
| Action| ActionID 114 | Print message 'James: We must get the plans back by tonight\! We believe they're hiddenwithin his Fun House\!  Signed, M P\.S\. Q says enjoy the gum\!' |
### Action 130 - Input: GO FUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 218, 24, 40, 80, 0, 0, 354, 11460|  |
| Verb| 1| GO |
| Noun| 68| FUN |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 2| move room 2 |
| Action| ActionID 76 | look |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 131 - Input: GO MERR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 225, 622, 0, 0, 0, 0, 17850, 0|  |
| Verb| 1| GO |
| Noun| 75| MERR |
| Condition| ConditionID 1 ArgID 31| item 'LOUD Steam Calliope(index:31)' in room with player |
| Action| ActionID 119 | Print message 'HUH? Why do you want me to MARRY?' |
### Action 132 - Input: GO MERR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 225, 642, 582, 360, 0, 0, 354, 11400|  |
| Verb| 1| GO |
| Noun| 75| MERR |
| Condition| ConditionID 1 ArgID 32| item 'Merry\-Go\-Round(index:32)' in room with player |
| Condition| ConditionID 1 ArgID 29| item 'Quiet Calliope(index:29)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 76 | look |
### Action 133 - Input: TURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 662, 685, 0, 0, 0, 16320, 0|  |
| Verb| 51| TURN |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 33| item 'Valve on a large warm pipe(index:33)' in room with player |
| Condition| ConditionID 4 ArgID 34| item 'Handle is on valve(index:34)' not in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 120 | Print message 'There's no handle on it' |
### Action 134 - Input: TURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 682, 68, 60, 580, 620, 360, 10800|  |
| Verb| 51| TURN |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 34| item 'Handle is on valve(index:34)' in room with player |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 60 ArgID 3| set 3 flag |
| Action| ActionID 72 ArgID 29, 31| swap item locations 'Quiet Calliope(index:29)' and 'LOUD Steam Calliope(index:31)' |
### Action 135 - Input: TURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 682, 69, 60, 580, 620, 358, 10800|  |
| Verb| 51| TURN |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 34| item 'Handle is on valve(index:34)' in room with player |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 58 ArgID 3| set 3 flag |
| Action| ActionID 72 ArgID 29, 31| swap item locations 'Quiet Calliope(index:29)' and 'LOUD Steam Calliope(index:31)' |
### Action 136 - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 544, 0, 0, 0, 0, 3373, 12000|  |
| Verb| 66| JUMP |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 27| player in room 27 |
| Action| ActionID 22 | Print message 'Wheeee' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 80 | swap location with saved location |
### Action 137 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 324, 300, 80, 0, 0, 8176, 9000|  |
| Probability| 0%|  |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 76 | look |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 138 - . - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 307, 540, 707, 0, 0, 12000, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 6 ArgID 15| player not in room 15 |
| Condition| ConditionID 6 ArgID 35| player not in room 35 |
| Action| ActionID 80 | swap location with saved location |
### Action 139 - Input: PRES BLUE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5421, 1462, 128, 120, 0, 0, 9146, 19093|  |
| Verb| 36| PRES |
| Noun| 21| BLUE |
| Condition| ConditionID 1 ArgID 73| item 'Blue button(index:73)' in room with player |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Action| ActionID 60 ArgID 6| set 6 flag |
| Action| ActionID 146 | Print message 'Click\!' |
| Action| ActionID 127 | Print message 'Ride' |
| Action| ActionID 43 | Print message 'starts\.' |
### Action 140 - Input: REMO SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3759, 83, 80, 0, 0, 0, 359, 0|  |
| Verb| 25| REMO |
| Noun| 9| SHOE |
| Condition| ConditionID 2 ArgID 4| item 'which I'm wearing(index:4)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 59 ArgID 4| Item 'which I'm wearing(index:4)' is removed from the game (put in room 0) |
### Action 141 - Input: WEAR SPEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6493, 923, 940, 920, 0, 0, 374, 11100|  |
| Verb| 43| WEAR |
| Noun| 43| SPEC |
| Condition| ConditionID 2 ArgID 46| item 'Strange spectacles(index:46)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 74 ArgID 47| take item 'which I'm wearing(index:47)', no check done to see if can carry |
| Action| ActionID 74 ArgID 46| take item 'Strange spectacles(index:46)', no check done to see if can carry |
### Action 142 - Input: REMO SPEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3793, 943, 940, 0, 0, 0, 359, 0|  |
| Verb| 25| REMO |
| Noun| 43| SPEC |
| Condition| ConditionID 2 ArgID 47| item 'which I'm wearing(index:47)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 59 ArgID 47| Item 'which I'm wearing(index:47)' is removed from the game (put in room 0) |
### Action 143 - Input: DROP SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2709, 63, 60, 80, 0, 0, 8009, 300|  |
| Verb| 18| DROP |
| Noun| 9| SHOE |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Action| ActionID 53 ArgID 3| drops item 'Shoes(index:3)' into current room |
| Action| ActionID 59 ArgID 4| Item 'which I'm wearing(index:4)' is removed from the game (put in room 0) |
| Action| ActionID 2 | Print message 'OK' |
### Action 144 - Input: DROP SPEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2743, 923, 920, 940, 0, 0, 8009, 300|  |
| Verb| 18| DROP |
| Noun| 43| SPEC |
| Condition| ConditionID 2 ArgID 46| item 'Strange spectacles(index:46)' carried or in room with player |
| Action| ActionID 53 ArgID 46| drops item 'Strange spectacles(index:46)' into current room |
| Action| ActionID 59 ArgID 47| Item 'which I'm wearing(index:47)' is removed from the game (put in room 0) |
| Action| ActionID 2 | Print message 'OK' |
### Action 145 - Input: LIGH FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6078, 723, 0, 0, 0, 0, 5473, 13288|  |
| Verb| 40| LIGH |
| Noun| 78| FUSE |
| Condition| ConditionID 2 ArgID 36| item 'Short fuse(index:36)' carried or in room with player |
| Action| ActionID 36 | Print message 'Sizzle, it burns with a dull glow\.' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
### Action 146 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 720, 1380, 0, 0, 0, 8887, 8850|  |
| Probability| 0%|  |
| Action| ActionID 59 ArgID 36| Item 'Short fuse(index:36)' is removed from the game (put in room 0) |
| Action| ActionID 37 | Print message 'its out' |
| Action| ActionID 59 ArgID 69| Item 'Match(index:69)' is removed from the game (put in room 0) |
### Action 147 - Input: LIGH FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6078, 743, 0, 0, 0, 0, 5473, 13318|  |
| Verb| 40| LIGH |
| Noun| 78| FUSE |
| Condition| ConditionID 2 ArgID 37| item 'Fuse is stuck in gum(index:37)' carried or in room with player |
| Action| ActionID 36 | Print message 'Sizzle, it burns with a dull glow\.' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 118 | Print message 'POP' |
### Action 148 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 741, 0, 0, 0, 0, 5761, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 0 ArgID 37| item 'Fuse is stuck in gum(index:37)' carried |
| Action| ActionID 38 | Print message 'I was holding it\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 149 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 707, 1002, 1200, 860, 0, 10800, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 6 ArgID 35| player not in room 35 |
| Condition| ConditionID 1 ArgID 50| item 'Gum is stuck to grate(index:50)' in room with player |
| Action| ActionID 72 ArgID 60, 43| swap item locations 'Broken grate(index:60)' and 'Large grate welded over hole(index:43)' |
### Action 150 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 707, 265, 700, 0, 0, 8176, 18600|  |
| Probability| 0%|  |
| Condition| ConditionID 6 ArgID 35| player not in room 35 |
| Condition| ConditionID 4 ArgID 13| item 'Closed flood door(index:13)' not in room with player |
| Action| ActionID 54 ArgID 35| move room 35 |
| Action| ActionID 76 | look |
| Action| ActionID 124 | Print message 'Guard hears explosion & shoots me\!' |
### Action 151 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1380, 740, 1000, 1140, 0, 8909, 8909|  |
| Probability| 0%|  |
| Action| ActionID 59 ArgID 69| Item 'Match(index:69)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 37| Item 'Fuse is stuck in gum(index:37)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 50| Item 'Gum is stuck to grate(index:50)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 57| Item 'Soft chewing gum(index:57)' is removed from the game (put in room 0) |
### Action 152 - Input: PRES RED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5426, 222, 148, 140, 0, 0, 9002, 21900|  |
| Verb| 36| PRES |
| Noun| 26| RED |
| Condition| ConditionID 1 ArgID 11| item 'Red knob in wall(index:11)' in room with player |
| Condition| ConditionID 7 ArgID 7| bitflag 7 is set |
| Action| ActionID 60 ArgID 7| set 7 flag |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 146 | Print message 'Click\!' |
### Action 153 - Input: PRES BLUE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5421, 1462, 129, 120, 0, 0, 8846, 19178|  |
| Verb| 36| PRES |
| Noun| 21| BLUE |
| Condition| ConditionID 1 ArgID 73| item 'Blue button(index:73)' in room with player |
| Condition| ConditionID 8 ArgID 6| bitflag 6 is false |
| Action| ActionID 58 ArgID 6| set 6 flag |
| Action| ActionID 146 | Print message 'Click\!' |
| Action| ActionID 127 | Print message 'Ride' |
| Action| ActionID 128 | Print message 'stops\.' |
### Action 154 - Input: LOOK GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6647, 1022, 0, 0, 0, 0, 20080, 0|  |
| Verb| 44| LOOK |
| Noun| 47| GRAT |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Action| ActionID 133 | Print message '2' |
| Action| ActionID 130 | Print message 'big bolts hold it down' |
### Action 155 - Input: LOOK GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6647, 902, 0, 0, 0, 0, 19930, 0|  |
| Verb| 44| LOOK |
| Noun| 47| GRAT |
| Condition| ConditionID 1 ArgID 45| item 'Loose grate(index:45)' in room with player |
| Action| ActionID 132 | Print message '1' |
| Action| ActionID 130 | Print message 'big bolts hold it down' |
### Action 156 - Input: MOVE GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10697, 902, 520, 534, 0, 0, 7952, 0|  |
| Verb| 71| MOVE |
| Noun| 47| GRAT |
| Condition| ConditionID 1 ArgID 45| item 'Loose grate(index:45)' in room with player |
| Condition| ConditionID 13 ArgID 26| item 'Dark manhole(index:26)' not in game |
| Action| ActionID 53 ArgID 26| drops item 'Dark manhole(index:26)' into current room |
| Action| ActionID 2 | Print message 'OK' |
### Action 157 - Input: MOVE GRAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10697, 902, 533, 520, 0, 0, 8852, 0|  |
| Verb| 71| MOVE |
| Noun| 47| GRAT |
| Condition| ConditionID 1 ArgID 45| item 'Loose grate(index:45)' in room with player |
| Condition| ConditionID 12 ArgID 26| item 'Dark manhole(index:26)' in game |
| Action| ActionID 59 ArgID 26| Item 'Dark manhole(index:26)' is removed from the game (put in room 0) |
| Action| ActionID 2 | Print message 'OK' |
### Action 158 - Input: USE WREN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5781, 383, 1022, 1020, 900, 0, 10802, 19650|  |
| Verb| 38| USE |
| Noun| 81| WREN |
| Condition| ConditionID 2 ArgID 19| item 'Wrench(index:19)' carried or in room with player |
| Condition| ConditionID 1 ArgID 51| item 'Rusty closed grating(index:51)' in room with player |
| Action| ActionID 72 ArgID 51, 45| swap item locations 'Rusty closed grating(index:51)' and 'Loose grate(index:45)' |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 131 | Print message 'I can only remove 1 bolt\!' |
### Action 159 - Input: USE WREN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5781, 383, 903, 0, 0, 0, 16307, 0|  |
| Verb| 38| USE |
| Noun| 81| WREN |
| Condition| ConditionID 2 ArgID 19| item 'Wrench(index:19)' carried or in room with player |
| Condition| ConditionID 2 ArgID 45| item 'Loose grate(index:45)' carried or in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 107 | Print message 'Too hard' |
### Action 160 - GO - Input: GO WIND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 201, 1262, 0, 0, 0, 0, 16250, 0|  |
| Verb| 1| GO |
| Noun| 51| WIND |
| Condition| ConditionID 1 ArgID 63| item 'Window\. Gun pointing into & mounted by window(index:63)' in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 50 | Print message 'Its too tight' |
### Action 161 - Input: KISS MERM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9631, 104, 542, 0, 0, 0, 322, 0|  |
| Verb| 64| KISS |
| Noun| 31| MERM |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 1 ArgID 27| item 'Mermaid(index:27)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 22 | Print message 'Wheeee' |
### Action 162 - Input: GO HOLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 232, 522, 260, 80, 0, 0, 356, 8158|  |
| Verb| 1| GO |
| Noun| 82| HOLE |
| Condition| ConditionID 1 ArgID 26| item 'Dark manhole(index:26)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 54 ArgID 13| move room 13 |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 163 - Input: GET BOLT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1580, 0, 0, 0, 0, 0, 3900, 0|  |
| Verb| 10| GET |
| Noun| 80| BOLT |
| Action| ActionID 26 | Print message 'How?' |
### Action 164 - Input: REMO BOLT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3830, 0, 0, 0, 0, 0, 3900, 0|  |
| Verb| 25| REMO |
| Noun| 80| BOLT |
| Action| ActionID 26 | Print message 'How?' |
### Action 165 - Input: BREA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7200, 460, 20, 89, 0, 0, 1532, 8904|  |
| Verb| 48| BREA |
| Noun| 0| ANY |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 10 | Print message 'Bouncer throws me out' |
| Action| ActionID 32 | Print message 'For Vandalism' |
| Action| ActionID 59 ArgID 23| Item 'Ticket(index:23)' is removed from the game (put in room 0) |
| Action| ActionID 54 ArgID 1| move room 1 |
### Action 166 - Input: PULL KNOB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5298, 0, 0, 0, 0, 0, 16800, 0|  |
| Verb| 35| PULL |
| Noun| 48| KNOB |
| Action| ActionID 112 | Print message 'Say again & use a color' |
### Action 167 - Input: PRES KNOB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5448, 0, 0, 0, 0, 0, 16800, 0|  |
| Verb| 36| PRES |
| Noun| 48| KNOB |
| Action| ActionID 112 | Print message 'Say again & use a color' |
### Action 168 - Input: PRES ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5400, 0, 0, 0, 0, 0, 327, 0|  |
| Verb| 36| PRES |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 169 - Input: TOUC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 0, 0, 0, 0, 0, 327, 0|  |
| Verb| 27| TOUC |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 170 - Input: BREA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7200, 88, 0, 0, 0, 0, 3900, 0|  |
| Verb| 48| BREA |
| Noun| 0| ANY |
| Condition| ConditionID 7 ArgID 4| bitflag 4 is set |
| Action| ActionID 26 | Print message 'How?' |
### Action 171 - Input: PULL RED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5276, 222, 140, 149, 0, 0, 358, 21900|  |
| Verb| 35| PULL |
| Noun| 26| RED |
| Condition| ConditionID 1 ArgID 11| item 'Red knob in wall(index:11)' in room with player |
| Condition| ConditionID 8 ArgID 7| bitflag 7 is false |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 58 ArgID 7| set 7 flag |
| Action| ActionID 146 | Print message 'Click\!' |
### Action 172 - Input: REMO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 0, 0, 0, 0, 0, 17550, 0|  |
| Verb| 25| REMO |
| Noun| 0| ANY |
| Action| ActionID 117 | Print message 'I'm not wearing it' |
### Action 173 - Input: FIND ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12450, 0, 0, 0, 0, 0, 1050, 0|  |
| Verb| 83| FIND |
| Noun| 0| ANY |
| Action| ActionID 7 | Print message 'Tell me where to look\!' |
### Action 174 - Input: INVE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5100, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 34| INVE |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
### Action 175 - Input: SAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 0, 0, 0, 0, 0, 416, 12777|  |
| Verb| 56| SAY |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 116 | Print message 'I say:' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 176 - Input: SAVE GAME
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4395, 0, 0, 0, 0, 0, 10650, 0|  |
| Verb| 29| SAVE |
| Noun| 45| GAME |
| Action| ActionID 71 | save game |
### Action 177 - Input: QUIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4950, 0, 0, 0, 0, 0, 9450, 0|  |
| Verb| 33| QUIT |
| Noun| 0| ANY |
| Action| ActionID 63 | game over |
### Action 178 - Input: GET INVE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1544, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 10| GET |
| Noun| 44| INVE |
| Action| ActionID 66 | output inventory |
### Action 179 - Input: ON ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11100, 0, 0, 0, 0, 0, 16200, 0|  |
| Verb| 74| ON |
| Noun| 0| ANY |
| Action| ActionID 108 | Print message 'I can't do that' |
### Action 180 - Input: SCOR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10350, 0, 0, 0, 0, 0, 4050, 0|  |
| Verb| 69| SCOR |
| Noun| 0| ANY |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 181 - Input: LOOK CEIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6686, 444, 20, 0, 0, 0, 353, 11400|  |
| Verb| 44| LOOK |
| Noun| 86| CEIL |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 53 ArgID 1| drops item 'Rope hanging from ceiling(index:1)' into current room |
| Action| ActionID 76 | look |
### Action 182 - Input: GET SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1538, 1285, 0, 0, 0, 0, 3900, 0|  |
| Verb| 10| GET |
| Noun| 38| SIGN |
| Condition| ConditionID 4 ArgID 64| item 'Sign(index:64)' not in room with player |
| Action| ActionID 26 | Print message 'How?' |
### Action 183 - Input: USE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 0, 0, 0, 0, 0, 16310, 0|  |
| Verb| 38| USE |
| Noun| 0| ANY |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 110 | Print message 'Doesn't work' |
### Action 184 - Input: WEAR SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6459, 63, 80, 60, 0, 0, 374, 11100|  |
| Verb| 43| WEAR |
| Noun| 9| SHOE |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 74 ArgID 4| take item 'which I'm wearing(index:4)', no check done to see if can carry |
| Action| ActionID 74 ArgID 3| take item 'Shoes(index:3)', no check done to see if can carry |
### Action 185 - Input: LIST ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 0, 0, 0, 0, 0, 4050, 0|  |
| Verb| 31| LIST |
| Noun| 0| ANY |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 186 - . - Input: READ SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7088, 1283, 0, 0, 0, 0, 7087, 3000|  |
| Verb| 47| READ |
| Noun| 38| SIGN |
| Condition| ConditionID 2 ArgID 64| item 'Sign(index:64)' carried or in room with player |
| Action| ActionID 47 | Print message 'it says' |
| Action| ActionID 37 | Print message 'its out' |
| Action| ActionID 20 | Print message 'of order' |
### Action 187 - Input: PULL RED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5276, 962, 0, 0, 0, 0, 4050, 0|  |
| Verb| 35| PULL |
| Noun| 26| RED |
| Condition| ConditionID 1 ArgID 48| item 'Fortune telling machine(index:48)' in room with player |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 188 - Input: GET SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1538, 1282, 1280, 0, 0, 0, 7802, 0|  |
| Verb| 10| GET |
| Noun| 38| SIGN |
| Condition| ConditionID 1 ArgID 64| item 'Sign(index:64)' in room with player |
| Action| ActionID 52 ArgID 64| get item 'Sign(index:64)', check if can carry |
| Action| ActionID 2 | Print message 'OK' |
### Action 189 - Input: OPEN WALL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12052, 0, 0, 0, 0, 0, 3900, 0|  |
| Verb| 80| OPEN |
| Noun| 52| WALL |
| Action| ActionID 26 | Print message 'How?' |
### Action 190 - Input: GO SLID
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 1042, 762, 0, 0, 0, 16206, 0|  |
| Verb| 1| GO |
| Noun| 24| SLID |
| Condition| ConditionID 1 ArgID 52| item 'Bottom of slide(index:52)' in room with player |
| Condition| ConditionID 1 ArgID 38| item 'Open Drain(index:38)' in room with player |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 6 | Print message 'Too steep' |
### Action 191 - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 0, 0, 0, 0, 0, 300, 0|  |
| Verb| 66| JUMP |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
### Action 192 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12011, 1414, 44, 1400, 941, 0, 353, 0|  |
| Verb| 80| OPEN |
| Noun| 11| DOOR |
| Condition| ConditionID 13 ArgID 70| item 'Open door in glass(index:70)' not in game |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Condition| ConditionID 0 ArgID 47| item 'which I'm wearing(index:47)' carried |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 53 ArgID 70| drops item 'Open door in glass(index:70)' into current room |
### Action 193 - Input: CLOS DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7811, 1402, 1400, 0, 0, 0, 8852, 0|  |
| Verb| 52| CLOS |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 70| item 'Open door in glass(index:70)' in room with player |
| Action| ActionID 59 ArgID 70| Item 'Open door in glass(index:70)' is removed from the game (put in room 0) |
| Action| ActionID 2 | Print message 'OK' |
### Action 194 - Input: GO DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 161, 1402, 340, 80, 0, 0, 354, 11458|  |
| Verb| 1| GO |
| Noun| 11| DOOR |
| Condition| ConditionID 1 ArgID 70| item 'Open door in glass(index:70)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 17| move room 17 |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 195 - Input: WAVE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3900, 0, 0, 0, 0, 0, 327, 0|  |
| Verb| 26| WAVE |
| Noun| 0| ANY |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 27 | Print message 'Nothing happens' |
### Action 196 - Input: TURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 0, 0, 0, 0, 0, 16310, 0|  |
| Verb| 51| TURN |
| Noun| 0| ANY |
| Action| ActionID 108 | Print message 'I can't do that' |
| Action| ActionID 110 | Print message 'Doesn't work' |
### Action 197 - Input: GO PIPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 206, 662, 0, 0, 0, 0, 15444, 16200|  |
| Verb| 1| GO |
| Noun| 56| PIPE |
| Condition| ConditionID 1 ArgID 33| item 'Valve on a large warm pipe(index:33)' in room with player |
| Action| ActionID 102 | Print message 'Ouch' |
| Action| ActionID 144 | Print message 'too hot' |
| Action| ActionID 108 | Print message 'I can't do that' |
### Action 198 - Input: STAN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12750, 224, 0, 0, 0, 0, 4037, 18900|  |
| Verb| 85| STAN |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 26 | Print message 'How?' |
| Action| ActionID 137 | Print message 'I fell' |
| Action| ActionID 126 | Print message 'flat on my face\!' |
### Action 199 - Input: COMB ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9300, 542, 563, 1180, 1040, 0, 10819, 0|  |
| Verb| 62| COMB |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 27| item 'Mermaid(index:27)' in room with player |
| Condition| ConditionID 2 ArgID 28| item 'Comb(index:28)' carried or in room with player |
| Action| ActionID 72 ArgID 59, 52| swap item locations 'Bottom of stairs(index:59)' and 'Bottom of slide(index:52)' |
| Action| ActionID 19 | Print message 'She thanks me & turns a hidden knob' |
### Action 200 - Input: GO LADD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 177, 282, 320, 80, 0, 0, 8176, 6958|  |
| Verb| 1| GO |
| Noun| 27| LADD |
| Condition| ConditionID 1 ArgID 14| item 'Ladder going down(index:14)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 76 | look |
| Action| ActionID 46 | Print message 'Fire ladder retracts and leaves me here\!' |
| Action| ActionID 58 ArgID 4| set 4 flag |
### Action 201 - Input: KISS LADY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9685, 24, 0, 0, 0, 0, 322, 0|  |
| Verb| 64| KISS |
| Noun| 85| LADY |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 22 | Print message 'Wheeee' |
### Action 202 - Input: GO HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 186, 822, 140, 0, 0, 0, 354, 11400|  |
| Verb| 1| GO |
| Noun| 36| HORS |
| Condition| ConditionID 1 ArgID 41| item 'Wooden horse(index:41)' in room with player |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 54 ArgID 7| move room 7 |
| Action| ActionID 76 | look |
### Action 203 - Input: LOOK CEIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6686, 424, 0, 0, 0, 0, 21750, 0|  |
| Verb| 44| LOOK |
| Noun| 86| CEIL |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 145 | Print message 'There's a catwalk above the ride' |
### Action 204 - Input: LOOK UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6605, 424, 0, 0, 0, 0, 21750, 0|  |
| Verb| 44| LOOK |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 145 | Print message 'There's a catwalk above the ride' |
### Action 205 - Input: LOOK ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6600, 0, 0, 0, 0, 0, 11451, 0|  |
| Verb| 44| LOOK |
| Noun| 0| ANY |
| Action| ActionID 76 | look |
| Action| ActionID 51 | Print message 'I see nothing special\.' |
### Action 206 - Input: GO HOLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 232, 842, 1202, 680, 0, 0, 8102, 11400|  |
| Verb| 1| GO |
| Noun| 82| HOLE |
| Condition| ConditionID 1 ArgID 42| item 'Dark hole(index:42)' in room with player |
| Condition| ConditionID 1 ArgID 60| item 'Broken grate(index:60)' in room with player |
| Action| ActionID 54 ArgID 34| move room 34 |
| Action| ActionID 2 | Print message 'OK' |
| Action| ActionID 76 | look |
### Action 207 - Input: FIX SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12909, 63, 0, 0, 0, 0, 300, 0|  |
| Verb| 86| FIX |
| Noun| 9| SHOE |
| Condition| ConditionID 2 ArgID 3| item 'Shoes(index:3)' carried or in room with player |
| Action| ActionID 2 | Print message 'OK' |
### Action 208 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 209 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 211 - Take for item Shoes - Input: GET SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 9| SHOE |
| Condition| ConditionID 1 ArgID 3| item 'Shoes(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Shoes(index:3)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 212 - Drop for item Shoes - Input: DROP SHOE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 9| SHOE |
| Condition| ConditionID 0 ArgID 3| item 'Shoes(index:3)' carried |
| Action| ActionID 53 ArgID 3| drops item 'Shoes(index:3)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 213 - Take for item Lit Flashlight - Input: GET FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 8| FLAS |
| Condition| ConditionID 1 ArgID 9| item 'Lit Flashlight(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Lit Flashlight(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 214 - Drop for item Lit Flashlight - Input: DROP FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 8| FLAS |
| Condition| ConditionID 0 ArgID 9| item 'Lit Flashlight(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Lit Flashlight(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 215 - Take for item Small Trampoline - Input: GET TRAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 15| TRAM |
| Condition| ConditionID 1 ArgID 18| item 'Small Trampoline(index:18)' in room with player |
| Action| ActionID 52 ArgID 18| get item 'Small Trampoline(index:18)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 216 - Drop for item Small Trampoline - Input: DROP TRAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 15| TRAM |
| Condition| ConditionID 0 ArgID 18| item 'Small Trampoline(index:18)' carried |
| Action| ActionID 53 ArgID 18| drops item 'Small Trampoline(index:18)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 217 - Take for item Wrench - Input: GET WREN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 81| WREN |
| Condition| ConditionID 1 ArgID 19| item 'Wrench(index:19)' in room with player |
| Action| ActionID 52 ArgID 19| get item 'Wrench(index:19)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 218 - Drop for item Wrench - Input: DROP WREN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 81| WREN |
| Condition| ConditionID 0 ArgID 19| item 'Wrench(index:19)' carried |
| Action| ActionID 53 ArgID 19| drops item 'Wrench(index:19)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 219 - Take for item Ticket - Input: GET TICK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 35| TICK |
| Condition| ConditionID 1 ArgID 23| item 'Ticket(index:23)' in room with player |
| Action| ActionID 52 ArgID 23| get item 'Ticket(index:23)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 220 - Drop for item Ticket - Input: DROP TICK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 35| TICK |
| Condition| ConditionID 0 ArgID 23| item 'Ticket(index:23)' carried |
| Action| ActionID 53 ArgID 23| drops item 'Ticket(index:23)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 221 - Take for item Bottom of heel - Input: GET HEEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 37| HEEL |
| Condition| ConditionID 1 ArgID 24| item 'Bottom of heel(index:24)' in room with player |
| Action| ActionID 52 ArgID 24| get item 'Bottom of heel(index:24)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 222 - Drop for item Bottom of heel - Input: DROP HEEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 37| HEEL |
| Condition| ConditionID 0 ArgID 24| item 'Bottom of heel(index:24)' carried |
| Action| ActionID 53 ArgID 24| drops item 'Bottom of heel(index:24)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 223 - Take for item Watch - Input: GET WATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 40| WATC |
| Condition| ConditionID 1 ArgID 25| item 'Watch(index:25)' in room with player |
| Action| ActionID 52 ArgID 25| get item 'Watch(index:25)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 224 - Drop for item Watch - Input: DROP WATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 40| WATC |
| Condition| ConditionID 0 ArgID 25| item 'Watch(index:25)' carried |
| Action| ActionID 53 ArgID 25| drops item 'Watch(index:25)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 225 - Take for item Comb - Input: GET COMB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 39| COMB |
| Condition| ConditionID 1 ArgID 28| item 'Comb(index:28)' in room with player |
| Action| ActionID 52 ArgID 28| get item 'Comb(index:28)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 226 - Drop for item Comb - Input: DROP COMB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 39| COMB |
| Condition| ConditionID 0 ArgID 28| item 'Comb(index:28)' carried |
| Action| ActionID 53 ArgID 28| drops item 'Comb(index:28)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 227 - Take for item Rusty key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 30| KEY |
| Condition| ConditionID 1 ArgID 30| item 'Rusty key(index:30)' in room with player |
| Action| ActionID 52 ArgID 30| get item 'Rusty key(index:30)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 228 - Drop for item Rusty key - Input: DROP KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 30| KEY |
| Condition| ConditionID 0 ArgID 30| item 'Rusty key(index:30)' carried |
| Action| ActionID 53 ArgID 30| drops item 'Rusty key(index:30)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 229 - Take for item Valve handle with no valve - Input: GET HAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 77| HAND |
| Condition| ConditionID 1 ArgID 35| item 'Valve handle with no valve(index:35)' in room with player |
| Action| ActionID 52 ArgID 35| get item 'Valve handle with no valve(index:35)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 230 - Drop for item Valve handle with no valve - Input: DROP HAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 77| HAND |
| Condition| ConditionID 0 ArgID 35| item 'Valve handle with no valve(index:35)' carried |
| Action| ActionID 53 ArgID 35| drops item 'Valve handle with no valve(index:35)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 231 - Take for item Short fuse - Input: GET FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 78| FUSE |
| Condition| ConditionID 1 ArgID 36| item 'Short fuse(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Short fuse(index:36)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 232 - Drop for item Short fuse - Input: DROP FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 78| FUSE |
| Condition| ConditionID 0 ArgID 36| item 'Short fuse(index:36)' carried |
| Action| ActionID 53 ArgID 36| drops item 'Short fuse(index:36)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 233 - Take for item Letter - Input: GET LETT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 66| LETT |
| Condition| ConditionID 1 ArgID 39| item 'Letter(index:39)' in room with player |
| Action| ActionID 52 ArgID 39| get item 'Letter(index:39)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 234 - Drop for item Letter - Input: DROP LETT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 66| LETT |
| Condition| ConditionID 0 ArgID 39| item 'Letter(index:39)' carried |
| Action| ActionID 53 ArgID 39| drops item 'Letter(index:39)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 235 - Take for item Pile of bones - Input: GET BONE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 53| BONE |
| Condition| ConditionID 1 ArgID 44| item 'Pile of bones(index:44)' in room with player |
| Action| ActionID 52 ArgID 44| get item 'Pile of bones(index:44)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 236 - Drop for item Pile of bones - Input: DROP BONE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 53| BONE |
| Condition| ConditionID 0 ArgID 44| item 'Pile of bones(index:44)' carried |
| Action| ActionID 53 ArgID 44| drops item 'Pile of bones(index:44)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 237 - Take for item Strange spectacles - Input: GET SPEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 43| SPEC |
| Condition| ConditionID 1 ArgID 46| item 'Strange spectacles(index:46)' in room with player |
| Action| ActionID 52 ArgID 46| get item 'Strange spectacles(index:46)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 238 - Drop for item Strange spectacles - Input: DROP SPEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 43| SPEC |
| Condition| ConditionID 0 ArgID 46| item 'Strange spectacles(index:46)' carried |
| Action| ActionID 53 ArgID 46| drops item 'Strange spectacles(index:46)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 239 - Take for item Silver Dollar - Input: GET DOLL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 60| DOLL |
| Condition| ConditionID 1 ArgID 54| item 'Silver Dollar(index:54)' in room with player |
| Action| ActionID 52 ArgID 54| get item 'Silver Dollar(index:54)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 240 - Drop for item Silver Dollar - Input: DROP DOLL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 60| DOLL |
| Condition| ConditionID 0 ArgID 54| item 'Silver Dollar(index:54)' carried |
| Action| ActionID 53 ArgID 54| drops item 'Silver Dollar(index:54)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 241 - Take for item Broken branch - Input: GET BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 55| item 'Broken branch(index:55)' in room with player |
| Action| ActionID 52 ArgID 55| get item 'Broken branch(index:55)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 242 - Drop for item Broken branch - Input: DROP BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 57| BRAN |
| Condition| ConditionID 0 ArgID 55| item 'Broken branch(index:55)' carried |
| Action| ActionID 53 ArgID 55| drops item 'Broken branch(index:55)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 243 - Take for item Hard dry chewing gum - Input: GET GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 59| GUM |
| Condition| ConditionID 1 ArgID 56| item 'Hard dry chewing gum(index:56)' in room with player |
| Action| ActionID 52 ArgID 56| get item 'Hard dry chewing gum(index:56)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 244 - Drop for item Hard dry chewing gum - Input: DROP GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 56| item 'Hard dry chewing gum(index:56)' carried |
| Action| ActionID 53 ArgID 56| drops item 'Hard dry chewing gum(index:56)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 245 - Take for item Soft chewing gum - Input: GET GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 59| GUM |
| Condition| ConditionID 1 ArgID 57| item 'Soft chewing gum(index:57)' in room with player |
| Action| ActionID 52 ArgID 57| get item 'Soft chewing gum(index:57)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 246 - Drop for item Soft chewing gum - Input: DROP GUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 59| GUM |
| Condition| ConditionID 0 ArgID 57| item 'Soft chewing gum(index:57)' carried |
| Action| ActionID 53 ArgID 57| drops item 'Soft chewing gum(index:57)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 247 - Take for item Stick with gum on end - Input: GET BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 57| BRAN |
| Condition| ConditionID 1 ArgID 58| item 'Stick with gum on end(index:58)' in room with player |
| Action| ActionID 52 ArgID 58| get item 'Stick with gum on end(index:58)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 248 - Drop for item Stick with gum on end - Input: DROP BRAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 57| BRAN |
| Condition| ConditionID 0 ArgID 58| item 'Stick with gum on end(index:58)' carried |
| Action| ActionID 53 ArgID 58| drops item 'Stick with gum on end(index:58)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 249 - Take for item Sign - Input: GET SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 38| SIGN |
| Condition| ConditionID 1 ArgID 64| item 'Sign(index:64)' in room with player |
| Action| ActionID 52 ArgID 64| get item 'Sign(index:64)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 250 - Drop for item Sign - Input: DROP SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 38| SIGN |
| Condition| ConditionID 0 ArgID 64| item 'Sign(index:64)' carried |
| Action| ActionID 53 ArgID 64| drops item 'Sign(index:64)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 251 - Take for item Flashlight - Input: GET FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 8| FLAS |
| Condition| ConditionID 1 ArgID 66| item 'Flashlight(index:66)' in room with player |
| Action| ActionID 52 ArgID 66| get item 'Flashlight(index:66)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 252 - Drop for item Flashlight - Input: DROP FLAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 8| FLAS |
| Condition| ConditionID 0 ArgID 66| item 'Flashlight(index:66)' carried |
| Action| ActionID 53 ArgID 66| drops item 'Flashlight(index:66)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 253 - Take for item Missing top secret plans - Input: GET PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 25| PLAN |
| Condition| ConditionID 1 ArgID 67| item 'Missing top secret plans(index:67)' in room with player |
| Action| ActionID 52 ArgID 67| get item 'Missing top secret plans(index:67)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 254 - Drop for item Missing top secret plans - Input: DROP PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 25| PLAN |
| Condition| ConditionID 0 ArgID 67| item 'Missing top secret plans(index:67)' carried |
| Action| ActionID 53 ArgID 67| drops item 'Missing top secret plans(index:67)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 255 - Take for item 5 Dollar Bill - Input: GET BILL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 41| BILL |
| Condition| ConditionID 1 ArgID 68| item '5 Dollar Bill(index:68)' in room with player |
| Action| ActionID 52 ArgID 68| get item '5 Dollar Bill(index:68)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 256 - Drop for item 5 Dollar Bill - Input: DROP BILL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 41| BILL |
| Condition| ConditionID 0 ArgID 68| item '5 Dollar Bill(index:68)' carried |
| Action| ActionID 53 ArgID 68| drops item '5 Dollar Bill(index:68)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 257 - Take for item Match - Input: GET MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 54| MATC |
| Condition| ConditionID 1 ArgID 69| item 'Match(index:69)' in room with player |
| Action| ActionID 52 ArgID 69| get item 'Match(index:69)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 258 - Drop for item Match - Input: DROP MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 54| MATC |
| Condition| ConditionID 0 ArgID 69| item 'Match(index:69)' carried |
| Action| ActionID 53 ArgID 69| drops item 'Match(index:69)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 259 - Take for item Soggy fuse - Input: GET FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 78| FUSE |
| Condition| ConditionID 1 ArgID 74| item 'Soggy fuse(index:74)' in room with player |
| Action| ActionID 52 ArgID 74| get item 'Soggy fuse(index:74)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 260 - Drop for item Soggy fuse - Input: DROP FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 78| FUSE |
| Condition| ConditionID 0 ArgID 74| item 'Soggy fuse(index:74)' carried |
| Action| ActionID 53 ArgID 74| drops item 'Soggy fuse(index:74)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 261 - Manually added load game action - Input: LOAD GAME
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 92| LOAD |
| Noun| 45| GAME |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUTO| 0|  |
| GO| 1| WALK, ., RUN, ENTE, MOUN, CLIM, ., RIDE |
| GET| 10| GRAB, TAKE, CATC, PICK |
| GUM| 15|  |
| SHOO| 16| FIRE |
| DROP| 18| PUT, LEAV, GIVE, PAY |
| BLOW| 23| MAKE |
| REMO| 25|  |
| WAVE| 26|  |
| TOUC| 27| FEEL |
| SAVE| 29|  |
| HELP| 30|  |
| LIST| 31| HEAR |
| QUIT| 33|  |
| INVE| 34|  |
| PULL| 35|  |
| PRES| 36| PUSH |
| USE| 38| WITH |
| LIGH| 40| IGNI |
| STIC| 42|  |
| WEAR| 43|  |
| LOOK| 44| EXAM, DESC |
| READ| 47|  |
| BREA| 48| HIT |
| SWIM| 50|  |
| TURN| 51|  |
| CLOS| 52| SHUT |
| EAT| 54|  |
| CHEW| 55|  |
| SAY| 56| YELL, SCRE, ASK, BUY |
| UNLI| 61|  |
| COMB| 62|  |
| CUT| 63|  |
| KISS| 64| RAPE |
| JUMP| 66| BOUN |
| \.| 68|  |
| SCOR| 69|  |
| CHAS| 70|  |
| MOVE| 71| SLID, ROTA |
| ON| 74| TO |
| CRAW| 76| ROLL |
| \.| 78|  |
| DANC| 79|  |
| OPEN| 80| UNLO, UNTI |
| FIND| 83| LOCA |
| STAN| 85|  |
| FIX| 86| REPA |
| | 88|  |
| | 89|  |
| LOAD| 92|  |
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
| ROPE| 7|  |
| FLAS| 8|  |
| SHOE| 9|  |
| MIRR| 10|  |
| DOOR| 11|  |
| SKEL| 12|  |
| POLE| 13|  |
| TUNN| 14|  |
| TRAM| 15|  |
| EXIT| 16|  |
| CHAR| 17|  |
| BACK| 18|  |
| GREE| 19|  |
| YELL| 20|  |
| BLUE| 21|  |
| FORT| 22|  |
| AROU| 23|  |
| SLID| 24|  |
| PLAN| 25|  |
| RED| 26|  |
| LADD| 27|  |
| MUSI| 28|  |
| TANK| 29|  |
| KEY| 30|  |
| MERM| 31|  |
| STAI| 32|  |
| MACH| 33|  |
| ROOM| 34|  |
| TICK| 35|  |
| HORS| 36|  |
| HEEL| 37|  |
| SIGN| 38|  |
| COMB| 39|  |
| WATC| 40|  |
| BILL| 41|  |
| DRAI| 42|  |
| SPEC| 43|  |
| INVE| 44|  |
| GAME| 45|  |
| HEMP| 46|  |
| GRAT| 47|  |
| KNOB| 48| BUTT |
| COUN| 50|  |
| WIND| 51|  |
| WALL| 52|  |
| BONE| 53|  |
| MATC| 54|  |
| HELP| 55|  |
| PIPE| 56|  |
| BRAN| 57| STIC |
| GUM| 59|  |
| DOLL| 60| COIN |
| GUN| 62|  |
| TREE| 63|  |
| SHEL| 64|  |
| HAIR| 65|  |
| LETT| 66|  |
| OFF| 67|  |
| FUN| 68| HOUS, PARK |
| BOUN| 71|  |
| BUBB| 72|  |
| CALL| 73|  |
| STEA| 74|  |
| MERR| 75|  |
| VALV| 76|  |
| HAND| 77|  |
| FUSE| 78|  |
| BARR| 79|  |
| BOLT| 80|  |
| WREN| 81|  |
| HOLE| 82| MAN, MANH |
| LADY| 85|  |
| CEIL| 86| CATW |
| LOCK| 88|  |
| PIGE| 89|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| \*I'm in front of the FUN HOUSE| East: 26 |
| 2| Magical Mirror Room| North: 30, South: 1 |
| 3| \*I'm on a small landing| North: 9, East: 19, Up: 20 |
| 4| \*I'm beside a LARGE tank| East: 10, Up: 9 |
| 5| windowed tank|  |
| 6| hidden laboratory| North: 25 |
| 7| Merry\-Go\-Round on a wooden horse| Down: 18 |
| 8| small room| South: 14, Up: 10 |
| 9| sloping hallway| Up: 3, Down: 4 |
| 10| room with a low ceiling| West: 4 |
| 11| large rolling barrel room|  |
| 12| store room| West: 33 |
| 13| Manhole| East: 28, Up: 26 |
| 14| shooting gallery| North: 8 |
| 15| \*I'm on a ledge over a deep pit| South: 20, East: 11 |
| 16| Pit|  |
| 17| Observation chamber| East: 2 |
| 18| \*I'm on a Merry\-Go\-Round| Down: 21 |
| 19| Windy hall| East: 30, West: 3 |
| 20| rickety staircase| Up: 15, Down: 3 |
| 21| large room with tall ceiling| South: 23 |
| 22| \*I'm on top of the ride| Down: 7 |
| 23| small room| East: 21, Down: 10 |
| 24| small room| North: 32, West: 10 |
| 25| large room| South: 6, Down: 34 |
| 26| Parking lot| West: 1 |
| 27| \*I'm on a Trampoline|  |
| 28| Sewer system|  |
| 29| windy maze| North: 31, South: 30, East: 32, West: 24 |
| 30| windy maze| North: 32, South: 31, East: 2, West: 31 |
| 31| windy maze| North: 32, South: 31, East: 29, West: 29 |
| 32| windy maze| North: 31, South: 29, East: 31, West: 32 |
| 33| catwalk| East: 12, Down: 22 |
| 34| long tunnel| Up: 25, Down: 28 |
| 35| Lot of TROUBLE\!|  |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| Good thing this ropes not too long |
| 2| OK |
| 3| I see a bunch of clay pigeons |
| 4| Splash, Oh no I am all washed up\! |
| 5| Ticket lady rips up bill & says `$5 grocery bill ain't money bub\!` |
| 6| Too steep |
| 7| Tell me where to look\! |
| 8| I see a hidden door in it |
| 9| I've no match\! |
| 10| Bouncer throws me out |
| 11| Park closes at midnight\. Shoes required at all times\. Management NOT responsible for accidents\!\! CAUTION this park is DANGERous\!  |
| 12| I can see myself thin,fat & tall |
| 13| There's strange music playing |
| 14| Sounds like a space opera |
| 15| till midnight |
| 16| The park is closing in |
| 17| turns |
| 18| Welcome to ADVENTURE 7, `MYSTERY FUN HOUSE` by Scott Adams Dedicated to Marin Computer Center\. |
| 19| She thanks me & turns a hidden knob |
| 20| of order |
| 21| She's pretty, but has really snarled hair\! |
| 22| Wheeee |
| 23| She's too fast for me |
| 24| Not here\! |
| 25| I am |
| 26| How? |
| 27| Nothing happens |
| 28| A mermaid swims by and waves |
| 29| \. |
| 30| Someone shot me\! |
| 31| All the water ran out |
| 32| For Vandalism |
| 33| Something dropped out |
| 34| On what? |
| 35| At What? |
| 36| Sizzle, it burns with a dull glow\. |
| 37| its out |
| 38| I was holding it\! |
| 39| Try: `STICK GUM` |
| 40| I shot a clay pigeon\! |
| 41| It collapsed into a pile of bones |
| 42| Calliope is so LOUD I can't hear clearly\! |
| 43| starts\. |
| 44| Tiny piece of hemp falls on my head and vanishes\! |
| 45| Tastes HORRIBLE\! |
| 46| Fire ladder retracts and leaves me here\! |
| 47| it says |
| 48| Ticket lady asks me what I want |
| 49| She hands me a ticket |
| 50| Its too tight |
| 51| I see nothing special\. |
| 52| Ouch |
| 53| She says: `That'll be a dollar` |
| 54| I see a shiny COIN at the bottom of the drain\! |
| 55| I can't reach it, my arm is too short\! |
| 56| Got it\! |
| 57| Too hard |
| 58| I can't do that |
| 59| Only thing left is one bare branch |
| 60| Doesn't work |
| 61| I just push it around |
| 62| Say again & use a color |
| 63| Wall swings me around & I'm elsewhere\.\.\. |
| 64| James: We must get the plans back by tonight\! We believe they're hiddenwithin his Fun House\!  Signed, M P\.S\. Q says enjoy the gum\! |
| 65| Try EXAMINING things\! |
| 66| I say: |
| 67| I'm not wearing it |
| 68| POP |
| 69| HUH? Why do you want me to MARRY? |
| 70| There's no handle on it |
| 71| My shoe heel is loose |
| 72| Something fell out |
| 73| AUTHORIZED PERSONNEL ONLY\! |
| 74| Guard hears explosion & shoots me\! |
| 75| Flashlight there |
| 76| flat on my face\! |
| 77| Ride |
| 78| stops\. |
| 79| There's a red button |
| 80| big bolts hold it down |
| 81| I can only remove 1 bolt\! |
| 82| 1 |
| 83| 2 |
| 84| Wall closed behind me |
| 85| Too high for me |
| 86| Moving ride throws me off balance |
| 87| I fell |
| 88| Gentle air blast blows up my leg\. |
| 89| Hard blast of air rips my body apart |
| 90| Machine lights up and says |
| 91| HURRAH\! You've done it\! |
| 92| I see into the mirror room |
| 93| not on it |
| 94| too hot |
| 95| There's a catwalk above the ride |
| 96| Click\! |
| 97|  |
| 98|  |
| 99|  |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Closed drain\. Water| | 5 |
| 1| Rope hanging from ceiling| | 0 |
| 2| Strange Mirror| | 2 |
| 3| Shoes| SHOE| -1 |
| 4| which I'm wearing| | 0 |
| 5| Slippery Slide\. Sign on slide| | 3 |
| 6| Locked door| | 6 |
| 7| Skeleton| | 10 |
| 8| Locked door| | 12 |
| 9| Lit Flashlight| FLAS| 0 |
| 10| Open flood door| | 28 |
| 11| Red knob in wall| | 12 |
| 12| Strange knobs on wall: Yellow, Green, Blue| | 10 |
| 13| Closed flood door| | 0 |
| 14| Ladder going down| | 15 |
| 15| Locked door| | 16 |
| 16| Open door with small shelves beyond| | 0 |
| 17| Sign on ladder| | 15 |
| 18| Small Trampoline| TRAM| 8 |
| 19| Wrench| WREN| 12 |
| 20| Locked door| | 33 |
| 21| Sign| | 1 |
| 22| Ticket Counter| | 1 |
| 23| Ticket| TICK| 0 |
| 24| Bottom of heel| HEEL| 0 |
| 25| Watch| WATC| -1 |
| 26| Dark manhole| | 0 |
| 27| Mermaid| | 5 |
| 28| Comb| COMB| 11 |
| 29| Quiet Calliope| | 0 |
| 30| Rusty key| KEY| 5 |
| 31| LOUD Steam Calliope| | 21 |
| 32| Merry\-Go\-Round| | 21 |
| 33| Valve on a large warm pipe| | 16 |
| 34| Handle is on valve| | 34 |
| 35| Valve handle with no valve| HAND| 17 |
| 36| Short fuse| FUSE| 0 |
| 37| Fuse is stuck in gum| | 0 |
| 38| Open Drain| | 0 |
| 39| Letter| LETT| 0 |
| 40| Exit| | 11 |
| 41| Wooden horse| | 18 |
| 42| Dark hole| | 28 |
| 43| Large grate welded over hole| | 28 |
| 44| Pile of bones| BONE| 0 |
| 45| Loose grate| | 0 |
| 46| Strange spectacles| SPEC| 14 |
| 47| which I'm wearing| | 0 |
| 48| Fortune telling machine| | 23 |
| 49| Rope hanging down| | 33 |
| 50| Gum is stuck to grate| | 0 |
| 51| Rusty closed grating| | 26 |
| 52| Bottom of slide| | 5 |
| 53| Dead tree| | 26 |
| 54| Silver Dollar| DOLL| 0 |
| 55| Broken branch| BRAN| 0 |
| 56| Hard dry chewing gum| GUM| -1 |
| 57| Soft chewing gum| GUM| 0 |
| 58| Stick with gum on end| BRAN| 0 |
| 59| Bottom of stairs| | 0 |
| 60| Broken grate| | 0 |
| 61| Pole coming out of horse's back| | 7 |
| 62| Window in tank| | 4 |
| 63| Window\. Gun pointing into & mounted by window| | 14 |
| 64| Sign| SIGN| 23 |
| 65| Clay pigeons| | 25 |
| 66| Flashlight| FLAS| 0 |
| 67| Missing top secret plans| PLAN| 6 |
| 68| 5 Dollar Bill| BILL| 26 |
| 69| Match| MATC| 11 |
| 70| Open door in glass| | 0 |
| 71| 1 way mirror| | 17 |
| 72| Locked door| | 17 |
| 73| Blue button| | 21 |
| 74| Soggy fuse| FUSE| 0 |