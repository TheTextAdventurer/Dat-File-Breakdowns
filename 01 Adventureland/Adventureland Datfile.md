# 1. Adventureland
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
| adventureNumber| 1 |
| Unknown| 5953 |
| numItems| 66 |
| numActions| 170 |
| numNounVerbs| 70 |
| numRooms| 34 |
| maxCarry| 6 |
| startRoom| 11 |
| totalTreasures| 13 |
| wordLength| 3 |
| lightDuration| 125 |
| numMessages| 76 |
| treasureRoom| 3 |
## Actions
### Action 0 - FISH ESCAPE - Probability: 75 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 75, 161, 386, 160, 200, 0, 17612, 0|  |
| Probability| 75%|  |
| Condition| ConditionID 0 ArgID 8| item '\*GOLDEN FISH\*(index:8)' carried |
| Condition| ConditionID 5 ArgID 19| item '\*GOLDEN NET\*(index:19)' not carried |
| Action| ActionID 117 | Print message 'Fish have escaped back to the lake\.' |
| Action| ActionID 62 ArgID 8, 10| item '*GOLDEN FISH*(index:8)' is moved to room 10 |
### Action 1 - DIE BITES - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 421, 667, 0, 0, 0, 2011, 0|  |
| Probability| 10%|  |
| Condition| ConditionID 0 ArgID 21| item 'Infected chigger bites(index:21)' carried |
| Condition| ConditionID 6 ArgID 33| player not in room 33 |
| Action| ActionID 13 | Print message 'My bites have rotted my whole body\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 2 - BITE INFECT - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 401, 420, 400, 146, 0, 1874, 8850|  |
| Probability| 10%|  |
| Condition| ConditionID 0 ArgID 20| item 'Chigger bites(index:20)' carried |
| Condition| ConditionID 5 ArgID 7| item 'Evil smelling mud(index:7)' not carried |
| Action| ActionID 12 | Print message ' My chigger bites are now INFECTED\! ' |
| Action| ActionID 74 ArgID 21| take item 'Infected chigger bites(index:21)', no check done to see if can carry |
| Action| ActionID 59 ArgID 20| Item 'Chigger bites(index:20)' is removed from the game (put in room 0) |
### Action 3 - BEES DIE - Probability: 8 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8, 523, 520, 260, 349, 0, 2622, 0|  |
| Probability| 8%|  |
| Condition| ConditionID 2 ArgID 26| item 'Bees in a bottle(index:26)' carried or in room with player |
| Condition| ConditionID 8 ArgID 17| bitflag 17 is false |
| Action| ActionID 17 | Print message 'The bees all suffocated and disappeared' |
| Action| ActionID 72 ArgID 26, 13| swap item locations 'Bees in a bottle(index:26)' and 'Empty bottle(index:13)' |
### Action 4 - HIT MIRROR - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 108, 760, 820, 420, 100, 8312, 9064|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 5| bitflag 5 is set |
| Action| ActionID 55 ArgID 38| Item '*MAGIC MIRROR*(index:38)' is removed from the game (put in room 0) |
| Action| ActionID 62 ArgID 41, 21| item 'Broken glass(index:41)' is moved to room 21 |
| Action| ActionID 60 ArgID 5| set 5 flag |
| Action| ActionID 64 | look |
### Action 5 - IN HADES - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 484, 0, 0, 0, 0, 5613, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Action| ActionID 37 | Print message 'You lost \*ALL\* treasures\.' |
| Action| ActionID 63 | game over |
### Action 6 - MUD OFF - Probability: 5 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5, 141, 140, 20, 246, 0, 6062, 0|  |
| Probability| 5%|  |
| Condition| ConditionID 0 ArgID 7| item 'Evil smelling mud(index:7)' carried |
| Condition| ConditionID 5 ArgID 12| item 'Water in bottle(index:12)' not carried |
| Action| ActionID 40 | Print message 'The mud dried up and fell off\.' |
| Action| ActionID 62 ArgID 7, 1| item 'Evil smelling mud(index:7)' is moved to room 1 |
### Action 7 - BIT CHIG - Probability: 8 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8, 406, 426, 400, 842, 146, 11145, 0|  |
| Probability| 8%|  |
| Condition| ConditionID 5 ArgID 20| item 'Chigger bites(index:20)' not carried |
| Condition| ConditionID 5 ArgID 21| item 'Infected chigger bites(index:21)' not carried |
| Condition| ConditionID 1 ArgID 42| item 'Chiggers(index:42)' in room with player |
| Condition| ConditionID 5 ArgID 7| item 'Evil smelling mud(index:7)' not carried |
| Action| ActionID 74 ArgID 20| take item 'Chigger bites(index:20)', no check done to see if can carry |
| Action| ActionID 45 | Print message ' I'm bitten by chiggers\. ' |
### Action 8 - BEE STING - Probability: 8 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8, 482, 152, 0, 0, 0, 2311, 0|  |
| Probability| 8%|  |
| Condition| ConditionID 1 ArgID 24| item 'Large african bees(index:24)' in room with player |
| Condition| ConditionID 11 ArgID 7| item 'Evil smelling mud(index:7)' not carried or in room with player |
| Action| ActionID 15 | Print message 'Bees sting me' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 9 - LITE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 104, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 10 - FISH DIE - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 161, 246, 160, 1100, 0, 7259, 7800|  |
| Probability| 50%|  |
| Condition| ConditionID 0 ArgID 8| item '\*GOLDEN FISH\*(index:8)' carried |
| Condition| ConditionID 5 ArgID 12| item 'Water in bottle(index:12)' not carried |
| Action| ActionID 48 | Print message 'Too dry, the fish died\.' |
| Action| ActionID 59 ArgID 8| Item '*GOLDEN FISH*(index:8)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 55| get item 'Dead fish(index:55)', check if can carry |
### Action 11 - MOVE OX - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 148, 140, 940, 500, 0, 9062, 9900|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 7| bitflag 7 is set |
| Action| ActionID 60 ArgID 7| set 7 flag |
| Action| ActionID 62 ArgID 47, 25| item '*Small statue of a BLUE OX*(index:47)' is moved to room 25 |
| Action| ActionID 66 | output inventory |
### Action 12 - GET CHIG - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 841, 426, 406, 400, 146, 11145, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 0 ArgID 42| item 'Chiggers(index:42)' carried |
| Condition| ConditionID 5 ArgID 21| item 'Infected chigger bites(index:21)' not carried |
| Condition| ConditionID 5 ArgID 20| item 'Chigger bites(index:20)' not carried |
| Condition| ConditionID 5 ArgID 7| item 'Evil smelling mud(index:7)' not carried |
| Action| ActionID 74 ArgID 20| take item 'Chigger bites(index:20)', no check done to see if can carry |
| Action| ActionID 45 | Print message ' I'm bitten by chiggers\. ' |
### Action 13 - MUD DRAGON - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 542, 143, 0, 0, 0, 10504, 9150|  |
| Probability| 50%|  |
| Condition| ConditionID 1 ArgID 27| item 'Large sleeping dragon(index:27)' in room with player |
| Condition| ConditionID 2 ArgID 7| item 'Evil smelling mud(index:7)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 4 | Print message 'Dragon smells something\. Awakens & attacks me\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 14 - BLAST WALL - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 248, 642, 720, 640, 700, 8005, 7950|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Condition| ConditionID 1 ArgID 32| item 'Bricked up window(index:32)' in room with player |
| Action| ActionID 53 ArgID 36| drops item 'Loose fire bricks(index:36)' into current room |
| Action| ActionID 55 ArgID 32| Item 'Bricked up window(index:32)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 35| drops item 'Bricked up window with a hole in it(index:35)' into current room |
### Action 15 - BLAS DRAGON - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 248, 542, 1040, 540, 0, 8005, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Condition| ConditionID 1 ArgID 27| item 'Large sleeping dragon(index:27)' in room with player |
| Action| ActionID 53 ArgID 52| drops item 'Smoking hole. pieces of dragon and gore.(index:52)' into current room |
| Action| ActionID 55 ArgID 27| Item 'Large sleeping dragon(index:27)' is removed from the game (put in room 0) |
### Action 16 - 1ST MIRROR CLUE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 49, 20, 40, 0, 6360, 8700|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 8 ArgID 2| bitflag 2 is false |
| Action| ActionID 42 | Print message '` DRAGON STING ` and fades\. I don't get it, I hope you do\.' |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 58 ArgID 2| set 2 flag |
### Action 17 - BEAR MAD - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 288, 260, 280, 0, 0, 11160, 9150|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 14| bitflag 14 is set |
| Action| ActionID 74 ArgID 13| take item 'Empty bottle(index:13)', no check done to see if can carry |
| Action| ActionID 60 ArgID 14| set 14 flag |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 18 - RESET BLAST - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 248, 240, 0, 0, 0, 9660, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Action| ActionID 64 | look |
| Action| ActionID 60 ArgID 12| set 12 flag |
### Action 19 - INTRO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 269, 260, 0, 0, 0, 16558, 17357|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 58 ArgID 13| set 13 flag |
| Action| ActionID 115 | Print message ' Welcome to Adventure number: 1 `ADVENTURELAND`\. In this Adventure you're to find \*TREASURES\* & store them away\.  To see how well you're doing say: `SCORE`' |
| Action| ActionID 107 | Print message 'Remember you can always say `HELP`' |
### Action 20 - 2ND MIRROR CLUE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 48, 20, 40, 0, 4110, 9000|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Action| ActionID 27 | Print message '`Don't waste honey, get mad instead\! Dam lava\!?`' |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 60 ArgID 2| set 2 flag |
### Action 21 - DEAD LAMP - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 320, 328, 1200, 180, 0, 9072, 11400|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 16| bitflag 16 is set |
| Action| ActionID 60 ArgID 16| set 16 flag |
| Action| ActionID 72 ArgID 60, 9| swap item locations 'Empty lamp(index:60)' and 'Lit brass lamp(index:9)' |
| Action| ActionID 76 | look |
### Action 22 - MUDDY RUG - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 524, 583, 580, 1220, 0, 10800, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Condition| ConditionID 2 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' carried or in room with player |
| Action| ActionID 72 ArgID 29, 61| swap item locations '*Thick PERSIAN RUG*(index:29)' and 'Muddy worthless old rug(index:61)' |
### Action 23 - Input: LOO LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4404, 682, 0, 0, 0, 0, 6900, 0|  |
| Verb| 29| LOO |
| Noun| 54| LAV |
| Condition| ConditionID 1 ArgID 34| item 'Stream of lava(index:34)' in room with player |
| Action| ActionID 46 | Print message 'There's something there all right\! Maybe I should go there?' |
### Action 24 - Input: LOO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4407, 82, 0, 0, 0, 0, 6900, 0|  |
| Verb| 29| LOO |
| Noun| 57| TRE |
| Condition| ConditionID 1 ArgID 4| item '\-HOLLOW\- stump and remains of a felled tree(index:4)' in room with player |
| Action| ActionID 46 | Print message 'There's something there all right\! Maybe I should go there?' |
### Action 25 - Input: GET MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1521, 142, 421, 420, 140, 0, 8902, 17703|  |
| Verb| 10| GET |
| Noun| 21| MUD |
| Condition| ConditionID 1 ArgID 7| item 'Evil smelling mud(index:7)' in room with player |
| Condition| ConditionID 0 ArgID 21| item 'Infected chigger bites(index:21)' carried |
| Action| ActionID 59 ArgID 21| Item 'Infected chigger bites(index:21)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 7| get item 'Evil smelling mud(index:7)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
### Action 26 - Input: GET HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1542, 462, 146, 482, 0, 0, 2311, 0|  |
| Verb| 10| GET |
| Noun| 42| HON |
| Condition| ConditionID 1 ArgID 23| item '\*ROYAL HONEY\*(index:23)' in room with player |
| Condition| ConditionID 5 ArgID 7| item 'Evil smelling mud(index:7)' not carried |
| Condition| ConditionID 1 ArgID 24| item 'Large african bees(index:24)' in room with player |
| Action| ActionID 15 | Print message 'Bees sting me' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 27 - Input: GET MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1521, 142, 401, 400, 140, 0, 8902, 17703|  |
| Verb| 10| GET |
| Noun| 21| MUD |
| Condition| ConditionID 1 ArgID 7| item 'Evil smelling mud(index:7)' in room with player |
| Condition| ConditionID 0 ArgID 20| item 'Chigger bites(index:20)' carried |
| Action| ActionID 59 ArgID 20| Item 'Chigger bites(index:20)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 7| get item 'Evil smelling mud(index:7)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
### Action 28 - Input: DRO HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2742, 461, 460, 502, 780, 500, 8864, 8005|  |
| Verb| 18| DRO |
| Noun| 42| HON |
| Condition| ConditionID 0 ArgID 23| item '\*ROYAL HONEY\*(index:23)' carried |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 59 ArgID 23| Item '*ROYAL HONEY*(index:23)' is removed from the game (put in room 0) |
| Action| ActionID 14 | Print message 'Bear eats the honey and falls asleep\.' |
| Action| ActionID 53 ArgID 39| drops item 'Sleeping bear(index:39)' into current room |
| Action| ActionID 55 ArgID 25| Item 'Very thin black bear(index:25)' is removed from the game (put in room 0) |
### Action 29 - Input: DRO HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2742, 461, 460, 0, 0, 0, 7950, 0|  |
| Verb| 18| DRO |
| Noun| 42| HON |
| Condition| ConditionID 0 ArgID 23| item '\*ROYAL HONEY\*(index:23)' carried |
| Action| ActionID 53 ArgID 23| drops item '*ROYAL HONEY*(index:23)' into current room |
### Action 30 - Input: GET BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1523, 482, 146, 0, 0, 0, 2311, 0|  |
| Verb| 10| GET |
| Noun| 23| BEE |
| Condition| ConditionID 1 ArgID 24| item 'Large african bees(index:24)' in room with player |
| Condition| ConditionID 5 ArgID 7| item 'Evil smelling mud(index:7)' not carried |
| Action| ActionID 15 | Print message 'Bees sting me' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 31 - Input: GET BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1523, 482, 141, 266, 0, 0, 2400, 0|  |
| Verb| 10| GET |
| Noun| 23| BEE |
| Condition| ConditionID 1 ArgID 24| item 'Large african bees(index:24)' in room with player |
| Condition| ConditionID 0 ArgID 7| item 'Evil smelling mud(index:7)' carried |
| Condition| ConditionID 5 ArgID 13| item 'Empty bottle(index:13)' not carried |
| Action| ActionID 16 | Print message 'First I need an empty container\.' |
### Action 32 - Input: GET BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1523, 482, 141, 261, 260, 520, 10918, 0|  |
| Verb| 10| GET |
| Noun| 23| BEE |
| Condition| ConditionID 1 ArgID 24| item 'Large african bees(index:24)' in room with player |
| Condition| ConditionID 0 ArgID 7| item 'Evil smelling mud(index:7)' carried |
| Condition| ConditionID 0 ArgID 13| item 'Empty bottle(index:13)' carried |
| Action| ActionID 72 ArgID 13, 26| swap item locations 'Empty bottle(index:13)' and 'Bees in a bottle(index:26)' |
| Action| ActionID 118 | Print message 'OK' |
### Action 33 - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1533, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 10| GET |
| Noun| 33| INV |
| Action| ActionID 66 | output inventory |
### Action 34 - Input: CRO LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8454, 364, 0, 0, 0, 0, 7650, 0|  |
| Verb| 56| CRO |
| Noun| 54| LAV |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 51 | Print message 'No, its too hot\.' |
### Action 35 - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5100, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 34| INV |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
### Action 36 - Input: SAY AWA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7209, 581, 344, 460, 0, 0, 8118, 8614|  |
| Verb| 48| SAY |
| Noun| 9| AWA |
| Condition| ConditionID 0 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' carried |
| Condition| ConditionID 3 ArgID 17| player in room 17 |
| Action| ActionID 54 ArgID 23| move room 23 |
| Action| ActionID 18 | Print message 'Something I'm holding vibrates and\.\.\.' |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 64 | look |
### Action 37 - Input: LIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2100, 566, 0, 0, 0, 0, 2850, 0|  |
| Verb| 14| LIG |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 28| item 'Flint & steel(index:28)' not carried |
| Action| ActionID 19 | Print message 'nothing to light it with' |
### Action 38 - Input: LIG GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2125, 621, 561, 620, 0, 0, 3021, 9209|  |
| Verb| 14| LIG |
| Noun| 25| GAS |
| Condition| ConditionID 0 ArgID 31| item 'Distended gas bladder(index:31)' carried |
| Condition| ConditionID 0 ArgID 28| item 'Flint & steel(index:28)' carried |
| Action| ActionID 20 | Print message 'Gas bladder blew up' |
| Action| ActionID 21 | Print message 'in my hands\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
| Action| ActionID 59 ArgID 31| Item 'Distended gas bladder(index:31)' is removed from the game (put in room 0) |
### Action 39 - Input: MAK HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8716, 523, 340, 0, 0, 0, 8818, 0|  |
| Verb| 58| MAK |
| Noun| 16| HOL |
| Condition| ConditionID 2 ArgID 26| item 'Bees in a bottle(index:26)' carried or in room with player |
| Action| ActionID 58 ArgID 17| set 17 flag |
| Action| ActionID 118 | Print message 'OK' |
### Action 40 - Input: LIG GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2125, 622, 561, 620, 240, 0, 10555, 8720|  |
| Verb| 14| LIG |
| Noun| 25| GAS |
| Condition| ConditionID 1 ArgID 31| item 'Distended gas bladder(index:31)' in room with player |
| Condition| ConditionID 0 ArgID 28| item 'Flint & steel(index:28)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 55 ArgID 31| Item 'Distended gas bladder(index:31)' is removed from the game (put in room 0) |
| Action| ActionID 58 ArgID 12| set 12 flag |
| Action| ActionID 20 | Print message 'Gas bladder blew up' |
### Action 41 - Input: GO LED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 184, 404, 702, 380, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 34| LED |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 1 ArgID 35| item 'Bricked up window with a hole in it(index:35)' in room with player |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 42 - Input: GET GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1525, 24, 806, 0, 0, 0, 2400, 0|  |
| Verb| 10| GET |
| Noun| 25| GAS |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Condition| ConditionID 5 ArgID 40| item 'Empty wine bladder(index:40)' not carried |
| Action| ActionID 16 | Print message 'First I need an empty container\.' |
### Action 43 - Input: GET GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1525, 24, 801, 800, 620, 0, 10918, 0|  |
| Verb| 10| GET |
| Noun| 25| GAS |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Condition| ConditionID 0 ArgID 40| item 'Empty wine bladder(index:40)' carried |
| Action| ActionID 72 ArgID 40, 31| swap item locations 'Empty wine bladder(index:40)' and 'Distended gas bladder(index:31)' |
| Action| ActionID 118 | Print message 'OK' |
### Action 44 - Input: DRO GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2725, 621, 620, 800, 0, 0, 10918, 3450|  |
| Verb| 18| DRO |
| Noun| 25| GAS |
| Condition| ConditionID 0 ArgID 31| item 'Distended gas bladder(index:31)' carried |
| Action| ActionID 72 ArgID 31, 40| swap item locations 'Distended gas bladder(index:31)' and 'Empty wine bladder(index:40)' |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 23 | Print message 'Gas dissipates\. \(I think you blew it\)' |
### Action 45 - Input: LIG GAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2125, 362, 561, 0, 0, 0, 3300, 0|  |
| Verb| 14| LIG |
| Noun| 25| GAS |
| Condition| ConditionID 1 ArgID 18| item 'Swamp gas(index:18)' in room with player |
| Condition| ConditionID 0 ArgID 28| item 'Flint & steel(index:28)' carried |
| Action| ActionID 22 | Print message 'gas needs to be contained before it will burn' |
### Action 46 - Input: FIN SWA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6803, 0, 0, 0, 0, 0, 17100, 0|  |
| Verb| 45| FIN |
| Noun| 53| SWA |
| Action| ActionID 114 | Print message 'I don't know where it is' |
### Action 47 - Input: GO THR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 185, 384, 0, 0, 0, 0, 3750, 0|  |
| Verb| 1| GO |
| Noun| 35| THR |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Action| ActionID 25 | Print message 'How?' |
### Action 48 - Input: GET MIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 762, 760, 505, 0, 0, 7918, 0|  |
| Verb| 10| GET |
| Noun| 10| MIR |
| Condition| ConditionID 1 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' in room with player |
| Condition| ConditionID 4 ArgID 25| item 'Very thin black bear(index:25)' not in room with player |
| Action| ActionID 52 ArgID 38| get item '*MAGIC MIRROR*(index:38)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
### Action 49 - Input: DRO MIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2710, 761, 760, 582, 20, 0, 7986, 8700|  |
| Verb| 18| DRO |
| Noun| 10| MIR |
| Condition| ConditionID 0 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' carried |
| Condition| ConditionID 1 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' in room with player |
| Action| ActionID 53 ArgID 38| drops item '*MAGIC MIRROR*(index:38)' into current room |
| Action| ActionID 36 | Print message 'Mirror lands softly on rug, lights up and says:' |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 50 - Input: DRI FRU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6343, 921, 920, 0, 0, 0, 509, 0|  |
| Verb| 42| DRI |
| Noun| 43| FRU |
| Condition| ConditionID 0 ArgID 46| item '\*JEWELED FRUIT\*(index:46)' carried |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
| Action| ActionID 59 ArgID 46| Item '*JEWELED FRUIT*(index:46)' is removed from the game (put in room 0) |
### Action 51 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1513, 122, 261, 260, 240, 0, 8902, 17700|  |
| Verb| 10| GET |
| Noun| 13| WAT |
| Condition| ConditionID 1 ArgID 6| item 'Water(index:6)' in room with player |
| Condition| ConditionID 0 ArgID 13| item 'Empty bottle(index:13)' carried |
| Action| ActionID 59 ArgID 13| Item 'Empty bottle(index:13)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 12| get item 'Water in bottle(index:12)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
### Action 52 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 384, 420, 726, 0, 0, 8164, 0|  |
| Verb| 6| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Condition| ConditionID 5 ArgID 36| item 'Loose fire bricks(index:36)' not carried |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 64 | look |
### Action 53 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 424, 380, 0, 0, 0, 8164, 0|  |
| Verb| 6| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 64 | look |
### Action 54 - Input: GO THR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 185, 424, 502, 0, 0, 0, 3900, 0|  |
| Verb| 1| GO |
| Noun| 35| THR |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 26 | Print message 'Bear won't let me' |
### Action 55 - Input: GO THR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 185, 424, 505, 440, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 35| THR |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 4 ArgID 25| item 'Very thin black bear(index:25)' not in room with player |
| Action| ActionID 54 ArgID 22| move room 22 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 56 - BUILD DAM - Input: MAK LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8754, 723, 0, 680, 900, 682, 10853, 11400|  |
| Verb| 58| MAK |
| Noun| 54| LAV |
| Condition| ConditionID 2 ArgID 36| item 'Loose fire bricks(index:36)' carried or in room with player |
| Condition| ConditionID 1 ArgID 34| item 'Stream of lava(index:34)' in room with player |
| Action| ActionID 72 ArgID 0, 34| swap item locations 'Glowing *FIRESTONE*(index:0)' and 'Stream of lava(index:34)' |
| Action| ActionID 53 ArgID 45| drops item 'Lava stream with brick dam(index:45)' into current room |
| Action| ActionID 76 | look |
### Action 57 - Input: GO LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 204, 364, 0, 0, 0, 0, 7650, 0|  |
| Verb| 1| GO |
| Noun| 54| LAV |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 51 | Print message 'No, its too hot\.' |
### Action 58 - Input: DRO BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2723, 521, 502, 520, 480, 280, 4259, 8008|  |
| Verb| 18| DRO |
| Noun| 23| BEE |
| Condition| ConditionID 0 ArgID 26| item 'Bees in a bottle(index:26)' carried |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 28 | Print message 'Bees madden bear, bear then attacks me\!' |
| Action| ActionID 59 ArgID 26| Item 'Bees in a bottle(index:26)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 24| drops item 'Large african bees(index:24)' into current room |
| Action| ActionID 58 ArgID 14| set 14 flag |
### Action 59 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1513, 122, 266, 0, 0, 0, 2400, 0|  |
| Verb| 10| GET |
| Noun| 13| WAT |
| Condition| ConditionID 1 ArgID 6| item 'Water(index:6)' in room with player |
| Condition| ConditionID 5 ArgID 13| item 'Empty bottle(index:13)' not carried |
| Action| ActionID 16 | Print message 'First I need an empty container\.' |
### Action 60 - Input: REA WEB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5751, 62, 0, 0, 0, 0, 300, 0|  |
| Verb| 38| REA |
| Noun| 51| WEB |
| Condition| ConditionID 1 ArgID 3| item 'Spider web with writing on it(index:3)' in room with player |
| Action| ActionID 2 | Print message 'Chop 'er down\!' |
### Action 61 - Input: GO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 207, 40, 102, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 57| TRE |
| Condition| ConditionID 1 ArgID 5| item 'Cypress tree(index:5)' in room with player |
| Action| ActionID 54 ArgID 2| move room 2 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 62 - Input: DRO WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2713, 241, 240, 260, 367, 0, 10918, 4350|  |
| Verb| 18| DRO |
| Noun| 13| WAT |
| Condition| ConditionID 0 ArgID 12| item 'Water in bottle(index:12)' carried |
| Condition| ConditionID 6 ArgID 18| player not in room 18 |
| Action| ActionID 72 ArgID 12, 13| swap item locations 'Water in bottle(index:12)' and 'Empty bottle(index:13)' |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 29 | Print message 'It soaks into the ground' |
### Action 63 - Input: FIL LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8267, 443, 1201, 440, 1200, 0, 8909, 6669|  |
| Verb| 55| FIL |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 22| item 'Patches of `OILY` slime(index:22)' carried or in room with player |
| Condition| ConditionID 0 ArgID 60| item 'Empty lamp(index:60)' carried |
| Action| ActionID 59 ArgID 22| Item 'Patches of `OILY` slime(index:22)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 60| Item 'Empty lamp(index:60)' is removed from the game (put in room 0) |
| Action| ActionID 44 | Print message 'Lamp is now full & lit' |
| Action| ActionID 69 | refill lamp |
### Action 64 - Input: CHO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1257, 100, 102, 292, 80, 221, 8303, 1050|  |
| Verb| 8| CHO |
| Noun| 57| TRE |
| Condition| ConditionID 1 ArgID 5| item 'Cypress tree(index:5)' in room with player |
| Condition| ConditionID 11 ArgID 14| item 'Ring of skeleton keys(index:14)' not carried or in room with player |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Action| ActionID 55 ArgID 5| Item 'Cypress tree(index:5)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 4| drops item '-HOLLOW- stump and remains of a felled tree(index:4)' into current room |
| Action| ActionID 7 | Print message 'TIMBER\. Something fell from the tree top & vanished in the swamp' |
### Action 65 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10370, 104, 322, 286, 0, 0, 900, 0|  |
| Verb| 69| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 1 ArgID 16| item 'Locked door(index:16)' in room with player |
| Condition| ConditionID 5 ArgID 14| item 'Ring of skeleton keys(index:14)' not carried |
| Action| ActionID 6 | Print message 'I can't its locked' |
### Action 66 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5570, 104, 322, 286, 0, 0, 900, 0|  |
| Verb| 37| UNL |
| Noun| 20| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 1 ArgID 16| item 'Locked door(index:16)' in room with player |
| Condition| ConditionID 5 ArgID 14| item 'Ring of skeleton keys(index:14)' not carried |
| Action| ActionID 6 | Print message 'I can't its locked' |
### Action 67 - Input: THR AXE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3611, 221, 60, 220, 0, 0, 4558, 7950|  |
| Verb| 24| THR |
| Noun| 11| AXE |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Action| ActionID 30 | Print message 'In 2 words tell me at what\.\.\.like: AT TREE' |
| Action| ActionID 58 ArgID 3| set 3 flag |
| Action| ActionID 53 ArgID 11| drops item 'Rusty axe (Magic word `BUNYON` on it)(index:11)' into current room |
### Action 68 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10370, 322, 281, 320, 340, 0, 8303, 11400|  |
| Verb| 69| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Locked door(index:16)' in room with player |
| Condition| ConditionID 0 ArgID 14| item 'Ring of skeleton keys(index:14)' carried |
| Action| ActionID 55 ArgID 16| Item 'Locked door(index:16)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 17| drops item 'Open door with a hallway beyond(index:17)' into current room |
| Action| ActionID 76 | look |
### Action 69 - Input: CRO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 0, 0, 0, 0, 0, 3750, 0|  |
| Verb| 56| CRO |
| Noun| 0| ANY |
| Action| ActionID 25 | Print message 'How?' |
### Action 70 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 384, 721, 0, 0, 0, 5011, 0|  |
| Verb| 6| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Condition| ConditionID 0 ArgID 36| item 'Loose fire bricks(index:36)' carried |
| Action| ActionID 33 | Print message 'Somethings too heavy\. I fall\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 71 - Input: DAM LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8604, 723, 0, 680, 900, 682, 10853, 11400|  |
| Verb| 57| DAM |
| Noun| 54| LAV |
| Condition| ConditionID 2 ArgID 36| item 'Loose fire bricks(index:36)' carried or in room with player |
| Condition| ConditionID 1 ArgID 34| item 'Stream of lava(index:34)' in room with player |
| Action| ActionID 72 ArgID 0, 34| swap item locations 'Glowing *FIRESTONE*(index:0)' and 'Stream of lava(index:34)' |
| Action| ActionID 53 ArgID 45| drops item 'Lava stream with brick dam(index:45)' into current room |
| Action| ActionID 76 | look |
### Action 72 - Input: GET BRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1537, 722, 720, 0, 0, 0, 7918, 4800|  |
| Verb| 10| GET |
| Noun| 37| BRI |
| Condition| ConditionID 1 ArgID 36| item 'Loose fire bricks(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Loose fire bricks(index:36)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 32 | Print message 'Its heavy\!' |
### Action 73 - Input: STO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4800, 0, 0, 0, 0, 0, 5100, 0|  |
| Verb| 32| STO |
| Noun| 0| ANY |
| Action| ActionID 34 | Print message 'To stop game say QUIT' |
### Action 74 - Input: QUI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3900, 0, 0, 0, 0, 0, 9813, 0|  |
| Verb| 26| QUI |
| Noun| 0| ANY |
| Action| ActionID 65 | score |
| Action| ActionID 63 | game over |
### Action 75 - Input: GET MIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 762, 502, 0, 0, 0, 3900, 0|  |
| Verb| 10| GET |
| Noun| 10| MIR |
| Condition| ConditionID 1 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' in room with player |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 26 | Print message 'Bear won't let me' |
### Action 76 - Input: DRO MIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2710, 761, 585, 820, 760, 0, 5303, 8850|  |
| Verb| 18| DRO |
| Noun| 10| MIR |
| Condition| ConditionID 0 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' carried |
| Condition| ConditionID 4 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' not in room with player |
| Action| ActionID 35 | Print message 'Mirror hits floor and shatters into a MILLION pieces' |
| Action| ActionID 53 ArgID 41| drops item 'Broken glass(index:41)' into current room |
| Action| ActionID 59 ArgID 38| Item '*MAGIC MIRROR*(index:38)' is removed from the game (put in room 0) |
### Action 77 - Input: AT BEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1088, 68, 765, 60, 0, 0, 18410, 16710|  |
| Verb| 7| AT |
| Noun| 38| BEA |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Condition| ConditionID 4 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' not in room with player |
| Action| ActionID 122 | Print message 'OK, I threw it\.' |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 111 | Print message 'please leave it alone' |
| Action| ActionID 60 ArgID 3| set 3 flag |
### Action 78 - Input: AT DRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1089, 68, 60, 542, 0, 0, 18339, 9000|  |
| Verb| 7| AT |
| Noun| 39| DRA |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Condition| ConditionID 1 ArgID 27| item 'Large sleeping dragon(index:27)' in room with player |
| Action| ActionID 122 | Print message 'OK, I threw it\.' |
| Action| ActionID 39 | Print message 'It doesn't seem to bother him at all\!' |
| Action| ActionID 60 ArgID 3| set 3 flag |
### Action 79 - Input: SCO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4950, 0, 0, 0, 0, 0, 9750, 0|  |
| Verb| 33| SCO |
| Noun| 0| ANY |
| Action| ActionID 65 | score |
### Action 80 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 401, 0, 0, 0, 0, 10610, 17055|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 20| item 'Chigger bites(index:20)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 113 | Print message 'Medicine is good for bites\.' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 81 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 421, 0, 0, 0, 0, 10610, 17055|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 21| item 'Infected chigger bites(index:21)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 113 | Print message 'Medicine is good for bites\.' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 82 - Input: GO LED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 184, 364, 0, 0, 0, 0, 15300, 0|  |
| Verb| 1| GO |
| Noun| 34| LED |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 102 | Print message 'Not here\.' |
### Action 83 - Input: GET LAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1554, 682, 0, 0, 0, 0, 7650, 0|  |
| Verb| 10| GET |
| Noun| 54| LAV |
| Condition| ConditionID 1 ArgID 34| item 'Stream of lava(index:34)' in room with player |
| Action| ActionID 51 | Print message 'No, its too hot\.' |
### Action 84 - Input: SCR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 502, 860, 360, 500, 0, 6212, 8250|  |
| Verb| 51| SCR |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 41 | Print message 'Bear is so startled that he FELL off the ledge\!' |
| Action| ActionID 62 ArgID 43, 18| item 'Slightly woozy bear(index:43)' is moved to room 18 |
| Action| ActionID 55 ArgID 25| Item 'Very thin black bear(index:25)' is removed from the game (put in room 0) |
### Action 85 - Input: DRO BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2723, 521, 542, 480, 880, 540, 8003, 8293|  |
| Verb| 18| DRO |
| Noun| 23| BEE |
| Condition| ConditionID 0 ArgID 26| item 'Bees in a bottle(index:26)' carried |
| Condition| ConditionID 1 ArgID 27| item 'Large sleeping dragon(index:27)' in room with player |
| Action| ActionID 53 ArgID 24| drops item 'Large african bees(index:24)' into current room |
| Action| ActionID 53 ArgID 44| drops item '*DRAGON EGGS* (very rare)(index:44)' into current room |
| Action| ActionID 55 ArgID 27| Item 'Large sleeping dragon(index:27)' is removed from the game (put in room 0) |
| Action| ActionID 43 | Print message 'The bees attack the dragon which gets so annoyed it gets up and flys away\.\.\.' |
### Action 86 - Input: AT WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1069, 68, 60, 0, 0, 0, 9001, 16607|  |
| Verb| 7| AT |
| Noun| 19| WIN |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 60 ArgID 3| set 3 flag |
| Action| ActionID 1 | Print message 'Nothing happens' |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 107 | Print message 'Remember you can always say `HELP`' |
### Action 87 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10370, 342, 0, 0, 0, 0, 9600, 0|  |
| Verb| 69| OPE |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 17| item 'Open door with a hallway beyond(index:17)' in room with player |
| Action| ActionID 64 | look |
### Action 88 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 166, 702, 380, 0, 0, 0, 10554, 9600|  |
| Verb| 1| GO |
| Noun| 16| HOL |
| Condition| ConditionID 1 ArgID 35| item 'Bricked up window with a hole in it(index:35)' in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 64 | look |
### Action 89 - Input: AT BEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1088, 68, 760, 100, 80, 762, 8308, 4710|  |
| Verb| 7| AT |
| Noun| 38| BEA |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Condition| ConditionID 1 ArgID 38| item '\*MAGIC MIRROR\*(index:38)' in room with player |
| Action| ActionID 55 ArgID 38| Item '*MAGIC MIRROR*(index:38)' is removed from the game (put in room 0) |
| Action| ActionID 58 ArgID 5| set 5 flag |
| Action| ActionID 31 | Print message 'OH NO\.\.\. Bear dodges\.\.\. CRASH\!' |
| Action| ActionID 60 ArgID 4| set 4 flag |
### Action 90 - Input: FIN AXE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6761, 0, 0, 0, 0, 0, 16614, 0|  |
| Verb| 45| FIN |
| Noun| 11| AXE |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 114 | Print message 'I don't know where it is' |
### Action 91 - Input: WAK ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5400, 0, 0, 0, 0, 0, 197, 0|  |
| Verb| 36| WAK |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
| Action| ActionID 47 | Print message 'Maybe if I threw something?\.\.\.' |
### Action 92 - Input: GO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 207, 82, 60, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 57| TRE |
| Condition| ConditionID 1 ArgID 4| item '\-HOLLOW\- stump and remains of a felled tree(index:4)' in room with player |
| Action| ActionID 54 ArgID 3| move room 3 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 93 - Input: CHO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1257, 102, 221, 100, 80, 281, 8303, 1200|  |
| Verb| 8| CHO |
| Noun| 57| TRE |
| Condition| ConditionID 1 ArgID 5| item 'Cypress tree(index:5)' in room with player |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Condition| ConditionID 0 ArgID 14| item 'Ring of skeleton keys(index:14)' carried |
| Action| ActionID 55 ArgID 5| Item 'Cypress tree(index:5)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 4| drops item '-HOLLOW- stump and remains of a felled tree(index:4)' into current room |
| Action| ActionID 8 | Print message 'TIMBER\!' |
### Action 94 - Input: ATT BEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5888, 502, 0, 0, 0, 0, 3947, 0|  |
| Verb| 39| ATT |
| Noun| 38| BEA |
| Condition| ConditionID 1 ArgID 25| item 'Very thin black bear(index:25)' in room with player |
| Action| ActionID 26 | Print message 'Bear won't let me' |
| Action| ActionID 47 | Print message 'Maybe if I threw something?\.\.\.' |
### Action 95 - Input: ATT DRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5889, 542, 0, 0, 0, 0, 5897, 0|  |
| Verb| 39| ATT |
| Noun| 39| DRA |
| Condition| ConditionID 1 ArgID 27| item 'Large sleeping dragon(index:27)' in room with player |
| Action| ActionID 39 | Print message 'It doesn't seem to bother him at all\!' |
| Action| ActionID 47 | Print message 'Maybe if I threw something?\.\.\.' |
### Action 96 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6313, 241, 240, 260, 0, 0, 509, 7800|  |
| Verb| 42| DRI |
| Noun| 13| WAT |
| Condition| ConditionID 0 ArgID 12| item 'Water in bottle(index:12)' carried |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
| Action| ActionID 59 ArgID 12| Item 'Water in bottle(index:12)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 13| get item 'Empty bottle(index:13)', check if can carry |
### Action 97 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6313, 122, 0, 0, 0, 0, 450, 0|  |
| Verb| 42| DRI |
| Noun| 13| WAT |
| Condition| ConditionID 1 ArgID 6| item 'Water(index:6)' in room with player |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
### Action 98 - Input: DRI HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6342, 463, 460, 0, 0, 0, 509, 0|  |
| Verb| 42| DRI |
| Noun| 42| HON |
| Condition| ConditionID 2 ArgID 23| item '\*ROYAL HONEY\*(index:23)' carried or in room with player |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
| Action| ActionID 59 ArgID 23| Item '*ROYAL HONEY*(index:23)' is removed from the game (put in room 0) |
### Action 99 - Input: AT DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1070, 322, 68, 320, 340, 60, 8303, 810|  |
| Verb| 7| AT |
| Noun| 20| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Locked door(index:16)' in room with player |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 55 ArgID 16| Item 'Locked door(index:16)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 17| drops item 'Open door with a hallway beyond(index:17)' into current room |
| Action| ActionID 5 | Print message 'Lock shatters' |
| Action| ActionID 60 ArgID 3| set 3 flag |
### Action 100 - Input: SWI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 524, 10, 0, 0, 0, 4950, 0|  |
| Verb| 27| SWI |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Condition| ConditionID 9 ArgID 0| something carried |
| Action| ActionID 33 | Print message 'Somethings too heavy\. I fall\.' |
### Action 101 - Input: SWI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 524, 11, 200, 0, 0, 8170, 9600|  |
| Verb| 27| SWI |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Condition| ConditionID 10 ArgID 0| nothing carried |
| Action| ActionID 54 ArgID 10| move room 10 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 102 - Input: CHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1200, 226, 0, 0, 0, 0, 5700, 0|  |
| Verb| 8| CHO |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' not carried |
| Action| ActionID 38 | Print message 'I'm not carrying ax, take inventory\!' |
### Action 103 - Input: SAY BUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7232, 943, 221, 220, 500, 140, 12768, 9358|  |
| Verb| 48| SAY |
| Noun| 32| BUN |
| Condition| ConditionID 2 ArgID 47| item '\*Small statue of a BLUE OX\*(index:47)' carried or in room with player |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Action| ActionID 85 | echo noun |
| Action| ActionID 18 | Print message 'Something I'm holding vibrates and\.\.\.' |
| Action| ActionID 62 ArgID 11, 25| item 'Rusty axe (Magic word `BUNYON` on it)(index:11)' is moved to room 25 |
| Action| ActionID 58 ArgID 7| set 7 flag |
### Action 104 - Input: SAY BUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7232, 221, 527, 220, 500, 0, 12768, 9366|  |
| Verb| 48| SAY |
| Noun| 32| BUN |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Condition| ConditionID 6 ArgID 26| player not in room 26 |
| Action| ActionID 85 | echo noun |
| Action| ActionID 18 | Print message 'Something I'm holding vibrates and\.\.\.' |
| Action| ActionID 62 ArgID 11, 25| item 'Rusty axe (Magic word `BUNYON` on it)(index:11)' is moved to room 25 |
| Action| ActionID 66 | output inventory |
### Action 105 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 183, 0, 0, 0, 0, 7650, 0|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 9| item 'Lit brass lamp(index:9)' carried or in room with player |
| Action| ActionID 51 | Print message 'No, its too hot\.' |
### Action 106 - Input: GET MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1521, 142, 140, 0, 0, 0, 7918, 0|  |
| Verb| 10| GET |
| Noun| 21| MUD |
| Condition| ConditionID 1 ArgID 7| item 'Evil smelling mud(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Evil smelling mud(index:7)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
### Action 107 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 203, 169, 960, 160, 0, 7403, 8700|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Condition| ConditionID 8 ArgID 8| bitflag 8 is false |
| Action| ActionID 49 | Print message 'A glowing Genie appears, drops somehting, then vanishes\.' |
| Action| ActionID 53 ArgID 48| drops item '*DIAMOND RING*(index:48)' into current room |
| Action| ActionID 58 ArgID 8| set 8 flag |
### Action 108 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 203, 228, 0, 0, 0, 150, 0|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 109 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 203, 208, 220, 960, 0, 7558, 9209|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 50 | Print message 'A glowing Genie appears, says `Boy you're selfish`, takes something and then makes `ME` vanish\!' |
| Action| ActionID 58 ArgID 11| set 11 flag |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
| Action| ActionID 59 ArgID 48| Item '*DIAMOND RING*(index:48)' is removed from the game (put in room 0) |
### Action 110 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 203, 188, 200, 980, 0, 7558, 9209|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Condition| ConditionID 7 ArgID 9| bitflag 9 is set |
| Action| ActionID 50 | Print message 'A glowing Genie appears, says `Boy you're selfish`, takes something and then makes `ME` vanish\!' |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
| Action| ActionID 59 ArgID 49| Item '*DIAMOND BRACELET*(index:49)' is removed from the game (put in room 0) |
### Action 111 - Input: RUB LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4217, 203, 168, 980, 180, 0, 7403, 8700|  |
| Verb| 28| RUB |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Condition| ConditionID 7 ArgID 8| bitflag 8 is set |
| Action| ActionID 49 | Print message 'A glowing Genie appears, drops somehting, then vanishes\.' |
| Action| ActionID 53 ArgID 49| drops item '*DIAMOND BRACELET*(index:49)' into current room |
| Action| ActionID 58 ArgID 9| set 9 flag |
### Action 112 - Input: SCR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 401, 400, 420, 0, 0, 462, 10800|  |
| Verb| 51| SCR |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 20| item 'Chigger bites(index:20)' carried |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
| Action| ActionID 12 | Print message ' My chigger bites are now INFECTED\! ' |
| Action| ActionID 72 ArgID 20, 21| swap item locations 'Chigger bites(index:20)' and 'Infected chigger bites(index:21)' |
### Action 113 - Input: SCR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 421, 0, 0, 0, 0, 463, 9150|  |
| Verb| 51| SCR |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 21| item 'Infected chigger bites(index:21)' carried |
| Action| ActionID 3 | Print message 'BOY that really hit the spot\!' |
| Action| ActionID 13 | Print message 'My bites have rotted my whole body\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 114 - Input: SWI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 527, 0, 0, 0, 0, 15300, 0|  |
| Verb| 27| SWI |
| Noun| 0| ANY |
| Condition| ConditionID 6 ArgID 26| player not in room 26 |
| Action| ActionID 102 | Print message 'Not here\.' |
### Action 115 - Input: WAV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9000, 0, 0, 0, 0, 0, 150, 0|  |
| Verb| 60| WAV |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 116 - Input: SAY BUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7232, 222, 0, 0, 0, 0, 17785, 18600|  |
| Verb| 48| SAY |
| Noun| 32| BUN |
| Condition| ConditionID 1 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' in room with player |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 124 | Print message 'The ax vibrated\!' |
### Action 117 - Input: LIG LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2117, 183, 0, 0, 0, 0, 1500, 0|  |
| Verb| 14| LIG |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 9| item 'Lit brass lamp(index:9)' carried or in room with player |
| Action| ActionID 10 | Print message 'Lamp burns with a cold flameless blue glow\.' |
### Action 118 - Input: FIN TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6807, 0, 0, 0, 0, 0, 15450, 0|  |
| Verb| 45| FIN |
| Noun| 57| TRE |
| Action| ActionID 103 | Print message 'Try the swamp' |
### Action 119 - Input: DRO BEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2723, 521, 480, 520, 260, 0, 8022, 17700|  |
| Verb| 18| DRO |
| Noun| 23| BEE |
| Condition| ConditionID 0 ArgID 26| item 'Bees in a bottle(index:26)' carried |
| Action| ActionID 53 ArgID 24| drops item 'Large african bees(index:24)' into current room |
| Action| ActionID 72 ArgID 26, 13| swap item locations 'Bees in a bottle(index:26)' and 'Empty bottle(index:13)' |
| Action| ActionID 118 | Print message 'OK' |
### Action 120 - Input: FIN KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6780, 0, 0, 0, 0, 0, 15450, 0|  |
| Verb| 45| FIN |
| Noun| 30| KEY |
| Action| ActionID 103 | Print message 'Try the swamp' |
### Action 121 - Input: FIN MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6771, 0, 0, 0, 0, 0, 15450, 0|  |
| Verb| 45| FIN |
| Noun| 21| MUD |
| Action| ActionID 103 | Print message 'Try the swamp' |
### Action 122 - Input: AT SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1110, 68, 60, 524, 220, 200, 9062, 17700|  |
| Verb| 7| AT |
| Noun| 60| SHO |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Action| ActionID 60 ArgID 3| set 3 flag |
| Action| ActionID 62 ArgID 11, 10| item 'Rusty axe (Magic word `BUNYON` on it)(index:11)' is moved to room 10 |
| Action| ActionID 118 | Print message 'OK' |
### Action 123 - Input: GO TRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 207, 224, 560, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 57| TRE |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 54 ArgID 28| move room 28 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 124 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 524, 0, 0, 0, 0, 16605, 16350|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
| Action| ActionID 109 | Print message 'You may need to say magic words here' |
### Action 125 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 224, 0, 0, 0, 0, 16605, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 126 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 384, 0, 0, 0, 0, 16605, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 127 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 464, 0, 0, 0, 0, 16606, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 23| player in room 23 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 106 | Print message 'There are only 3 ways to wake the Dragon\!' |
### Action 128 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 264, 0, 0, 0, 0, 16609, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 109 | Print message 'You may need to say magic words here' |
### Action 129 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 344, 0, 0, 0, 0, 16609, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 17| player in room 17 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 109 | Print message 'You may need to say magic words here' |
### Action 130 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 304, 0, 0, 0, 0, 16609, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 109 | Print message 'You may need to say magic words here' |
### Action 131 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 424, 0, 0, 0, 0, 16605, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 132 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 164, 0, 0, 0, 0, 16608, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 108 | Print message 'Read the sign in the meadow\!' |
### Action 133 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5570, 281, 322, 340, 320, 0, 8005, 0|  |
| Verb| 37| UNL |
| Noun| 20| DOO |
| Condition| ConditionID 0 ArgID 14| item 'Ring of skeleton keys(index:14)' carried |
| Condition| ConditionID 1 ArgID 16| item 'Locked door(index:16)' in room with player |
| Action| ActionID 53 ArgID 17| drops item 'Open door with a hallway beyond(index:17)' into current room |
| Action| ActionID 55 ArgID 16| Item 'Locked door(index:16)' is removed from the game (put in room 0) |
### Action 134 - Input: GO HAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 206, 342, 120, 0, 0, 0, 8156, 10564|  |
| Verb| 1| GO |
| Noun| 56| HAL |
| Condition| ConditionID 1 ArgID 17| item 'Open door with a hallway beyond(index:17)' in room with player |
| Action| ActionID 54 ArgID 6| move room 6 |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 135 - Input: LIG LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2117, 203, 200, 180, 0, 0, 10810, 11400|  |
| Verb| 14| LIG |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried or in room with player |
| Action| ActionID 72 ArgID 10, 9| swap item locations 'Old fashioned brass lamp(index:10)' and 'Lit brass lamp(index:9)' |
| Action| ActionID 10 | Print message 'Lamp burns with a cold flameless blue glow\.' |
| Action| ActionID 76 | look |
### Action 136 - Input: UNL LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5567, 183, 180, 200, 0, 0, 10918, 1426|  |
| Verb| 37| UNL |
| Noun| 17| LAM |
| Condition| ConditionID 2 ArgID 9| item 'Lit brass lamp(index:9)' carried or in room with player |
| Action| ActionID 72 ArgID 9, 10| swap item locations 'Lit brass lamp(index:9)' and 'Old fashioned brass lamp(index:10)' |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 9 | Print message 'Lamp is off' |
| Action| ActionID 76 | look |
### Action 137 - Input: GET WEB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1551, 62, 0, 0, 0, 0, 1711, 0|  |
| Verb| 10| GET |
| Noun| 51| WEB |
| Condition| ConditionID 1 ArgID 3| item 'Spider web with writing on it(index:3)' in room with player |
| Action| ActionID 11 | Print message 'I'm bit by a spider' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 138 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 166, 1042, 480, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 16| HOL |
| Condition| ConditionID 1 ArgID 52| item 'Smoking hole\. pieces of dragon and gore\.(index:52)' in room with player |
| Action| ActionID 54 ArgID 24| move room 24 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 139 - Input: GET SIG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1549, 0, 0, 0, 0, 0, 16611, 0|  |
| Verb| 10| GET |
| Noun| 49| SIG |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 111 | Print message 'please leave it alone' |
### Action 140 - Input: LIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2100, 561, 365, 0, 0, 0, 3600, 0|  |
| Verb| 14| LIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 28| item 'Flint & steel(index:28)' carried |
| Condition| ConditionID 4 ArgID 18| item 'Swamp gas(index:18)' not in room with player |
| Action| ActionID 24 | Print message 'That won't ignite' |
### Action 141 - Input: SCR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 0, 0, 0, 0, 0, 150, 0|  |
| Verb| 51| SCR |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 142 - Input: SAY AWA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7209, 581, 347, 340, 667, 527, 8118, 8464|  |
| Verb| 48| SAY |
| Noun| 9| AWA |
| Condition| ConditionID 0 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' carried |
| Condition| ConditionID 6 ArgID 17| player not in room 17 |
| Condition| ConditionID 6 ArgID 33| player not in room 33 |
| Condition| ConditionID 6 ArgID 26| player not in room 26 |
| Action| ActionID 54 ArgID 17| move room 17 |
| Action| ActionID 18 | Print message 'Something I'm holding vibrates and\.\.\.' |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 64 | look |
### Action 143 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 24, 0, 0, 0, 0, 16605, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 105 | Print message 'Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\.' |
### Action 144 - Input: THR AXE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3611, 226, 0, 0, 0, 0, 5700, 0|  |
| Verb| 24| THR |
| Noun| 11| AXE |
| Condition| ConditionID 5 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' not carried |
| Action| ActionID 38 | Print message 'I'm not carrying ax, take inventory\!' |
### Action 145 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 404, 0, 0, 0, 0, 16616, 15450|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 110 | Print message 'A voice BOOOOMS out:' |
| Action| ActionID 116 | Print message 'Blow it up\!' |
| Action| ActionID 103 | Print message 'Try the swamp' |
### Action 146 - Input: SAY BUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7232, 0, 0, 0, 0, 0, 17785, 150|  |
| Verb| 48| SAY |
| Noun| 32| BUN |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 147 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 166, 84, 100, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 16| HOL |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 148 - Input: GET HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1542, 462, 460, 0, 0, 0, 7918, 0|  |
| Verb| 10| GET |
| Noun| 42| HON |
| Condition| ConditionID 1 ArgID 23| item '\*ROYAL HONEY\*(index:23)' in room with player |
| Action| ActionID 52 ArgID 23| get item '*ROYAL HONEY*(index:23)', check if can carry |
| Action| ActionID 118 | Print message 'OK' |
### Action 149 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 0, 0, 0, 0, 0, 270, 0|  |
| Verb| 47| HEL |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
| Action| ActionID 120 | Print message 'You might try examining things\.\.\.' |
### Action 150 - Input: CHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1200, 0, 0, 0, 0, 0, 197, 0|  |
| Verb| 8| CHO |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
| Action| ActionID 47 | Print message 'Maybe if I threw something?\.\.\.' |
### Action 151 - Input: THR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 0, 0, 0, 0, 0, 16800, 0|  |
| Verb| 24| THR |
| Noun| 0| ANY |
| Action| ActionID 112 | Print message 'Sorry, I can only throw the ax\.' |
### Action 152 - Input: AT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1050, 68, 60, 0, 0, 0, 9122, 150|  |
| Verb| 7| AT |
| Noun| 0| ANY |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 60 ArgID 3| set 3 flag |
| Action| ActionID 122 | Print message 'OK, I threw it\.' |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 153 - Input: SAV GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5315, 0, 0, 0, 0, 0, 17771, 0|  |
| Verb| 35| SAV |
| Noun| 65| GAM |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 71 | save game |
### Action 154 - Input: RUB ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4200, 0, 0, 0, 0, 0, 150, 0|  |
| Verb| 28| RUB |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 155 - Input: SAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7200, 0, 0, 0, 0, 0, 17785, 150|  |
| Verb| 48| SAY |
| Noun| 0| ANY |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 1 | Print message 'Nothing happens' |
### Action 156 - Input: DRI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 0, 0, 0, 0, 0, 17850, 0|  |
| Verb| 42| DRI |
| Noun| 0| ANY |
| Action| ActionID 119 | Print message 'Huh? I don't think so\!' |
### Action 157 - Input: DRO WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2713, 241, 364, 240, 260, 0, 15673, 10800|  |
| Verb| 18| DRO |
| Noun| 13| WAT |
| Condition| ConditionID 0 ArgID 12| item 'Water in bottle(index:12)' carried |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 104 | Print message 'Sizzle\.\.\.' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 72 ArgID 12, 13| swap item locations 'Water in bottle(index:12)' and 'Empty bottle(index:13)' |
### Action 158 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 2, 1120, 0, 0, 0, 10800, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 0| item 'Glowing \*FIRESTONE\*(index:0)' in room with player |
| Action| ActionID 72 ArgID 56, 0| swap item locations '*FIRESTONE* (cold now)(index:56)' and 'Glowing *FIRESTONE*(index:0)' |
### Action 159 - Input: GET FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1559, 2, 0, 0, 0, 0, 7650, 0|  |
| Verb| 10| GET |
| Noun| 59| FIR |
| Condition| ConditionID 1 ArgID 0| item 'Glowing \*FIRESTONE\*(index:0)' in room with player |
| Action| ActionID 51 | Print message 'No, its too hot\.' |
### Action 160 - Input: GET FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1559, 1122, 1120, 0, 0, 0, 17752, 0|  |
| Verb| 10| GET |
| Noun| 59| FIR |
| Condition| ConditionID 1 ArgID 56| item '\*FIRESTONE\* \(cold now\)(index:56)' in room with player |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 52 ArgID 56| get item '*FIRESTONE* (cold now)(index:56)', check if can carry |
### Action 161 - Input: FIN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6750, 0, 0, 0, 0, 0, 17100, 0|  |
| Verb| 45| FIN |
| Noun| 0| ANY |
| Action| ActionID 114 | Print message 'I don't know where it is' |
### Action 162 - Input: REA ADV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5762, 1243, 0, 0, 0, 0, 10623, 0|  |
| Verb| 38| REA |
| Noun| 62| ADV |
| Condition| ConditionID 2 ArgID 62| item 'Large outdoor Advertisement(index:62)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 123 | Print message ' Check with your favorite computer dealer for the next Adventure program: PIRATE ADVENTURE\. If they don't carry `ADVENTURE` have them call: 1\-305\-862\-6917 today\! ' |
### Action 163 - Input: LOO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4366, 0, 0, 0, 0, 0, 6900, 0|  |
| Verb| 29| LOO |
| Noun| 16| HOL |
| Action| ActionID 46 | Print message 'There's something there all right\! Maybe I should go there?' |
### Action 164 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 900, 0, 0, 0, 0, 0, 15300, 0|  |
| Verb| 6| JUM |
| Noun| 0| ANY |
| Action| ActionID 102 | Print message 'Not here\.' |
### Action 165 - Input: ATT SPI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5868, 0, 0, 0, 0, 0, 17100, 0|  |
| Verb| 39| ATT |
| Noun| 18| SPI |
| Action| ActionID 114 | Print message 'I don't know where it is' |
### Action 166 - Input: ATT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5850, 0, 0, 0, 0, 0, 3750, 0|  |
| Verb| 39| ATT |
| Noun| 0| ANY |
| Action| ActionID 25 | Print message 'How?' |
### Action 167 - Input: LOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4350, 0, 0, 0, 0, 0, 17825, 11400|  |
| Verb| 29| LOO |
| Noun| 0| ANY |
| Action| ActionID 118 | Print message 'OK' |
| Action| ActionID 125 | Print message 'I see nothing special' |
| Action| ActionID 76 | look |
### Action 168 - Input: AT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1050, 0, 0, 0, 0, 0, 18150, 0|  |
| Verb| 7| AT |
| Noun| 0| ANY |
| Action| ActionID 121 | Print message 'What?' |
### Action 169 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 166, 584, 600, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 16| HOL |
| Condition| ConditionID 3 ArgID 29| player in room 29 |
| Action| ActionID 54 ArgID 30| move room 30 |
| Action| ActionID 76 | look |
### Action 171 - Take for item *Pot of RUBIES* - Input: GET RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 41| RUB |
| Condition| ConditionID 1 ArgID 2| item '\*Pot of RUBIES\*(index:2)' in room with player |
| Action| ActionID 52 ArgID 2| get item '*Pot of RUBIES*(index:2)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 172 - Drop for item *Pot of RUBIES* - Input: DRO RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 41| RUB |
| Condition| ConditionID 0 ArgID 2| item '\*Pot of RUBIES\*(index:2)' carried |
| Action| ActionID 53 ArgID 2| drops item '*Pot of RUBIES*(index:2)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 173 - Take for item Evil smelling mud - Input: GET MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 21| MUD |
| Condition| ConditionID 1 ArgID 7| item 'Evil smelling mud(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Evil smelling mud(index:7)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 174 - Drop for item Evil smelling mud - Input: DRO MUD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 21| MUD |
| Condition| ConditionID 0 ArgID 7| item 'Evil smelling mud(index:7)' carried |
| Action| ActionID 53 ArgID 7| drops item 'Evil smelling mud(index:7)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 175 - Take for item *GOLDEN FISH* - Input: GET FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 8| FIS |
| Condition| ConditionID 1 ArgID 8| item '\*GOLDEN FISH\*(index:8)' in room with player |
| Action| ActionID 52 ArgID 8| get item '*GOLDEN FISH*(index:8)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 176 - Drop for item *GOLDEN FISH* - Input: DRO FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 8| FIS |
| Condition| ConditionID 0 ArgID 8| item '\*GOLDEN FISH\*(index:8)' carried |
| Action| ActionID 53 ArgID 8| drops item '*GOLDEN FISH*(index:8)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 177 - Take for item Lit brass lamp - Input: GET LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 17| LAM |
| Condition| ConditionID 1 ArgID 9| item 'Lit brass lamp(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Lit brass lamp(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 178 - Drop for item Lit brass lamp - Input: DRO LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 17| LAM |
| Condition| ConditionID 0 ArgID 9| item 'Lit brass lamp(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Lit brass lamp(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 179 - Take for item Old fashioned brass lamp - Input: GET LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 17| LAM |
| Condition| ConditionID 1 ArgID 10| item 'Old fashioned brass lamp(index:10)' in room with player |
| Action| ActionID 52 ArgID 10| get item 'Old fashioned brass lamp(index:10)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 180 - Drop for item Old fashioned brass lamp - Input: DRO LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 17| LAM |
| Condition| ConditionID 0 ArgID 10| item 'Old fashioned brass lamp(index:10)' carried |
| Action| ActionID 53 ArgID 10| drops item 'Old fashioned brass lamp(index:10)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 181 - Take for item Rusty axe (Magic word `BUNYON` on it) - Input: GET AXE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 11| AXE |
| Condition| ConditionID 1 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' in room with player |
| Action| ActionID 52 ArgID 11| get item 'Rusty axe (Magic word `BUNYON` on it)(index:11)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 182 - Drop for item Rusty axe (Magic word `BUNYON` on it) - Input: DRO AXE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 11| AXE |
| Condition| ConditionID 0 ArgID 11| item 'Rusty axe \(Magic word `BUNYON` on it\)(index:11)' carried |
| Action| ActionID 53 ArgID 11| drops item 'Rusty axe (Magic word `BUNYON` on it)(index:11)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 183 - Take for item Water in bottle - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| BOT |
| Condition| ConditionID 1 ArgID 12| item 'Water in bottle(index:12)' in room with player |
| Action| ActionID 52 ArgID 12| get item 'Water in bottle(index:12)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 184 - Drop for item Water in bottle - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| BOT |
| Condition| ConditionID 0 ArgID 12| item 'Water in bottle(index:12)' carried |
| Action| ActionID 53 ArgID 12| drops item 'Water in bottle(index:12)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 185 - Take for item Empty bottle - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| BOT |
| Condition| ConditionID 1 ArgID 13| item 'Empty bottle(index:13)' in room with player |
| Action| ActionID 52 ArgID 13| get item 'Empty bottle(index:13)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 186 - Drop for item Empty bottle - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| BOT |
| Condition| ConditionID 0 ArgID 13| item 'Empty bottle(index:13)' carried |
| Action| ActionID 53 ArgID 13| drops item 'Empty bottle(index:13)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 187 - Take for item Ring of skeleton keys - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 30| KEY |
| Condition| ConditionID 1 ArgID 14| item 'Ring of skeleton keys(index:14)' in room with player |
| Action| ActionID 52 ArgID 14| get item 'Ring of skeleton keys(index:14)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 188 - Drop for item Ring of skeleton keys - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 30| KEY |
| Condition| ConditionID 0 ArgID 14| item 'Ring of skeleton keys(index:14)' carried |
| Action| ActionID 53 ArgID 14| drops item 'Ring of skeleton keys(index:14)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 189 - Take for item *GOLDEN NET* - Input: GET NET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 7| NET |
| Condition| ConditionID 1 ArgID 19| item '\*GOLDEN NET\*(index:19)' in room with player |
| Action| ActionID 52 ArgID 19| get item '*GOLDEN NET*(index:19)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 190 - Drop for item *GOLDEN NET* - Input: DRO NET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 7| NET |
| Condition| ConditionID 0 ArgID 19| item '\*GOLDEN NET\*(index:19)' carried |
| Action| ActionID 53 ArgID 19| drops item '*GOLDEN NET*(index:19)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 191 - Take for item Patches of `OILY` slime - Input: GET OIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 28| OIL |
| Condition| ConditionID 1 ArgID 22| item 'Patches of `OILY` slime(index:22)' in room with player |
| Action| ActionID 52 ArgID 22| get item 'Patches of `OILY` slime(index:22)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 192 - Drop for item Patches of `OILY` slime - Input: DRO OIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 28| OIL |
| Condition| ConditionID 0 ArgID 22| item 'Patches of `OILY` slime(index:22)' carried |
| Action| ActionID 53 ArgID 22| drops item 'Patches of `OILY` slime(index:22)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 193 - Take for item *ROYAL HONEY* - Input: GET HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 42| HON |
| Condition| ConditionID 1 ArgID 23| item '\*ROYAL HONEY\*(index:23)' in room with player |
| Action| ActionID 52 ArgID 23| get item '*ROYAL HONEY*(index:23)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 194 - Drop for item *ROYAL HONEY* - Input: DRO HON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 42| HON |
| Condition| ConditionID 0 ArgID 23| item '\*ROYAL HONEY\*(index:23)' carried |
| Action| ActionID 53 ArgID 23| drops item '*ROYAL HONEY*(index:23)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 195 - Take for item Bees in a bottle - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 14| BOT |
| Condition| ConditionID 1 ArgID 26| item 'Bees in a bottle(index:26)' in room with player |
| Action| ActionID 52 ArgID 26| get item 'Bees in a bottle(index:26)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 196 - Drop for item Bees in a bottle - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 14| BOT |
| Condition| ConditionID 0 ArgID 26| item 'Bees in a bottle(index:26)' carried |
| Action| ActionID 53 ArgID 26| drops item 'Bees in a bottle(index:26)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 197 - Take for item Flint & steel - Input: GET FLI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 26| FLI |
| Condition| ConditionID 1 ArgID 28| item 'Flint & steel(index:28)' in room with player |
| Action| ActionID 52 ArgID 28| get item 'Flint & steel(index:28)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 198 - Drop for item Flint & steel - Input: DRO FLI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 26| FLI |
| Condition| ConditionID 0 ArgID 28| item 'Flint & steel(index:28)' carried |
| Action| ActionID 53 ArgID 28| drops item 'Flint & steel(index:28)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 199 - Take for item *Thick PERSIAN RUG* - Input: GET RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 40| RUG |
| Condition| ConditionID 1 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' in room with player |
| Action| ActionID 52 ArgID 29| get item '*Thick PERSIAN RUG*(index:29)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 200 - Drop for item *Thick PERSIAN RUG* - Input: DRO RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 40| RUG |
| Condition| ConditionID 0 ArgID 29| item '\*Thick PERSIAN RUG\*(index:29)' carried |
| Action| ActionID 53 ArgID 29| drops item '*Thick PERSIAN RUG*(index:29)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 201 - Take for item Distended gas bladder - Input: GET BLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 50| BLA |
| Condition| ConditionID 1 ArgID 31| item 'Distended gas bladder(index:31)' in room with player |
| Action| ActionID 52 ArgID 31| get item 'Distended gas bladder(index:31)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 202 - Drop for item Distended gas bladder - Input: DRO BLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 50| BLA |
| Condition| ConditionID 0 ArgID 31| item 'Distended gas bladder(index:31)' carried |
| Action| ActionID 53 ArgID 31| drops item 'Distended gas bladder(index:31)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 203 - Take for item Loose fire bricks - Input: GET BRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 37| BRI |
| Condition| ConditionID 1 ArgID 36| item 'Loose fire bricks(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Loose fire bricks(index:36)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 204 - Drop for item Loose fire bricks - Input: DRO BRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 37| BRI |
| Condition| ConditionID 0 ArgID 36| item 'Loose fire bricks(index:36)' carried |
| Action| ActionID 53 ArgID 36| drops item 'Loose fire bricks(index:36)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 205 - Take for item *GOLD CROWN* - Input: GET CRO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 36| CRO |
| Condition| ConditionID 1 ArgID 37| item '\*GOLD CROWN\*(index:37)' in room with player |
| Action| ActionID 52 ArgID 37| get item '*GOLD CROWN*(index:37)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 206 - Drop for item *GOLD CROWN* - Input: DRO CRO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 36| CRO |
| Condition| ConditionID 0 ArgID 37| item '\*GOLD CROWN\*(index:37)' carried |
| Action| ActionID 53 ArgID 37| drops item '*GOLD CROWN*(index:37)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 207 - Take for item Empty wine bladder - Input: GET BLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 50| BLA |
| Condition| ConditionID 1 ArgID 40| item 'Empty wine bladder(index:40)' in room with player |
| Action| ActionID 52 ArgID 40| get item 'Empty wine bladder(index:40)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 208 - Drop for item Empty wine bladder - Input: DRO BLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 50| BLA |
| Condition| ConditionID 0 ArgID 40| item 'Empty wine bladder(index:40)' carried |
| Action| ActionID 53 ArgID 40| drops item 'Empty wine bladder(index:40)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 209 - Take for item Broken glass - Input: GET GLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 63| GLA |
| Condition| ConditionID 1 ArgID 41| item 'Broken glass(index:41)' in room with player |
| Action| ActionID 52 ArgID 41| get item 'Broken glass(index:41)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 210 - Drop for item Broken glass - Input: DRO GLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 63| GLA |
| Condition| ConditionID 0 ArgID 41| item 'Broken glass(index:41)' carried |
| Action| ActionID 53 ArgID 41| drops item 'Broken glass(index:41)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 211 - Take for item Chiggers - Input: GET CHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 46| CHI |
| Condition| ConditionID 1 ArgID 42| item 'Chiggers(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Chiggers(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 212 - Drop for item Chiggers - Input: DRO CHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 46| CHI |
| Condition| ConditionID 0 ArgID 42| item 'Chiggers(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Chiggers(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 213 - Take for item *DRAGON EGGS* (very rare) - Input: GET EGG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 27| EGG |
| Condition| ConditionID 1 ArgID 44| item '\*DRAGON EGGS\* \(very rare\)(index:44)' in room with player |
| Action| ActionID 52 ArgID 44| get item '*DRAGON EGGS* (very rare)(index:44)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 214 - Drop for item *DRAGON EGGS* (very rare) - Input: DRO EGG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 27| EGG |
| Condition| ConditionID 0 ArgID 44| item '\*DRAGON EGGS\* \(very rare\)(index:44)' carried |
| Action| ActionID 53 ArgID 44| drops item '*DRAGON EGGS* (very rare)(index:44)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 215 - Take for item *JEWELED FRUIT* - Input: GET FRU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 43| FRU |
| Condition| ConditionID 1 ArgID 46| item '\*JEWELED FRUIT\*(index:46)' in room with player |
| Action| ActionID 52 ArgID 46| get item '*JEWELED FRUIT*(index:46)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 216 - Drop for item *JEWELED FRUIT* - Input: DRO FRU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 43| FRU |
| Condition| ConditionID 0 ArgID 46| item '\*JEWELED FRUIT\*(index:46)' carried |
| Action| ActionID 53 ArgID 46| drops item '*JEWELED FRUIT*(index:46)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 217 - Take for item *Small statue of a BLUE OX* - Input: GET OX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| OX |
| Condition| ConditionID 1 ArgID 47| item '\*Small statue of a BLUE OX\*(index:47)' in room with player |
| Action| ActionID 52 ArgID 47| get item '*Small statue of a BLUE OX*(index:47)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 218 - Drop for item *Small statue of a BLUE OX* - Input: DRO OX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| OX |
| Condition| ConditionID 0 ArgID 47| item '\*Small statue of a BLUE OX\*(index:47)' carried |
| Action| ActionID 53 ArgID 47| drops item '*Small statue of a BLUE OX*(index:47)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 219 - Take for item *DIAMOND RING* - Input: GET RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 45| RIN |
| Condition| ConditionID 1 ArgID 48| item '\*DIAMOND RING\*(index:48)' in room with player |
| Action| ActionID 52 ArgID 48| get item '*DIAMOND RING*(index:48)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 220 - Drop for item *DIAMOND RING* - Input: DRO RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 45| RIN |
| Condition| ConditionID 0 ArgID 48| item '\*DIAMOND RING\*(index:48)' carried |
| Action| ActionID 53 ArgID 48| drops item '*DIAMOND RING*(index:48)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 221 - Take for item *DIAMOND BRACELET* - Input: GET BRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 48| BRA |
| Condition| ConditionID 1 ArgID 49| item '\*DIAMOND BRACELET\*(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item '*DIAMOND BRACELET*(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 222 - Drop for item *DIAMOND BRACELET* - Input: DRO BRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 48| BRA |
| Condition| ConditionID 0 ArgID 49| item '\*DIAMOND BRACELET\*(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item '*DIAMOND BRACELET*(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 223 - Take for item Dead fish - Input: GET FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 8| FIS |
| Condition| ConditionID 1 ArgID 55| item 'Dead fish(index:55)' in room with player |
| Action| ActionID 52 ArgID 55| get item 'Dead fish(index:55)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 224 - Drop for item Dead fish - Input: DRO FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 8| FIS |
| Condition| ConditionID 0 ArgID 55| item 'Dead fish(index:55)' carried |
| Action| ActionID 53 ArgID 55| drops item 'Dead fish(index:55)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 225 - Take for item *FIRESTONE* (cold now) - Input: GET FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 59| FIR |
| Condition| ConditionID 1 ArgID 56| item '\*FIRESTONE\* \(cold now\)(index:56)' in room with player |
| Action| ActionID 52 ArgID 56| get item '*FIRESTONE* (cold now)(index:56)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 226 - Drop for item *FIRESTONE* (cold now) - Input: DRO FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 59| FIR |
| Condition| ConditionID 0 ArgID 56| item '\*FIRESTONE\* \(cold now\)(index:56)' carried |
| Action| ActionID 53 ArgID 56| drops item '*FIRESTONE* (cold now)(index:56)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 227 - Take for item Empty lamp - Input: GET LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 17| LAM |
| Condition| ConditionID 1 ArgID 60| item 'Empty lamp(index:60)' in room with player |
| Action| ActionID 52 ArgID 60| get item 'Empty lamp(index:60)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 228 - Drop for item Empty lamp - Input: DRO LAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 17| LAM |
| Condition| ConditionID 0 ArgID 60| item 'Empty lamp(index:60)' carried |
| Action| ActionID 53 ArgID 60| drops item 'Empty lamp(index:60)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 229 - Take for item Muddy worthless old rug - Input: GET RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 40| RUG |
| Condition| ConditionID 1 ArgID 61| item 'Muddy worthless old rug(index:61)' in room with player |
| Action| ActionID 52 ArgID 61| get item 'Muddy worthless old rug(index:61)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 230 - Drop for item Muddy worthless old rug - Input: DRO RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 40| RUG |
| Condition| ConditionID 0 ArgID 61| item 'Muddy worthless old rug(index:61)' carried |
| Action| ActionID 53 ArgID 61| drops item 'Muddy worthless old rug(index:61)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 231 - Take for item Large outdoor Advertisement - Input: GET ADV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 62| ADV |
| Condition| ConditionID 1 ArgID 62| item 'Large outdoor Advertisement(index:62)' in room with player |
| Action| ActionID 52 ArgID 62| get item 'Large outdoor Advertisement(index:62)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 232 - Drop for item Large outdoor Advertisement - Input: DRO ADV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 62| ADV |
| Condition| ConditionID 0 ArgID 62| item 'Large outdoor Advertisement(index:62)' carried |
| Action| ActionID 53 ArgID 62| drops item 'Large outdoor Advertisement(index:62)' into current room |
| Action| ActionID 64 ArgID 0| look |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUT| 0|  |
| GO| 1| ENT, RUN, WAL, CLI |
| JUM| 6|  |
| AT| 7|  |
| CHO| 8| CUT |
| GET| 10| TAK, PIC, CAT |
| LIG| 14| ., IGN, BUR |
| DRO| 18| REL, SPI, LEA, GIV, POU |
| THR| 24| TOS |
| QUI| 26|  |
| SWI| 27|  |
| RUB| 28|  |
| LOO| 29| EXA, DES |
| STO| 32|  |
| SCO| 33|  |
| INV| 34|  |
| SAV| 35|  |
| WAK| 36|  |
| UNL| 37|  |
| REA| 38|  |
| ATT| 39| SLA, KIL |
| DRI| 42| EAT |
| \.| 44|  |
| FIN| 45| LOC |
| HEL| 47|  |
| SAY| 48| SPE, CAL |
| SCR| 51| YEL, HOL |
| \.| 54|  |
| FIL| 55|  |
| CRO| 56|  |
| DAM| 57|  |
| MAK| 58| BUI |
| WAV| 60| TIC, KIC, KIS, TOU, FEE, FUC, HIT, POK |
| OPE| 69|  |
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
| NET| 7|  |
| FIS| 8|  |
| AWA| 9|  |
| MIR| 10|  |
| AXE| 11| AX |
| WAT| 13|  |
| BOT| 14| CON |
| HOL| 16|  |
| LAM| 17|  |
| SPI| 18|  |
| WIN| 19|  |
| DOO| 20|  |
| MUD| 21| MED |
| BEE| 23|  |
| ROC| 24|  |
| GAS| 25|  |
| FLI| 26|  |
| EGG| 27|  |
| OIL| 28| SLI |
| KEY| 30|  |
| HEL| 31|  |
| BUN| 32|  |
| INV| 33|  |
| LED| 34|  |
| THR| 35|  |
| CRO| 36|  |
| BRI| 37|  |
| BEA| 38|  |
| DRA| 39|  |
| RUG| 40|  |
| RUB| 41|  |
| HON| 42|  |
| FRU| 43|  |
| OX| 44|  |
| RIN| 45|  |
| CHI| 46| BIT |
| BRA| 48|  |
| SIG| 49|  |
| BLA| 50|  |
| WEB| 51| WRI |
| SWA| 53|  |
| LAV| 54| DAM |
| HAL| 56|  |
| TRE| 57| STU |
| FIR| 59|  |
| SHO| 60| BAN |
| ADV| 62|  |
| GLA| 63|  |
| ARO| 64|  |
| GAM| 65|  |
| BOO| 66|  |
| CHA| 67|  |
| LAK| 68|  |
| YOH| 69|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| | 7, 10, 1, 24 |
| 1| dismal swamp| 23, 29, 25 |
| 2| top of a tall cypress tree| 1 |
| 3| damp hollow stump in the swamp| 1, 4 |
| 4| root chamber under the stump| 3 |
| 5| semi\-dark hole by the root chamber| 4 |
| 6| long down sloping hall| 5, 7 |
| 7| large cavern| 31, 9, 27, 6, 12 |
| 8| large 8 sided room| 31 |
| 9| royal anteroom| 7, 20 |
| 10| \*I'm on the shore of a lake| 26, 29, 23 |
| 11| forest| 11, 11, 23, 11 |
| 12| maze of pits| 13, 15, 15, 13 |
| 13| maze of pits| 14, 12 |
| 14| maze of pits| 17, 12, 13, 16, 16, 17 |
| 15| maze of pits| 12, 13, 12, 13 |
| 16| maze of pits| 17, 14, 17 |
| 17| maze of pits| 17, 12, 12, 15, 14, 18 |
| 18| \*I'm at the bottom of a very deep chasm\. High above me is a pair of ledges\. One has a bricked up window across its face the other faces a Throne\-room| 17 |
| 19| \*I'm on a narrow ledge by a chasm\. Across the chasm is the Throne\-room| 20 |
| 20| royal chamber| 9 |
| 21| \*I'm on a narrow ledge by a Throne\-room Across the chasm is another ledge|  |
| 22| throne room| 21 |
| 23| sunny meadow| 1, 10, 11 |
| 24| \*I think I'm in real trouble now\. There's a fellow here with a pitchfork and pointed tail\. \.\.\.Oh Hell\!|  |
| 25| hidden grove| 11, 1 |
| 26| quick\-sand bog|  |
| 27| Memory chip of a COMPUTER\! I took a wrong turn\!| 7 |
| 28| top of an oak\. To the East I see a meadow, beyond that a lake\.| 11 |
| 29| \*I'm at the edge of a BOTTOMLESS hole| 10, 1 |
| 30| \*I'm on a ledge just below the rim of the BOTTOMLESS hole\. I don't think I want to go down| 29, 24 |
| 31| long tunnel\. I hear buzzing ahead| 8, 7 |
| 32| \*I'm in an endless corridor| 32, 33, 32, 32, 32, 32 |
| 33| large misty room with strange unreadable letters over all the exits\.| 32, 24, 11, 24, 28, 24 |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| Nothing happens |
| 2| Chop 'er down\! |
| 3| BOY that really hit the spot\! |
| 4| Dragon smells something\. Awakens & attacks me\! |
| 5| Lock shatters |
| 6| I can't its locked |
| 7| TIMBER\. Something fell from the tree top & vanished in the swamp |
| 8| TIMBER\! |
| 9| Lamp is off |
| 10| Lamp burns with a cold flameless blue glow\. |
| 11| I'm bit by a spider |
| 12|  My chigger bites are now INFECTED\!  |
| 13| My bites have rotted my whole body\! |
| 14| Bear eats the honey and falls asleep\. |
| 15| Bees sting me |
| 16| First I need an empty container\. |
| 17| The bees all suffocated and disappeared |
| 18| Something I'm holding vibrates and\.\.\. |
| 19| nothing to light it with |
| 20| Gas bladder blew up |
| 21| in my hands\! |
| 22| gas needs to be contained before it will burn |
| 23| Gas dissipates\. \(I think you blew it\) |
| 24| That won't ignite |
| 25| How? |
| 26| Bear won't let me |
| 27| `Don't waste honey, get mad instead\! Dam lava\!?` |
| 28| Bees madden bear, bear then attacks me\! |
| 29| It soaks into the ground |
| 30| In 2 words tell me at what\.\.\.like: AT TREE |
| 31| OH NO\.\.\. Bear dodges\.\.\. CRASH\! |
| 32| Its heavy\! |
| 33| Somethings too heavy\. I fall\. |
| 34| To stop game say QUIT |
| 35| Mirror hits floor and shatters into a MILLION pieces |
| 36| Mirror lands softly on rug, lights up and says: |
| 37| You lost \*ALL\* treasures\. |
| 38| I'm not carrying ax, take inventory\! |
| 39| It doesn't seem to bother him at all\! |
| 40| The mud dried up and fell off\. |
| 41| Bear is so startled that he FELL off the ledge\! |
| 42| ` DRAGON STING ` and fades\. I don't get it, I hope you do\. |
| 43| The bees attack the dragon which gets so annoyed it gets up and flys away\.\.\. |
| 44| Lamp is now full & lit |
| 45|  I'm bitten by chiggers\.  |
| 46| There's something there all right\! Maybe I should go there? |
| 47| Maybe if I threw something?\.\.\. |
| 48| Too dry, the fish died\. |
| 49| A glowing Genie appears, drops somehting, then vanishes\. |
| 50| A glowing Genie appears, says `Boy you're selfish`, takes something and then makes `ME` vanish\! |
| 51| No, its too hot\. |
| 52| Not here\. |
| 53| Try the swamp |
| 54| Sizzle\.\.\. |
| 55| Try \-\-\> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP` and any other verbs you can think of\.\.\. |
| 56| There are only 3 ways to wake the Dragon\! |
| 57| Remember you can always say `HELP` |
| 58| Read the sign in the meadow\! |
| 59| You may need to say magic words here |
| 60| A voice BOOOOMS out: |
| 61| please leave it alone |
| 62| Sorry, I can only throw the ax\. |
| 63| Medicine is good for bites\. |
| 64| I don't know where it is |
| 65|  Welcome to Adventure number: 1 `ADVENTURELAND`\. In this Adventure you're to find \*TREASURES\* & store them away\.  To see how well you're doing say: `SCORE` |
| 66| Blow it up\! |
| 67| Fish have escaped back to the lake\. |
| 68| OK |
| 69| Huh? I don't think so\! |
| 70| You might try examining things\.\.\. |
| 71| What? |
| 72| OK, I threw it\. |
| 73|  Check with your favorite computer dealer for the next Adventure program: PIRATE ADVENTURE\. If they don't carry `ADVENTURE` have them call: 1\-305\-862\-6917 today\!  |
| 74| The ax vibrated\! |
| 75| I see nothing special |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Glowing \*FIRESTONE\*| | 0 |
| 1| Dark hole| | 4 |
| 2| \*Pot of RUBIES\*| RUB| 4 |
| 3| Spider web with writing on it| | 2 |
| 4| \-HOLLOW\- stump and remains of a felled tree| | 0 |
| 5| Cypress tree| | 1 |
| 6| Water| | 10 |
| 7| Evil smelling mud| MUD| 1 |
| 8| \*GOLDEN FISH\*| FIS| 10 |
| 9| Lit brass lamp| LAM| 0 |
| 10| Old fashioned brass lamp| LAM| 3 |
| 11| Rusty axe \(Magic word `BUNYON` on it\)| AXE| 10 |
| 12| Water in bottle| BOT| 3 |
| 13| Empty bottle| BOT| 0 |
| 14| Ring of skeleton keys| KEY| 2 |
| 15| Sign `Leave \*TREASURES\* here, then say: SCORE`| | 3 |
| 16| Locked door| | 5 |
| 17| Open door with a hallway beyond| | 0 |
| 18| Swamp gas| | 1 |
| 19| \*GOLDEN NET\*| NET| 18 |
| 20| Chigger bites| | 0 |
| 21| Infected chigger bites| | 0 |
| 22| Patches of `OILY` slime| OIL| 1 |
| 23| \*ROYAL HONEY\*| HON| 8 |
| 24| Large african bees| | 8 |
| 25| Very thin black bear| | 21 |
| 26| Bees in a bottle| BOT| 0 |
| 27| Large sleeping dragon| | 23 |
| 28| Flint & steel| FLI| 30 |
| 29| \*Thick PERSIAN RUG\*| RUG| 17 |
| 30| Sign: `magic word's AWAY\! Look la\.\.\.` \(Rest of sign is missing\!\)| | 18 |
| 31| Distended gas bladder| BLA| 0 |
| 32| Bricked up window| | 20 |
| 33| Sign here says `In many cases mud is good\. In others\.\.\.`| | 23 |
| 34| Stream of lava| | 18 |
| 35| Bricked up window with a hole in it| | 0 |
| 36| Loose fire bricks| BRI| 0 |
| 37| \*GOLD CROWN\*| CRO| 22 |
| 38| \*MAGIC MIRROR\*| | 21 |
| 39| Sleeping bear| | 0 |
| 40| Empty wine bladder| BLA| 9 |
| 41| Broken glass| GLA| 0 |
| 42| Chiggers| CHI| 1 |
| 43| Slightly woozy bear| | 0 |
| 44| \*DRAGON EGGS\* \(very rare\)| EGG| 0 |
| 45| Lava stream with brick dam| | 0 |
| 46| \*JEWELED FRUIT\*| FRU| 25 |
| 47| \*Small statue of a BLUE OX\*| OX| 26 |
| 48| \*DIAMOND RING\*| RIN| 0 |
| 49| \*DIAMOND BRACELET\*| BRA| 0 |
| 50| Strange scratchings on rock says: `ALADIN was here`| | 14 |
| 51| Sign says `LIMBO\. Find right exit and live again\!`| | 33 |
| 52| Smoking hole\. pieces of dragon and gore\.| | 0 |
| 53| Sign says `No swimming allowed here`| | 10 |
| 54| Arrow pointing down| | 17 |
| 55| Dead fish| FIS| 0 |
| 56| \*FIRESTONE\* \(cold now\)| FIR| 0 |
| 57| Sign says `Paul's place`| | 25 |
| 58| Trees| | 11 |
| 59| Sign here says `Opposite of LIGHT is UNLIGHT`| | 12 |
| 60| Empty lamp| LAM| 0 |
| 61| Muddy worthless old rug| RUG| 0 |
| 62| Large outdoor Advertisement| ADV| 29 |
| 63| Hole| | 29 |
| 64| | | 0 |
| 65| | | 0 |