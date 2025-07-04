# Voodcastle Datfile
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
| adventureNumber| 4 |
| Unknown| 0 |
| numItems| 66 |
| numActions| 190 |
| numNounVerbs| 90 |
| numRooms| 26 |
| maxCarry| 9 |
| startRoom| 1 |
| totalTreasures| 0 |
| wordLength| 3 |
| lightDuration| 15000 |
| numMessages| 100 |
| treasureRoom| 0 |
## Actions
### Action 0 - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 202, 0, 0, 0, 0, 1950, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 1 ArgID 10| item 'Open Window(index:10)' in room with player |
| Action| ActionID 13 | Print message 'Raven crys something outside' |
### Action 1 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 184, 202, 292, 200, 380, 1272, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 1 ArgID 10| item 'Open Window(index:10)' in room with player |
| Condition| ConditionID 11 ArgID 14| item 'Four leaf clover(index:14)' not carried or in room with player |
| Action| ActionID 8 | Print message 'Window just slAmmed shut' |
| Action| ActionID 72 ArgID 10, 19| swap item locations 'Open Window(index:10)' and 'Closed Window(index:19)' |
### Action 2 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 187, 393, 200, 380, 0, 10800, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 6 ArgID 9| player not in room 9 |
| Condition| ConditionID 12 ArgID 19| item 'Closed Window(index:19)' in game |
| Action| ActionID 72 ArgID 10, 19| swap item locations 'Open Window(index:10)' and 'Closed Window(index:19)' |
### Action 3 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 4 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 5 - Probability: 45 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 45, 384, 294, 0, 0, 0, 4200, 0|  |
| Probability| 45%|  |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Condition| ConditionID 13 ArgID 14| item 'Four leaf clover(index:14)' not in game |
| Action| ActionID 28 | Print message 'A beam of light shines on grave' |
### Action 6 - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 723, 146, 500, 0, 0, 8164, 2173|  |
| Probability| 30%|  |
| Condition| ConditionID 2 ArgID 36| item 'Chem tubes(index:36)' carried or in room with player |
| Condition| ConditionID 5 ArgID 7| item 'Shield(index:7)' not carried |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 64 | look |
| Action| ActionID 14 | Print message 'One of the test tubes EXPLODED\!' |
| Action| ActionID 73 | continue with next action |
### Action 7 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 3631, 0|  |
| Probability| 0%|  |
| Action| ActionID 24 | Print message 'A sign here says:' |
| Action| ActionID 31 | Print message 'This grAve reserved for you\!' |
### Action 8 - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 723, 141, 0, 0, 0, 2100, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 2 ArgID 36| item 'Chem tubes(index:36)' carried or in room with player |
| Condition| ConditionID 0 ArgID 7| item 'Shield(index:7)' carried |
| Action| ActionID 14 | Print message 'One of the test tubes EXPLODED\!' |
### Action 9 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 10 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 304, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 11 - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 421, 220, 204, 0, 0, 6054, 0|  |
| Probability| 50%|  |
| Condition| ConditionID 0 ArgID 21| item 'Soot(index:21)' carried |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 40 | Print message 'Maid chased me with broom for tracking soot through the Ball\- room\. I wonder where I am?' |
| Action| ActionID 54 ArgID 11| move room 11 |
### Action 12 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 64, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 13 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 14 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 364, 713, 0, 0, 0, 15600, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Condition| ConditionID 12 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in game |
| Action| ActionID 104 | Print message 'I hear strange sounds, as if someone were moaning\.' |
### Action 15 - Probability: 35 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 35, 284, 713, 0, 0, 0, 15600, 0|  |
| Probability| 35%|  |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Condition| ConditionID 12 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in game |
| Action| ActionID 104 | Print message 'I hear strange sounds, as if someone were moaning\.' |
### Action 16 - Probability: 35 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 35, 304, 713, 0, 0, 0, 15600, 0|  |
| Probability| 35%|  |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 12 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in game |
| Action| ActionID 104 | Print message 'I hear strange sounds, as if someone were moaning\.' |
### Action 17 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 504, 0, 0, 0, 0, 6963, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 46 | Print message 'Luck wasn't with me\!' |
| Action| ActionID 63 | game over |
### Action 18 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 149, 140, 0, 0, 0, 18808, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 7| bitflag 7 is false |
| Action| ActionID 125 | Print message 'Welcome to ADVENTURE:4, `VOODOO CASTLE` by Alexis ADAMS\. Dedicated to all MOMS\!' |
| Action| ActionID 58 ArgID 7| set 7 flag |
### Action 19 - Probability: 7 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7, 861, 0, 0, 0, 0, 19481, 0|  |
| Probability| 7%|  |
| Condition| ConditionID 0 ArgID 43| item 'Dusty Idol(index:43)' carried |
| Action| ActionID 129 | Print message 'My idol acted strange' |
| Action| ActionID 131 | Print message 'Some dust fell off it and it glowed briefly\.' |
### Action 20 - Probability: 35 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 35, 583, 0, 0, 0, 0, 21150, 0|  |
| Probability| 35%|  |
| Condition| ConditionID 2 ArgID 29| item 'Ju\-Ju man(index:29)' carried or in room with player |
| Action| ActionID 141 | Print message 'I hear someone mumbling\.' |
### Action 21 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 22 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 23 - Input: GET SWE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1552, 702, 0, 0, 0, 0, 16650, 0|  |
| Verb| 10| GET |
| Noun| 52| SWE |
| Condition| ConditionID 1 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in room with player |
| Action| ActionID 111 | Print message 'won't budge\!' |
### Action 24 - Input: GET GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 1183, 1180, 0, 0, 0, 3052, 0|  |
| Verb| 10| GET |
| Noun| 20| GRA |
| Condition| ConditionID 2 ArgID 59| item 'Broken grating(index:59)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 52 ArgID 59| get item 'Broken grating(index:59)', check if can carry |
### Action 25 - Input: WAV BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3644, 164, 634, 523, 620, 1220, 4888, 13272|  |
| Verb| 24| WAV |
| Noun| 44| BAG |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Condition| ConditionID 13 ArgID 31| item 'Wide crack in the wall(index:31)' not in game |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 72 ArgID 31, 61| swap item locations 'Wide crack in the wall(index:31)' and 'Crack in the wall(index:61)' |
### Action 26 - Input: OPE CEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5767, 286, 0, 0, 0, 0, 750, 0|  |
| Verb| 38| OPE |
| Noun| 67| CEL |
| Condition| ConditionID 5 ArgID 14| item 'Four leaf clover(index:14)' not carried |
| Action| ActionID 5 | Print message 'I can't do that' |
### Action 27 - Input: GO CEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 217, 1122, 285, 420, 0, 0, 10622, 8164|  |
| Verb| 1| GO |
| Noun| 67| CEL |
| Condition| ConditionID 1 ArgID 56| item 'Open jail cell(index:56)' in room with player |
| Condition| ConditionID 4 ArgID 14| item 'Four leaf clover(index:14)' not in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 122 | Print message 'Cell door slams shut' |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 64 | look |
### Action 28 - Input: LOO WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6325, 43, 0, 0, 0, 0, 2700, 0|  |
| Verb| 42| LOO |
| Noun| 25| WRI |
| Condition| ConditionID 2 ArgID 2| item 'Plaque(index:2)' carried or in room with player |
| Action| ActionID 18 | Print message 'There's something written there' |
### Action 29 - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 10| GET |
| Noun| 10| INV |
| Action| ActionID 66 | output inventory |
### Action 30 - Input: BRE WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4815, 382, 0, 0, 0, 0, 2250, 0|  |
| Verb| 32| BRE |
| Noun| 15| WIN |
| Condition| ConditionID 1 ArgID 19| item 'Closed Window(index:19)' in room with player |
| Action| ActionID 15 | Print message 'This glass can't be broken' |
### Action 31 - Input: MOV KET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4361, 102, 125, 120, 0, 0, 7970, 0|  |
| Verb| 29| MOV |
| Noun| 11| KET |
| Condition| ConditionID 1 ArgID 5| item 'Big kettle(index:5)' in room with player |
| Condition| ConditionID 4 ArgID 6| item 'Dark hole(index:6)' not in room with player |
| Action| ActionID 53 ArgID 6| drops item 'Dark hole(index:6)' into current room |
| Action| ActionID 20 | Print message 'OK' |
### Action 32 - Input: GET BAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1522, 362, 0, 0, 0, 0, 2852, 0|  |
| Verb| 10| GET |
| Noun| 22| BAL |
| Condition| ConditionID 1 ArgID 18| item 'Crystal Ball(index:18)' in room with player |
| Action| ActionID 19 | Print message 'A sepulchral voice says:' |
| Action| ActionID 2 | Print message 'It belongs to the medium' |
### Action 33 - Input: GET CLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1516, 282, 280, 0, 0, 0, 7800, 0|  |
| Verb| 10| GET |
| Noun| 16| CLO |
| Condition| ConditionID 1 ArgID 14| item 'Four leaf clover(index:14)' in room with player |
| Action| ActionID 52 ArgID 14| get item 'Four leaf clover(index:14)', check if can carry |
### Action 34 - Input: LOO GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6320, 302, 294, 0, 0, 0, 1824, 4650|  |
| Verb| 42| LOO |
| Noun| 20| GRA |
| Condition| ConditionID 1 ArgID 15| item 'GrAves(index:15)' in room with player |
| Condition| ConditionID 13 ArgID 14| item 'Four leaf clover(index:14)' not in game |
| Action| ActionID 12 | Print message 'Amongst the GRAVES is a four leaf clover\.' |
| Action| ActionID 24 | Print message 'A sign here says:' |
| Action| ActionID 31 | Print message 'This grAve reserved for you\!' |
### Action 35 - Input: GET CLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1516, 294, 384, 280, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 16| CLO |
| Condition| ConditionID 13 ArgID 14| item 'Four leaf clover(index:14)' not in game |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Action| ActionID 52 ArgID 14| get item 'Four leaf clover(index:14)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 36 - Input: LOO GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6320, 302, 293, 0, 0, 0, 3631, 0|  |
| Verb| 42| LOO |
| Noun| 20| GRA |
| Condition| ConditionID 1 ArgID 15| item 'GrAves(index:15)' in room with player |
| Condition| ConditionID 12 ArgID 14| item 'Four leaf clover(index:14)' in game |
| Action| ActionID 24 | Print message 'A sign here says:' |
| Action| ActionID 31 | Print message 'This grAve reserved for you\!' |
### Action 37 - Input: GO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 162, 400, 0, 0, 0, 10554, 9600|  |
| Verb| 1| GO |
| Noun| 43| STA |
| Condition| ConditionID 1 ArgID 8| item 'Stairs(index:8)' in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 54 ArgID 20| move room 20 |
| Action| ActionID 64 | look |
### Action 38 - Input: LOO SAF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6328, 742, 0, 0, 0, 0, 3150, 0|  |
| Verb| 42| LOO |
| Noun| 28| SAF |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 21 | Print message 'Safe's combination lock is numbered from 33 to 38\.' |
### Action 39 - Input: LOO SAF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6328, 682, 940, 954, 0, 0, 8067, 0|  |
| Verb| 42| LOO |
| Noun| 28| SAF |
| Condition| ConditionID 1 ArgID 34| item 'Open SAfe(index:34)' in room with player |
| Condition| ConditionID 13 ArgID 47| item 'Antique hammer(index:47)' not in game |
| Action| ActionID 53 ArgID 47| drops item 'Antique hammer(index:47)' into current room |
| Action| ActionID 117 | Print message 'There's an antique hammer here' |
### Action 40 - Input: OPE FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5735, 242, 240, 260, 220, 0, 10820, 7950|  |
| Verb| 38| OPE |
| Noun| 35| FLU |
| Condition| ConditionID 1 ArgID 12| item 'Closed Flue(index:12)' in room with player |
| Action| ActionID 72 ArgID 12, 13| swap item locations 'Closed Flue(index:12)' and 'Open Flue(index:13)' |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 53 ArgID 11| drops item 'Dark Chimney(index:11)' into current room |
### Action 41 - Input: CLO FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5885, 262, 240, 260, 220, 0, 10820, 8850|  |
| Verb| 39| CLO |
| Noun| 35| FLU |
| Condition| ConditionID 1 ArgID 13| item 'Open Flue(index:13)' in room with player |
| Action| ActionID 72 ArgID 12, 13| swap item locations 'Closed Flue(index:12)' and 'Open Flue(index:13)' |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 59 ArgID 11| Item 'Dark Chimney(index:11)' is removed from the game (put in room 0) |
### Action 42 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 162, 122, 320, 0, 0, 0, 8156, 10564|  |
| Verb| 1| GO |
| Noun| 12| HOL |
| Condition| ConditionID 1 ArgID 6| item 'Dark hole(index:6)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 43 - Input: GO FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 185, 304, 262, 280, 0, 0, 8454, 10564|  |
| Verb| 1| GO |
| Noun| 35| FLU |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 1 ArgID 13| item 'Open Flue(index:13)' in room with player |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 54 ArgID 14| move room 14 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 44 - Input: LOO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6387, 1203, 0, 0, 0, 0, 2700, 0|  |
| Verb| 42| LOO |
| Noun| 87| LEA |
| Condition| ConditionID 2 ArgID 60| item 'Advertising leaflet(index:60)' carried or in room with player |
| Action| ActionID 18 | Print message 'There's something written there' |
### Action 45 - Input: LOO BAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6322, 124, 362, 80, 0, 0, 1554, 11403|  |
| Verb| 42| LOO |
| Noun| 22| BAL |
| Condition| ConditionID 3 ArgID 6| player in room 6 |
| Condition| ConditionID 1 ArgID 18| item 'Crystal Ball(index:18)' in room with player |
| Action| ActionID 10 | Print message 'I see nothing very special\.' |
| Action| ActionID 54 ArgID 4| move room 4 |
| Action| ActionID 76 | look |
| Action| ActionID 3 | Print message 'Spirit vibrations drive me from room\.' |
### Action 46 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 47 - Input: GO FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 184, 402, 300, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 34| FIR |
| Condition| ConditionID 1 ArgID 20| item 'Large fireplace(index:20)' in room with player |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 76 | look |
### Action 48 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5717, 264, 0, 0, 0, 0, 3000, 0|  |
| Verb| 38| OPE |
| Noun| 17| DOO |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Action| ActionID 20 | Print message 'OK' |
### Action 49 - Input: WAV RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3632, 482, 501, 560, 480, 0, 10822, 0|  |
| Verb| 24| WAV |
| Noun| 32| RIN |
| Condition| ConditionID 1 ArgID 24| item 'Massive stone door with a SAPPHIRE set into it(index:24)' in room with player |
| Condition| ConditionID 0 ArgID 25| item 'Sapphire ring(index:25)' carried |
| Action| ActionID 72 ArgID 28, 24| swap item locations 'Slick chute leading downward(index:28)' and 'Massive stone door with a SAPPHIRE set into it(index:24)' |
| Action| ActionID 22 | Print message 'Ring glows briefly & door vanishes' |
### Action 50 - Input: GO CHU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 168, 562, 160, 0, 0, 0, 3054, 11400|  |
| Verb| 1| GO |
| Noun| 18| CHU |
| Condition| ConditionID 1 ArgID 28| item 'Slick chute leading downward(index:28)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 51 - Input: GET RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 542, 514, 500, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 32| RIN |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Condition| ConditionID 13 ArgID 25| item 'Sapphire ring(index:25)' not in game |
| Action| ActionID 52 ArgID 25| get item 'Sapphire ring(index:25)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 52 - Input: DRI BRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7229, 323, 0, 0, 0, 0, 4888, 18063|  |
| Verb| 48| DRI |
| Noun| 29| BRE |
| Condition| ConditionID 2 ArgID 16| item 'Cast iron pot(index:16)' carried or in room with player |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 120 | Print message 'You've been turned into a broomstick & a witch rides off on you\!' |
| Action| ActionID 63 | game over |
### Action 53 - Input: OPE COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5708, 342, 340, 540, 0, 0, 10820, 0|  |
| Verb| 38| OPE |
| Noun| 8| COF |
| Condition| ConditionID 1 ArgID 17| item 'Closed Coffin(index:17)' in room with player |
| Action| ActionID 72 ArgID 17, 27| swap item locations 'Closed Coffin(index:17)' and 'Open Coffin(index:27)' |
| Action| ActionID 20 | Print message 'OK' |
### Action 54 - Input: CLO COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5858, 542, 340, 540, 0, 0, 10820, 0|  |
| Verb| 39| CLO |
| Noun| 8| COF |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Action| ActionID 72 ArgID 17, 27| swap item locations 'Closed Coffin(index:17)' and 'Open Coffin(index:27)' |
| Action| ActionID 20 | Print message 'OK' |
### Action 55 - Input: GET ARM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1530, 1142, 0, 0, 0, 0, 786, 0|  |
| Verb| 10| GET |
| Noun| 30| ARM |
| Condition| ConditionID 1 ArgID 57| item 'Knight's Suit of Armor(index:57)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 36 | Print message 'It's much to heavy to LIFT\!' |
### Action 56 - Input: BRE BAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4822, 124, 0, 0, 0, 0, 9178, 4713|  |
| Verb| 32| BRE |
| Noun| 22| BAL |
| Condition| ConditionID 3 ArgID 6| player in room 6 |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
| Action| ActionID 28 | Print message 'A beam of light shines on grave' |
| Action| ActionID 31 | Print message 'This grAve reserved for you\!' |
| Action| ActionID 63 | game over |
### Action 57 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5717, 482, 0, 0, 0, 0, 861, 0|  |
| Verb| 38| OPE |
| Noun| 17| DOO |
| Condition| ConditionID 1 ArgID 24| item 'Massive stone door with a SAPPHIRE set into it(index:24)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 111 | Print message 'won't budge\!' |
### Action 58 - Input: GET BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1544, 523, 593, 520, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 44| BAG |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Action| ActionID 52 ArgID 26| get item 'Ju-Ju bag(index:26)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 59 - Input: REA WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5275, 43, 83, 308, 0, 0, 4500, 0|  |
| Verb| 35| REA |
| Noun| 25| WRI |
| Condition| ConditionID 2 ArgID 2| item 'Plaque(index:2)' carried or in room with player |
| Condition| ConditionID 2 ArgID 4| item 'Broken glass(index:4)' carried or in room with player |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 30 | Print message 'Plaque says: `safe \-\-\> 38 33`' |
### Action 60 - Input: GO CHU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 168, 562, 160, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 18| CHU |
| Condition| ConditionID 1 ArgID 28| item 'Slick chute leading downward(index:28)' in room with player |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 61 - Input: GO CHU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 168, 602, 0, 0, 0, 0, 4050, 0|  |
| Verb| 1| GO |
| Noun| 18| CHU |
| Condition| ConditionID 1 ArgID 30| item 'Slippery chute leading up(index:30)' in room with player |
| Action| ActionID 27 | Print message 'I slide back down' |
### Action 62 - Input: LOO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6344, 523, 1054, 1093, 0, 0, 20100, 0|  |
| Verb| 42| LOO |
| Noun| 44| BAG |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Condition| ConditionID 13 ArgID 52| item 'Voodoo book(index:52)' not in game |
| Condition| ConditionID 12 ArgID 54| item 'Stick(index:54)' in game |
| Action| ActionID 134 | Print message 'There's a book there\.' |
### Action 63 - Input: CIR COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6758, 0, 24, 0, 0, 0, 10970, 988|  |
| Verb| 45| CIR |
| Noun| 8| COF |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
| Action| ActionID 88 | wait 2 seconds |
### Action 64 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 654, 183, 1, 60, 0, 8732, 8514|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 32| item 'Rabbit's foot(index:32)' not in game |
| Condition| ConditionID 2 ArgID 9| item 'Brightly glowing idol(index:9)' carried or in room with player |
| Condition| ConditionID 0 ArgID 0| item 'Bloody Knife(index:0)' carried |
| Action| ActionID 58 ArgID 3| set 3 flag |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 114 | Print message 'Its very dark, the only light is from the idol\.' |
### Action 65 - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6342, 803, 0, 0, 0, 0, 17850, 0|  |
| Verb| 42| LOO |
| Noun| 42| CHE |
| Condition| ConditionID 2 ArgID 40| item 'Mixed Chemicals(index:40)' carried or in room with player |
| Action| ActionID 119 | Print message 'Looks almost like lemonade\. Yummy\!' |
### Action 66 - Input: GET HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1540, 9, 663, 60, 740, 62, 7853, 3067|  |
| Verb| 10| GET |
| Noun| 40| HEA |
| Condition| ConditionID 8 ArgID 0| bitflag 0 is false |
| Condition| ConditionID 2 ArgID 33| item 'Dull & broken sword(index:33)' carried or in room with player |
| Condition| ConditionID 1 ArgID 3| item 'Animal heads(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Animal heads(index:3)', check if can carry |
| Action| ActionID 53 ArgID 37| drops item 'Closed SAfe(index:37)' into current room |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 67 | Set bit 0 true |
### Action 67 - Input: OPE SAF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5728, 104, 682, 0, 0, 0, 3000, 0|  |
| Verb| 38| OPE |
| Noun| 28| SAF |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 1 ArgID 34| item 'Open SAfe(index:34)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
### Action 68 - Input: LOO SAF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6328, 104, 682, 953, 0, 0, 3140, 0|  |
| Verb| 42| LOO |
| Noun| 28| SAF |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 1 ArgID 34| item 'Open SAfe(index:34)' in room with player |
| Condition| ConditionID 12 ArgID 47| item 'Antique hammer(index:47)' in game |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 140 | Print message 'Its empty\.' |
### Action 69 - Input: GET HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1540, 8, 63, 60, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 40| HEA |
| Condition| ConditionID 7 ArgID 0| bitflag 0 is set |
| Condition| ConditionID 2 ArgID 3| item 'Animal heads(index:3)' carried or in room with player |
| Action| ActionID 52 ArgID 3| get item 'Animal heads(index:3)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 70 - Input: TUR 38
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6037, 29, 742, 20, 0, 0, 8720, 0|  |
| Verb| 40| TUR |
| Noun| 37| 38 |
| Condition| ConditionID 8 ArgID 1| bitflag 1 is false |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 71 - Input: TUR 33
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6039, 28, 742, 680, 740, 0, 10820, 0|  |
| Verb| 40| TUR |
| Noun| 39| 33 |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 72 ArgID 34, 37| swap item locations 'Open SAfe(index:34)' and 'Closed SAfe(index:37)' |
| Action| ActionID 20 | Print message 'OK' |
### Action 72 - Input: LOO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6344, 523, 1094, 1054, 593, 0, 20235, 0|  |
| Verb| 42| LOO |
| Noun| 44| BAG |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Condition| ConditionID 13 ArgID 54| item 'Stick(index:54)' not in game |
| Condition| ConditionID 13 ArgID 52| item 'Voodoo book(index:52)' not in game |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Action| ActionID 134 | Print message 'There's a book there\.' |
| Action| ActionID 135 | Print message 'There's a stick there\.' |
### Action 73 - Input: REA BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5313, 1043, 0, 0, 0, 0, 16950, 0|  |
| Verb| 35| REA |
| Noun| 63| BOO |
| Condition| ConditionID 2 ArgID 52| item 'Voodoo book(index:52)' carried or in room with player |
| Action| ActionID 113 | Print message 'It's a book on removing curses\. Says: `With knife in hand you take a stand\. Circle coffin and\.\.\.` The rest of the page is missing\!\!\!' |
### Action 74 - Input: YEL MED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9623, 474, 124, 460, 0, 0, 3085, 8096|  |
| Verb| 64| YEL |
| Noun| 23| MED |
| Condition| ConditionID 13 ArgID 23| item 'Spirit Medium(index:23)' not in game |
| Condition| ConditionID 3 ArgID 6| player in room 6 |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 53 ArgID 23| drops item 'Spirit Medium(index:23)' into current room |
| Action| ActionID 146 | Print message 'Medium appears, says: `Keep a good luck charm on you & your friend\. I also see a \-moving\- bag helping you through a tight squeeze\!`' |
### Action 75 - Input: GO CHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 262, 280, 0, 0, 0, 8156, 11400|  |
| Verb| 1| GO |
| Noun| 24| CHI |
| Condition| ConditionID 1 ArgID 13| item 'Open Flue(index:13)' in room with player |
| Action| ActionID 54 ArgID 14| move room 14 |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 76 | look |
### Action 76 - Input: REA LAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5269, 763, 0, 0, 0, 0, 2550, 0|  |
| Verb| 35| REA |
| Noun| 19| LAB |
| Condition| ConditionID 2 ArgID 38| item 'Labeled chemicals(index:38)' carried or in room with player |
| Action| ActionID 17 | Print message 'They appear to be mixable\.' |
### Action 77 - Input: DRI CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7242, 803, 820, 440, 760, 0, 4873, 10859|  |
| Verb| 48| DRI |
| Noun| 42| CHE |
| Condition| ConditionID 2 ArgID 40| item 'Mixed Chemicals(index:40)' carried or in room with player |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 72 ArgID 41, 22| swap item locations 'Wide open door(index:41)' and 'Tiny open door(index:22)' |
| Action| ActionID 59 ArgID 38| Item 'Labeled chemicals(index:38)' is removed from the game (put in room 0) |
### Action 78 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 800, 0, 0, 0, 0, 8938, 13235|  |
| Probability| 0%|  |
| Action| ActionID 59 ArgID 40| Item 'Mixed Chemicals(index:40)' is removed from the game (put in room 0) |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 35 | Print message 'I'm now 4 feet tall\!' |
### Action 79 - Input: YEL ZAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9665, 1063, 1060, 580, 0, 0, 8903, 11035|  |
| Verb| 64| YEL |
| Noun| 65| ZAP |
| Condition| ConditionID 2 ArgID 53| item 'Ju\-Ju man statue(index:53)' carried or in room with player |
| Action| ActionID 59 ArgID 53| Item 'Ju-Ju man statue(index:53)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 29| drops item 'Ju-Ju man(index:29)' into current room |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 85 | echo noun |
### Action 80 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 17841, 0|  |
| Probability| 0%|  |
| Action| ActionID 118 | Print message 'There's a Clap of Thunder & then suddenly the stone statue begins to crack\. I may be in trouble now, there's someone in the room with me\!' |
| Action| ActionID 141 | Print message 'I hear someone mumbling\.' |
### Action 81 - Input: SAV GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5149, 0, 0, 0, 0, 0, 10650, 0|  |
| Verb| 34| SAV |
| Noun| 49| GAM |
| Action| ActionID 71 | save game |
### Action 82 - Input: GET KET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1511, 102, 0, 0, 0, 0, 786, 0|  |
| Verb| 10| GET |
| Noun| 11| KET |
| Condition| ConditionID 1 ArgID 5| item 'Big kettle(index:5)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 36 | Print message 'It's much to heavy to LIFT\!' |
### Action 83 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 167, 442, 0, 0, 0, 0, 787, 22050|  |
| Verb| 1| GO |
| Noun| 17| DOO |
| Condition| ConditionID 1 ArgID 22| item 'Tiny open door(index:22)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 37 | Print message 'I'm too big' |
| Action| ActionID 147 | Print message 'It will take some strong magic to get me through that\!' |
### Action 84 - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6600, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 44| INV |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
### Action 85 - Input: GET HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1540, 9, 63, 0, 0, 0, 16762, 0|  |
| Verb| 10| GET |
| Noun| 40| HEA |
| Condition| ConditionID 8 ArgID 0| bitflag 0 is false |
| Condition| ConditionID 2 ArgID 3| item 'Animal heads(index:3)' carried or in room with player |
| Action| ActionID 111 | Print message 'won't budge\!' |
| Action| ActionID 112 | Print message 'I'll need something to pry it off the wall\!' |
### Action 86 - Input: DRO FOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2747, 641, 0, 0, 0, 0, 5850, 0|  |
| Verb| 18| DRO |
| Noun| 47| FOO |
| Condition| ConditionID 0 ArgID 32| item 'Rabbit's foot(index:32)' carried |
| Action| ActionID 39 | Print message 'On what?' |
### Action 87 - Input: ON MAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3503, 643, 640, 542, 0, 0, 3032, 8850|  |
| Verb| 23| ON |
| Noun| 53| MAN |
| Condition| ConditionID 2 ArgID 32| item 'Rabbit's foot(index:32)' carried or in room with player |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 59 ArgID 32| Item 'Rabbit's foot(index:32)' is removed from the game (put in room 0) |
### Action 88 - Input: GET PIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1545, 882, 0, 0, 0, 0, 861, 0|  |
| Verb| 10| GET |
| Noun| 45| PIN |
| Condition| ConditionID 1 ArgID 44| item 'Doll(index:44)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 111 | Print message 'won't budge\!' |
### Action 89 - Input: PRE SWE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4102, 364, 702, 700, 1020, 0, 6205, 11100|  |
| Verb| 27| PRE |
| Noun| 52| SWE |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Condition| ConditionID 1 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in room with player |
| Action| ActionID 41 | Print message 'Sweep pops out, thanks me, hands me a piece of paper then vanishes\!' |
| Action| ActionID 55 ArgID 35| Item 'Stuck Chimney Sweep(index:35)' is removed from the game (put in room 0) |
| Action| ActionID 74 ArgID 51| take item 'Paper(index:51)', no check done to see if can carry |
### Action 90 - Input: REA PAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5301, 1023, 0, 0, 0, 0, 16200, 0|  |
| Verb| 35| REA |
| Noun| 51| PAP |
| Condition| ConditionID 2 ArgID 51| item 'Paper(index:51)' carried or in room with player |
| Action| ActionID 108 | Print message 'says: `SAY ZAP   to restore someone changed to stone\!`' |
### Action 91 - Input: LOO DOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6355, 883, 0, 0, 0, 0, 7050, 0|  |
| Verb| 42| LOO |
| Noun| 55| DOL |
| Condition| ConditionID 2 ArgID 44| item 'Doll(index:44)' carried or in room with player |
| Action| ActionID 47 | Print message 'Doll looks like Count Cristo\. There're pins in it\!' |
### Action 92 - Input: LOO COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6308, 542, 0, 0, 0, 0, 3601, 10975|  |
| Verb| 42| LOO |
| Noun| 8| COF |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Action| ActionID 24 | Print message 'A sign here says:' |
| Action| ActionID 1 | Print message 'Count Cristo's been CURSED\! There's one way for him to flee\! Find it, and he'll go FREE\!' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 25 | Print message 'There's a man here' |
### Action 93 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 654, 0, 0, 0, 0, 6450, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 32| item 'Rabbit's foot(index:32)' not in game |
| Action| ActionID 43 | Print message 'He's wearing a rabbit's foot' |
### Action 94 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 514, 0, 0, 0, 0, 3900, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 25| item 'Sapphire ring(index:25)' not in game |
| Action| ActionID 26 | Print message 'Wearing a sapphire ring' |
### Action 95 - Input: YEL CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9664, 24, 183, 283, 128, 883, 10982, 13229|  |
| Verb| 64| YEL |
| Noun| 64| CHA |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Condition| ConditionID 2 ArgID 9| item 'Brightly glowing idol(index:9)' carried or in room with player |
| Condition| ConditionID 2 ArgID 14| item 'Four leaf clover(index:14)' carried or in room with player |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Condition| ConditionID 2 ArgID 44| item 'Doll(index:44)' carried or in room with player |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 29 | Print message 'Pins fall out of doll' |
### Action 96 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1300, 0, 0, 0, 0, 8026, 5163|  |
| Probability| 0%|  |
| Action| ActionID 53 ArgID 65| drops item 'Smiling Count Cristo(index:65)' into current room |
| Action| ActionID 76 | look |
| Action| ActionID 34 | Print message 'HURRAH\! Look who is in the room\!' |
| Action| ActionID 63 | game over |
### Action 97 - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1575, 843, 840, 0, 0, 0, 3052, 0|  |
| Verb| 10| GET |
| Noun| 75| NAI |
| Condition| ConditionID 2 ArgID 42| item 'Nails(index:42)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 52 ArgID 42| get item 'Nails(index:42)', check if can carry |
### Action 98 - Input: GO POT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 216, 1122, 0, 0, 0, 0, 3000, 0|  |
| Verb| 1| GO |
| Noun| 66| POT |
| Condition| ConditionID 1 ArgID 56| item 'Open jail cell(index:56)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
### Action 99 - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6342, 763, 0, 0, 0, 0, 2550, 0|  |
| Verb| 42| LOO |
| Noun| 42| CHE |
| Condition| ConditionID 2 ArgID 38| item 'Labeled chemicals(index:38)' carried or in room with player |
| Action| ActionID 17 | Print message 'They appear to be mixable\.' |
### Action 100 - Input: LOO POT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6366, 323, 0, 0, 0, 0, 18150, 0|  |
| Verb| 42| LOO |
| Noun| 66| POT |
| Condition| ConditionID 2 ArgID 16| item 'Cast iron pot(index:16)' carried or in room with player |
| Action| ActionID 121 | Print message 'There's witch's brew there' |
### Action 101 - Input: GET FOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1547, 654, 542, 640, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 47| FOO |
| Condition| ConditionID 13 ArgID 32| item 'Rabbit's foot(index:32)' not in game |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Action| ActionID 52 ArgID 32| get item 'Rabbit's foot(index:32)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 102 - Input: GET FOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1547, 643, 640, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 47| FOO |
| Condition| ConditionID 2 ArgID 32| item 'Rabbit's foot(index:32)' carried or in room with player |
| Action| ActionID 52 ArgID 32| get item 'Rabbit's foot(index:32)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 103 - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 165, 202, 440, 0, 0, 0, 8120, 11400|  |
| Verb| 1| GO |
| Noun| 15| WIN |
| Condition| ConditionID 1 ArgID 10| item 'Open Window(index:10)' in room with player |
| Action| ActionID 54 ArgID 22| move room 22 |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 76 | look |
### Action 104 - Input: DUS IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3759, 863, 180, 860, 0, 0, 6372, 11400|  |
| Verb| 25| DUS |
| Noun| 9| IDO |
| Condition| ConditionID 2 ArgID 43| item 'Dusty Idol(index:43)' carried or in room with player |
| Action| ActionID 42 | Print message 'As I dust of the Idol it begins to glow\!' |
| Action| ActionID 72 ArgID 9, 43| swap item locations 'Brightly glowing idol(index:9)' and 'Dusty Idol(index:43)' |
| Action| ActionID 76 | look |
### Action 105 - Input: MOV KET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4361, 122, 120, 122, 0, 0, 8850, 0|  |
| Verb| 29| MOV |
| Noun| 11| KET |
| Condition| ConditionID 1 ArgID 6| item 'Dark hole(index:6)' in room with player |
| Condition| ConditionID 1 ArgID 6| item 'Dark hole(index:6)' in room with player |
| Action| ActionID 59 ArgID 6| Item 'Dark hole(index:6)' is removed from the game (put in room 0) |
### Action 106 - Input: LOO KET
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6311, 102, 64, 134, 0, 0, 3051, 7500|  |
| Verb| 42| LOO |
| Noun| 11| KET |
| Condition| ConditionID 1 ArgID 5| item 'Big kettle(index:5)' in room with player |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Condition| ConditionID 13 ArgID 6| item 'Dark hole(index:6)' not in game |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 51 | Print message 'I see a hole under it\!' |
| Action| ActionID 50 | Print message 'There's some soup here\.' |
### Action 107 - Input: CLO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5867, 0, 0, 0, 0, 0, 16650, 0|  |
| Verb| 39| CLO |
| Noun| 17| DOO |
| Action| ActionID 111 | Print message 'won't budge\!' |
### Action 108 - Input: DRI SOU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7202, 102, 900, 0, 0, 0, 3055, 0|  |
| Verb| 48| DRI |
| Noun| 2| SOU |
| Condition| ConditionID 1 ArgID 5| item 'Big kettle(index:5)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 55 ArgID 45| Item 'Wooden boards(index:45)' is removed from the game (put in room 0) |
### Action 109 - Input: WAV STI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3661, 883, 0, 0, 0, 0, 10970, 988|  |
| Verb| 24| WAV |
| Noun| 61| STI |
| Condition| ConditionID 2 ArgID 44| item 'Doll(index:44)' carried or in room with player |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
| Action| ActionID 88 | wait 2 seconds |
### Action 110 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 183, 24, 68, 120, 0, 13232, 17458|  |
| Probability| 0%|  |
| Condition| ConditionID 2 ArgID 9| item 'Brightly glowing idol(index:9)' carried or in room with player |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 32 | Print message 'There's a CLAP OF THUNDER\!' |
| Action| ActionID 116 | Print message 'Double bubble toil & trouble the encAntAtions Are About to peAk\!' |
| Action| ActionID 58 ArgID 6| set 6 flag |
### Action 111 - Input: SAW GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7520, 962, 981, 960, 0, 0, 15470, 11005|  |
| Verb| 50| SAW |
| Noun| 20| GRA |
| Condition| ConditionID 1 ArgID 48| item 'GrAting(index:48)' in room with player |
| Condition| ConditionID 0 ArgID 49| item 'Rusting SAW(index:49)' carried |
| Action| ActionID 103 | Print message 'It's hArd work but it seems to be coming loose' |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 55 ArgID 48| Item 'GrAting(index:48)' is removed from the game (put in room 0) |
### Action 112 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1000, 1180, 0, 0, 0, 8055, 11100|  |
| Probability| 0%|  |
| Action| ActionID 53 ArgID 50| drops item 'Button in the wall(index:50)' into current room |
| Action| ActionID 105 | Print message 'I've got it\!' |
| Action| ActionID 74 ArgID 59| take item 'Broken grating(index:59)', no check done to see if can carry |
### Action 113 - Input: PRE BUT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4109, 1002, 360, 0, 0, 0, 15954, 11400|  |
| Verb| 27| PRE |
| Noun| 59| BUT |
| Condition| ConditionID 1 ArgID 50| item 'Button in the wall(index:50)' in room with player |
| Action| ActionID 106 | Print message 'Heavy duty exhaust fan comes on & sucks me up\!' |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 76 | look |
### Action 114 - Input: QUI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7050, 0, 0, 0, 0, 0, 9450, 0|  |
| Verb| 47| QUI |
| Noun| 0| ANY |
| Action| ActionID 63 | game over |
### Action 115 - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 227, 622, 460, 0, 0, 0, 3054, 11400|  |
| Verb| 1| GO |
| Noun| 77| CRA |
| Condition| ConditionID 1 ArgID 31| item 'Wide crack in the wall(index:31)' in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 54 ArgID 23| move room 23 |
| Action| ActionID 76 | look |
### Action 116 - Input: LOO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6343, 1063, 0, 0, 0, 0, 16350, 0|  |
| Verb| 42| LOO |
| Noun| 43| STA |
| Condition| ConditionID 2 ArgID 53| item 'Ju\-Ju man statue(index:53)' carried or in room with player |
| Action| ActionID 109 | Print message 'Statue is made of stone' |
### Action 117 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 583, 0, 0, 0, 0, 4950, 0|  |
| Verb| 56| LIS |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 29| item 'Ju\-Ju man(index:29)' carried or in room with player |
| Action| ActionID 33 | Print message 'Ju\-Ju man says:`My bag is now yours\! Its magic will help you \-CRACK\- the curse\!`\.' |
### Action 118 - Input: GET HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1557, 943, 940, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 57| HAM |
| Condition| ConditionID 2 ArgID 47| item 'Antique hammer(index:47)' carried or in room with player |
| Action| ActionID 52 ArgID 47| get item 'Antique hammer(index:47)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 119 - Input: GET HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1557, 682, 109, 940, 100, 0, 7820, 8700|  |
| Verb| 10| GET |
| Noun| 57| HAM |
| Condition| ConditionID 1 ArgID 34| item 'Open SAfe(index:34)' in room with player |
| Condition| ConditionID 8 ArgID 5| bitflag 5 is false |
| Action| ActionID 52 ArgID 47| get item 'Antique hammer(index:47)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 58 ArgID 5| set 5 flag |
### Action 120 - Input: REA PAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5339, 1283, 0, 0, 0, 0, 18600, 0|  |
| Verb| 35| REA |
| Noun| 89| PAG |
| Condition| ConditionID 2 ArgID 64| item 'Page torn from a book(index:64)' carried or in room with player |
| Action| ActionID 124 | Print message '\.\.\.wave the stick and hold the lamp and don't forget to yell `CHANT`\! Oh yes, to help it succeed, a doll you'll need\.\.\.' |
### Action 121 - Input: WAV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 0, 0, 0, 0, 0, 3006, 0|  |
| Verb| 24| WAV |
| Noun| 0| ANY |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 122 - Input: SHR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8100, 0, 0, 0, 0, 0, 18900, 0|  |
| Verb| 54| SHR |
| Noun| 0| ANY |
| Action| ActionID 126 | Print message 'how?' |
### Action 123 - Input: REA WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5275, 43, 92, 0, 0, 0, 754, 0|  |
| Verb| 35| REA |
| Noun| 25| WRI |
| Condition| ConditionID 2 ArgID 2| item 'Plaque(index:2)' carried or in room with player |
| Condition| ConditionID 11 ArgID 4| item 'Broken glass(index:4)' not carried or in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 4 | Print message 'Prints too small for the unaided eye\.' |
### Action 124 - Input: OPE BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5744, 593, 523, 0, 0, 0, 3000, 0|  |
| Verb| 38| OPE |
| Noun| 44| BAG |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
### Action 125 - Input: LOO CEL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6367, 224, 0, 0, 0, 0, 1500, 0|  |
| Verb| 42| LOO |
| Noun| 67| CEL |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 10 | Print message 'I see nothing very special\.' |
### Action 126 - Input: MOV ARM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4380, 1143, 0, 0, 0, 0, 3000, 0|  |
| Verb| 29| MOV |
| Noun| 30| ARM |
| Condition| ConditionID 2 ArgID 57| item 'Knight's Suit of Armor(index:57)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
### Action 127 - Input: GET BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1544, 522, 0, 0, 0, 0, 19050, 0|  |
| Verb| 10| GET |
| Noun| 44| BAG |
| Condition| ConditionID 1 ArgID 26| item 'Ju\-Ju bag(index:26)' in room with player |
| Action| ActionID 127 | Print message 'It appears stuck to the floor\!' |
### Action 128 - Input: REA WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5275, 43, 83, 0, 0, 0, 761, 0|  |
| Verb| 35| REA |
| Noun| 25| WRI |
| Condition| ConditionID 2 ArgID 2| item 'Plaque(index:2)' carried or in room with player |
| Condition| ConditionID 2 ArgID 4| item 'Broken glass(index:4)' carried or in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 11 | Print message 'Phosphorescent letters are very hard to read in bright light\!' |
### Action 129 - Input: GO LED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 220, 184, 22, 0, 0, 0, 7350, 0|  |
| Verb| 1| GO |
| Noun| 70| LED |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 1 ArgID 1| item 'Ledge(index:1)' in room with player |
| Action| ActionID 49 | Print message 'Bird says: `ask for ADVENTURE 5, \-THE COUNT\- at your favorite computer dealer\. It will be LOVE AT FIRST BYTE\!` ' |
### Action 130 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 304, 713, 0, 0, 0, 15732, 0|  |
| Verb| 56| LIS |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 12 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in game |
| Action| ActionID 104 | Print message 'I hear strange sounds, as if someone were moaning\.' |
| Action| ActionID 132 | Print message 'Its very faint\.' |
### Action 131 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 713, 284, 0, 0, 0, 15733, 0|  |
| Verb| 56| LIS |
| Noun| 0| ANY |
| Condition| ConditionID 12 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in game |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Action| ActionID 104 | Print message 'I hear strange sounds, as if someone were moaning\.' |
| Action| ActionID 133 | Print message 'Its much louder up here\.' |
### Action 132 - Input: GO COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 158, 542, 0, 0, 0, 0, 19200, 0|  |
| Verb| 1| GO |
| Noun| 8| COF |
| Condition| ConditionID 1 ArgID 27| item 'Open Coffin(index:27)' in room with player |
| Action| ActionID 128 | Print message 'There's no room in there for me\!' |
### Action 133 - Input: GET SOU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1502, 102, 0, 0, 0, 0, 19500, 0|  |
| Verb| 10| GET |
| Noun| 2| SOU |
| Condition| ConditionID 1 ArgID 5| item 'Big kettle(index:5)' in room with player |
| Action| ActionID 130 | Print message 'I've no container\.' |
### Action 134 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 162, 1242, 120, 460, 0, 0, 8176, 5759|  |
| Verb| 1| GO |
| Noun| 12| HOL |
| Condition| ConditionID 1 ArgID 62| item 'Hole in the wall(index:62)' in room with player |
| Action| ActionID 54 ArgID 6| move room 6 |
| Action| ActionID 76 | look |
| Action| ActionID 38 | Print message 'You startled medium & she vanished' |
| Action| ActionID 59 ArgID 23| Item 'Spirit Medium(index:23)' is removed from the game (put in room 0) |
### Action 135 - Input: LOO RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6332, 503, 0, 0, 0, 0, 2700, 0|  |
| Verb| 42| LOO |
| Noun| 32| RIN |
| Condition| ConditionID 2 ArgID 25| item 'Sapphire ring(index:25)' carried or in room with player |
| Action| ActionID 18 | Print message 'There's something written there' |
### Action 136 - Input: CUT IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10359, 863, 3, 0, 0, 0, 19481, 0|  |
| Verb| 69| CUT |
| Noun| 9| IDO |
| Condition| ConditionID 2 ArgID 43| item 'Dusty Idol(index:43)' carried or in room with player |
| Condition| ConditionID 2 ArgID 0| item 'Bloody Knife(index:0)' carried or in room with player |
| Action| ActionID 129 | Print message 'My idol acted strange' |
| Action| ActionID 131 | Print message 'Some dust fell off it and it glowed briefly\.' |
### Action 137 - Input: CUT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10350, 3, 0, 0, 0, 0, 3006, 22350|  |
| Verb| 69| CUT |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 0| item 'Bloody Knife(index:0)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
| Action| ActionID 149 | Print message 'Knife made no impression on it\!' |
### Action 138 - Input: LOO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6344, 1053, 1094, 593, 523, 0, 20250, 0|  |
| Verb| 42| LOO |
| Noun| 44| BAG |
| Condition| ConditionID 12 ArgID 52| item 'Voodoo book(index:52)' in game |
| Condition| ConditionID 13 ArgID 54| item 'Stick(index:54)' not in game |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Action| ActionID 135 | Print message 'There's a stick there\.' |
### Action 139 - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1563, 523, 593, 1040, 1054, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 63| BOO |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Condition| ConditionID 13 ArgID 52| item 'Voodoo book(index:52)' not in game |
| Action| ActionID 52 ArgID 52| get item 'Voodoo book(index:52)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 140 - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1563, 1043, 1040, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 63| BOO |
| Condition| ConditionID 2 ArgID 52| item 'Voodoo book(index:52)' carried or in room with player |
| Action| ActionID 52 ArgID 52| get item 'Voodoo book(index:52)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 141 - Input: GET STI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1561, 523, 1094, 1080, 593, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 61| STI |
| Condition| ConditionID 2 ArgID 26| item 'Ju\-Ju bag(index:26)' carried or in room with player |
| Condition| ConditionID 13 ArgID 54| item 'Stick(index:54)' not in game |
| Condition| ConditionID 12 ArgID 29| item 'Ju\-Ju man(index:29)' in game |
| Action| ActionID 52 ArgID 54| get item 'Stick(index:54)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 142 - Input: GET STI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1561, 1083, 1080, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 61| STI |
| Condition| ConditionID 2 ArgID 54| item 'Stick(index:54)' carried or in room with player |
| Action| ActionID 52 ArgID 54| get item 'Stick(index:54)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 143 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 167, 822, 380, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 17| DOO |
| Condition| ConditionID 1 ArgID 41| item 'Wide open door(index:41)' in room with player |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 76 | look |
### Action 144 - Input: SHA SWO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9013, 4, 0, 0, 0, 0, 0, 0|  |
| Verb| 60| SHA |
| Noun| 13| SWO |
| Condition| ConditionID 3 ArgID 0| player in room 0 |
### Action 145 - Input: LOO IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6309, 863, 0, 0, 0, 0, 20410, 0|  |
| Verb| 42| LOO |
| Noun| 9| IDO |
| Condition| ConditionID 2 ArgID 43| item 'Dusty Idol(index:43)' carried or in room with player |
| Action| ActionID 136 | Print message 'Boy it looks dusty\.' |
| Action| ActionID 10 | Print message 'I see nothing very special\.' |
### Action 146 - Input: LOO IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6309, 183, 0, 0, 0, 0, 20550, 0|  |
| Verb| 42| LOO |
| Noun| 9| IDO |
| Condition| ConditionID 2 ArgID 9| item 'Brightly glowing idol(index:9)' carried or in room with player |
| Action| ActionID 137 | Print message 'Its glowing\.' |
### Action 147 - Input: DIG GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3320, 783, 0, 0, 0, 0, 2988, 0|  |
| Verb| 22| DIG |
| Noun| 20| GRA |
| Condition| ConditionID 2 ArgID 39| item 'Pocket Shovel(index:39)' carried or in room with player |
| Action| ActionID 19 | Print message 'A sepulchral voice says:' |
| Action| ActionID 138 | Print message 'Strange hobby you have' |
### Action 148 - Input: SAW ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7500, 981, 1162, 220, 0, 0, 18504, 9600|  |
| Verb| 50| SAW |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 49| item 'Rusting SAW(index:49)' carried |
| Condition| ConditionID 1 ArgID 58| item 'Closed cell door(index:58)' in room with player |
| Action| ActionID 123 | Print message 'You've been sprung' |
| Action| ActionID 54 ArgID 11| move room 11 |
| Action| ActionID 64 | look |
### Action 149 - Input: LIS CRY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8481, 184, 0, 0, 0, 0, 7350, 0|  |
| Verb| 56| LIS |
| Noun| 81| CRY |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Action| ActionID 49 | Print message 'Bird says: `ask for ADVENTURE 5, \-THE COUNT\- at your favorite computer dealer\. It will be LOVE AT FIRST BYTE\!` ' |
### Action 150 - Input: OPE WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5715, 4, 0, 0, 0, 0, 0, 0|  |
| Verb| 38| OPE |
| Noun| 15| WIN |
| Condition| ConditionID 3 ArgID 0| player in room 0 |
### Action 151 - Input: SLI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9300, 562, 160, 0, 0, 0, 8176, 0|  |
| Verb| 62| SLI |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 28| item 'Slick chute leading downward(index:28)' in room with player |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 152 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 702, 0, 0, 0, 0, 6750, 0|  |
| Verb| 56| LIS |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in room with player |
| Action| ActionID 45 | Print message 'HELP ME, I'm stuck\!' |
### Action 153 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 204, 0, 0, 0, 0, 20850, 0|  |
| Verb| 15| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Action| ActionID 139 | Print message 'Check out the fireplace\.' |
### Action 154 - Input: DAN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9450, 0, 0, 0, 0, 0, 3006, 0|  |
| Verb| 63| DAN |
| Noun| 0| ANY |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 155 - Input: YEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9600, 0, 0, 0, 0, 0, 3085, 900|  |
| Verb| 64| YEL |
| Noun| 0| ANY |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 156 - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1575, 922, 941, 920, 900, 840, 15372, 11100|  |
| Verb| 10| GET |
| Noun| 75| NAI |
| Condition| ConditionID 1 ArgID 46| item 'Wood boards nailed to chimney wall(index:46)' in room with player |
| Condition| ConditionID 0 ArgID 47| item 'Antique hammer(index:47)' carried |
| Action| ActionID 102 | Print message 'Nails were rusted but I got them out\.' |
| Action| ActionID 72 ArgID 46, 45| swap item locations 'Wood boards nailed to chimney wall(index:46)' and 'Wooden boards(index:45)' |
| Action| ActionID 74 ArgID 42| take item 'Nails(index:42)', no check done to see if can carry |
### Action 157 - Input: ON FLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3524, 641, 640, 0, 0, 0, 7970, 0|  |
| Verb| 23| ON |
| Noun| 74| FLO |
| Condition| ConditionID 0 ArgID 32| item 'Rabbit's foot(index:32)' carried |
| Action| ActionID 53 ArgID 32| drops item 'Rabbit's foot(index:32)' into current room |
| Action| ActionID 20 | Print message 'OK' |
### Action 158 - Input: GET BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1556, 903, 900, 169, 960, 160, 7853, 8700|  |
| Verb| 10| GET |
| Noun| 56| BOA |
| Condition| ConditionID 2 ArgID 45| item 'Wooden boards(index:45)' carried or in room with player |
| Condition| ConditionID 8 ArgID 8| bitflag 8 is false |
| Action| ActionID 52 ArgID 45| get item 'Wooden boards(index:45)', check if can carry |
| Action| ActionID 53 ArgID 48| drops item 'GrAting(index:48)' into current room |
| Action| ActionID 58 ArgID 8| set 8 flag |
### Action 159 - Input: GET BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1556, 903, 900, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 56| BOA |
| Condition| ConditionID 2 ArgID 45| item 'Wooden boards(index:45)' carried or in room with player |
| Action| ActionID 52 ArgID 45| get item 'Wooden boards(index:45)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 160 - Input: GET BRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1529, 0, 0, 0, 0, 0, 19500, 0|  |
| Verb| 10| GET |
| Noun| 29| BRE |
| Action| ActionID 130 | Print message 'I've no container\.' |
### Action 161 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 962, 0, 0, 0, 0, 21450, 0|  |
| Verb| 15| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 48| item 'GrAting(index:48)' in room with player |
| Action| ActionID 143 | Print message 'Saw grating\!' |
### Action 162 - Input: MIX CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7692, 763, 800, 760, 0, 0, 10820, 0|  |
| Verb| 51| MIX |
| Noun| 42| CHE |
| Condition| ConditionID 2 ArgID 38| item 'Labeled chemicals(index:38)' carried or in room with player |
| Action| ActionID 72 ArgID 40, 38| swap item locations 'Mixed Chemicals(index:40)' and 'Labeled chemicals(index:38)' |
| Action| ActionID 20 | Print message 'OK' |
### Action 163 - Input: HEL SWE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2302, 702, 0, 0, 0, 0, 18900, 0|  |
| Verb| 15| HEL |
| Noun| 52| SWE |
| Condition| ConditionID 1 ArgID 35| item 'Stuck Chimney Sweep(index:35)' in room with player |
| Action| ActionID 126 | Print message 'how?' |
### Action 164 - Input: RUB IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10809, 863, 0, 0, 0, 0, 19481, 0|  |
| Verb| 72| RUB |
| Noun| 9| IDO |
| Condition| ConditionID 2 ArgID 43| item 'Dusty Idol(index:43)' carried or in room with player |
| Action| ActionID 129 | Print message 'My idol acted strange' |
| Action| ActionID 131 | Print message 'Some dust fell off it and it glowed briefly\.' |
### Action 165 - Input: LOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 0, 0, 0, 0, 0, 11410, 0|  |
| Verb| 42| LOO |
| Noun| 0| ANY |
| Action| ActionID 76 | look |
| Action| ActionID 10 | Print message 'I see nothing very special\.' |
### Action 166 - Input: CUT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10350, 6, 0, 0, 0, 0, 894, 0|  |
| Verb| 69| CUT |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 0| item 'Bloody Knife(index:0)' not carried |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 144 | Print message 'I haven't got a knife\!' |
### Action 167 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8400, 0, 0, 0, 0, 0, 16500, 0|  |
| Verb| 56| LIS |
| Noun| 0| ANY |
| Action| ActionID 110 | Print message 'I hear nothing\.' |
### Action 168 - Input: GET RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 502, 500, 0, 0, 0, 7820, 0|  |
| Verb| 10| GET |
| Noun| 32| RIN |
| Condition| ConditionID 1 ArgID 25| item 'Sapphire ring(index:25)' in room with player |
| Action| ActionID 52 ArgID 25| get item 'Sapphire ring(index:25)', check if can carry |
| Action| ActionID 20 | Print message 'OK' |
### Action 169 - Input: SMO POT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11016, 0, 0, 0, 0, 0, 17250, 0|  |
| Verb| 73| SMO |
| Noun| 66| POT |
| Action| ActionID 115 | Print message 'That's illegal\!' |
### Action 170 - Input: BRE TUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4833, 723, 146, 500, 0, 0, 8164, 2173|  |
| Verb| 32| BRE |
| Noun| 33| TUB |
| Condition| ConditionID 2 ArgID 36| item 'Chem tubes(index:36)' carried or in room with player |
| Condition| ConditionID 5 ArgID 7| item 'Shield(index:7)' not carried |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 64 | look |
| Action| ActionID 14 | Print message 'One of the test tubes EXPLODED\!' |
| Action| ActionID 73 | continue with next action |
### Action 171 - Input: SAW ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7500, 981, 0, 0, 0, 0, 3006, 0|  |
| Verb| 50| SAW |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 49| item 'Rusting SAW(index:49)' carried |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 172 - Input: REA LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5337, 1203, 0, 0, 0, 0, 3009, 0|  |
| Verb| 35| REA |
| Noun| 87| LEA |
| Condition| ConditionID 2 ArgID 60| item 'Advertising leaflet(index:60)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 9 | Print message 'For a reading just `SUMMON MEDIUM MAEGEN` today\!\!' |
### Action 173 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3300, 783, 0, 0, 0, 0, 3006, 0|  |
| Verb| 22| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 39| item 'Pocket Shovel(index:39)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 174 - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 227, 1222, 0, 0, 0, 0, 787, 22050|  |
| Verb| 1| GO |
| Noun| 77| CRA |
| Condition| ConditionID 1 ArgID 61| item 'Crack in the wall(index:61)' in room with player |
| Action| ActionID 5 | Print message 'I can't do that' |
| Action| ActionID 37 | Print message 'I'm too big' |
| Action| ActionID 147 | Print message 'It will take some strong magic to get me through that\!' |
### Action 175 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2250, 0, 0, 0, 0, 0, 900, 0|  |
| Verb| 15| HEL |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 176 - Input: OPE SAF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5728, 742, 0, 0, 0, 0, 3150, 0|  |
| Verb| 38| OPE |
| Noun| 28| SAF |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 21 | Print message 'Safe's combination lock is numbered from 33 to 38\.' |
### Action 177 - Input: BRE STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4843, 1063, 1060, 1260, 0, 0, 3072, 0|  |
| Verb| 32| BRE |
| Noun| 43| STA |
| Condition| ConditionID 2 ArgID 53| item 'Ju\-Ju man statue(index:53)' carried or in room with player |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 72 ArgID 53, 63| swap item locations 'Ju-Ju man statue(index:53)' and 'Pieces of rock(index:63)' |
### Action 178 - Input: TUR 34
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6083, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 83| 34 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 179 - Input: TUR 35
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6084, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 84| 35 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 180 - Input: TUR 36
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6085, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 85| 36 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 181 - Input: TUR 37
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6086, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 86| 37 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 182 - Input: REA RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5282, 503, 0, 0, 0, 0, 21750, 0|  |
| Verb| 35| REA |
| Noun| 32| RIN |
| Condition| ConditionID 2 ArgID 25| item 'Sapphire ring(index:25)' carried or in room with player |
| Action| ActionID 145 | Print message 'Inscription on ring says: `WAVE ME\!`' |
### Action 183 - Input: OPE WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5715, 382, 0, 0, 0, 0, 16650, 0|  |
| Verb| 38| OPE |
| Noun| 15| WIN |
| Condition| ConditionID 1 ArgID 19| item 'Closed Window(index:19)' in room with player |
| Action| ActionID 111 | Print message 'won't budge\!' |
### Action 184 - Input: RUB RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10832, 503, 0, 0, 0, 0, 2700, 0|  |
| Verb| 72| RUB |
| Noun| 32| RIN |
| Condition| ConditionID 2 ArgID 25| item 'Sapphire ring(index:25)' carried or in room with player |
| Action| ActionID 18 | Print message 'There's something written there' |
### Action 185 - Input: RUB ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10800, 0, 0, 0, 0, 0, 3006, 0|  |
| Verb| 72| RUB |
| Noun| 0| ANY |
| Action| ActionID 20 | Print message 'OK' |
| Action| ActionID 6 | Print message 'Nothing happened' |
### Action 186 - Input: TUR LOC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6069, 742, 0, 0, 0, 0, 22200, 0|  |
| Verb| 40| TUR |
| Noun| 69| LOC |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 148 | Print message 'Use a number\!' |
### Action 187 - Input: TUR 33
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6039, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 39| 33 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 188 - Input: TUR 38
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6037, 742, 20, 0, 0, 0, 9020, 0|  |
| Verb| 40| TUR |
| Noun| 37| 38 |
| Condition| ConditionID 1 ArgID 37| item 'Closed SAfe(index:37)' in room with player |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 20 | Print message 'OK' |
### Action 189 - Input: HUG DOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11305, 883, 0, 0, 0, 0, 3450, 0|  |
| Verb| 75| HUG |
| Noun| 55| DOL |
| Condition| ConditionID 2 ArgID 44| item 'Doll(index:44)' carried or in room with player |
| Action| ActionID 23 | Print message 'OUCH' |
### Action 191 - Take for item Bloody Knife - Input: GET KNI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 7| KNI |
| Condition| ConditionID 1 ArgID 0| item 'Bloody Knife(index:0)' in room with player |
| Action| ActionID 52 ArgID 0| get item 'Bloody Knife(index:0)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 192 - Drop for item Bloody Knife - Input: DRO KNI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 7| KNI |
| Condition| ConditionID 0 ArgID 0| item 'Bloody Knife(index:0)' carried |
| Action| ActionID 53 ArgID 0| drops item 'Bloody Knife(index:0)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 193 - Take for item Plaque - Input: GET WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 25| WRI |
| Condition| ConditionID 1 ArgID 2| item 'Plaque(index:2)' in room with player |
| Action| ActionID 52 ArgID 2| get item 'Plaque(index:2)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 194 - Drop for item Plaque - Input: DRO WRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 25| WRI |
| Condition| ConditionID 0 ArgID 2| item 'Plaque(index:2)' carried |
| Action| ActionID 53 ArgID 2| drops item 'Plaque(index:2)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 195 - Take for item Animal heads - Input: GET HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 40| HEA |
| Condition| ConditionID 1 ArgID 3| item 'Animal heads(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Animal heads(index:3)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 196 - Drop for item Animal heads - Input: DRO HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 40| HEA |
| Condition| ConditionID 0 ArgID 3| item 'Animal heads(index:3)' carried |
| Action| ActionID 53 ArgID 3| drops item 'Animal heads(index:3)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 197 - Take for item Broken glass - Input: GET GLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 31| GLA |
| Condition| ConditionID 1 ArgID 4| item 'Broken glass(index:4)' in room with player |
| Action| ActionID 52 ArgID 4| get item 'Broken glass(index:4)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 198 - Drop for item Broken glass - Input: DRO GLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 31| GLA |
| Condition| ConditionID 0 ArgID 4| item 'Broken glass(index:4)' carried |
| Action| ActionID 53 ArgID 4| drops item 'Broken glass(index:4)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 199 - Take for item Shield - Input: GET SHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 27| SHI |
| Condition| ConditionID 1 ArgID 7| item 'Shield(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Shield(index:7)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 200 - Drop for item Shield - Input: DRO SHI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 27| SHI |
| Condition| ConditionID 0 ArgID 7| item 'Shield(index:7)' carried |
| Action| ActionID 53 ArgID 7| drops item 'Shield(index:7)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 201 - Take for item Brightly glowing idol - Input: GET IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 9| IDO |
| Condition| ConditionID 1 ArgID 9| item 'Brightly glowing idol(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Brightly glowing idol(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 202 - Drop for item Brightly glowing idol - Input: DRO IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 9| IDO |
| Condition| ConditionID 0 ArgID 9| item 'Brightly glowing idol(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Brightly glowing idol(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 203 - Take for item Four leaf clover - Input: GET CLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 16| CLO |
| Condition| ConditionID 1 ArgID 14| item 'Four leaf clover(index:14)' in room with player |
| Action| ActionID 52 ArgID 14| get item 'Four leaf clover(index:14)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 204 - Drop for item Four leaf clover - Input: DRO CLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 16| CLO |
| Condition| ConditionID 0 ArgID 14| item 'Four leaf clover(index:14)' carried |
| Action| ActionID 53 ArgID 14| drops item 'Four leaf clover(index:14)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 205 - Take for item Cast iron pot - Input: GET POT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 66| POT |
| Condition| ConditionID 1 ArgID 16| item 'Cast iron pot(index:16)' in room with player |
| Action| ActionID 52 ArgID 16| get item 'Cast iron pot(index:16)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 206 - Drop for item Cast iron pot - Input: DRO POT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 66| POT |
| Condition| ConditionID 0 ArgID 16| item 'Cast iron pot(index:16)' carried |
| Action| ActionID 53 ArgID 16| drops item 'Cast iron pot(index:16)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 207 - Take for item Soot - Input: GET SOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 38| SOO |
| Condition| ConditionID 1 ArgID 21| item 'Soot(index:21)' in room with player |
| Action| ActionID 52 ArgID 21| get item 'Soot(index:21)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 208 - Drop for item Soot - Input: DRO SOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 38| SOO |
| Condition| ConditionID 0 ArgID 21| item 'Soot(index:21)' carried |
| Action| ActionID 53 ArgID 21| drops item 'Soot(index:21)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 209 - Take for item Sapphire ring - Input: GET RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 32| RIN |
| Condition| ConditionID 1 ArgID 25| item 'Sapphire ring(index:25)' in room with player |
| Action| ActionID 52 ArgID 25| get item 'Sapphire ring(index:25)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 210 - Drop for item Sapphire ring - Input: DRO RIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 32| RIN |
| Condition| ConditionID 0 ArgID 25| item 'Sapphire ring(index:25)' carried |
| Action| ActionID 53 ArgID 25| drops item 'Sapphire ring(index:25)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 211 - Take for item Ju-Ju bag - Input: GET BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| BAG |
| Condition| ConditionID 1 ArgID 26| item 'Ju\-Ju bag(index:26)' in room with player |
| Action| ActionID 52 ArgID 26| get item 'Ju-Ju bag(index:26)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 212 - Drop for item Ju-Ju bag - Input: DRO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| BAG |
| Condition| ConditionID 0 ArgID 26| item 'Ju\-Ju bag(index:26)' carried |
| Action| ActionID 53 ArgID 26| drops item 'Ju-Ju bag(index:26)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 213 - Take for item Rabbit's foot - Input: GET FOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 47| FOO |
| Condition| ConditionID 1 ArgID 32| item 'Rabbit's foot(index:32)' in room with player |
| Action| ActionID 52 ArgID 32| get item 'Rabbit's foot(index:32)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 214 - Drop for item Rabbit's foot - Input: DRO FOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 47| FOO |
| Condition| ConditionID 0 ArgID 32| item 'Rabbit's foot(index:32)' carried |
| Action| ActionID 53 ArgID 32| drops item 'Rabbit's foot(index:32)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 215 - Take for item Dull & broken sword - Input: GET SWO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 13| SWO |
| Condition| ConditionID 1 ArgID 33| item 'Dull & broken sword(index:33)' in room with player |
| Action| ActionID 52 ArgID 33| get item 'Dull & broken sword(index:33)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 216 - Drop for item Dull & broken sword - Input: DRO SWO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 13| SWO |
| Condition| ConditionID 0 ArgID 33| item 'Dull & broken sword(index:33)' carried |
| Action| ActionID 53 ArgID 33| drops item 'Dull & broken sword(index:33)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 217 - Take for item Chem tubes - Input: GET TUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 33| TUB |
| Condition| ConditionID 1 ArgID 36| item 'Chem tubes(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Chem tubes(index:36)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 218 - Drop for item Chem tubes - Input: DRO TUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 33| TUB |
| Condition| ConditionID 0 ArgID 36| item 'Chem tubes(index:36)' carried |
| Action| ActionID 53 ArgID 36| drops item 'Chem tubes(index:36)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 219 - Take for item Labeled chemicals - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 42| CHE |
| Condition| ConditionID 1 ArgID 38| item 'Labeled chemicals(index:38)' in room with player |
| Action| ActionID 52 ArgID 38| get item 'Labeled chemicals(index:38)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 220 - Drop for item Labeled chemicals - Input: DRO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 42| CHE |
| Condition| ConditionID 0 ArgID 38| item 'Labeled chemicals(index:38)' carried |
| Action| ActionID 53 ArgID 38| drops item 'Labeled chemicals(index:38)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 221 - Take for item Pocket Shovel - Input: GET SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 50| SHO |
| Condition| ConditionID 1 ArgID 39| item 'Pocket Shovel(index:39)' in room with player |
| Action| ActionID 52 ArgID 39| get item 'Pocket Shovel(index:39)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 222 - Drop for item Pocket Shovel - Input: DRO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 50| SHO |
| Condition| ConditionID 0 ArgID 39| item 'Pocket Shovel(index:39)' carried |
| Action| ActionID 53 ArgID 39| drops item 'Pocket Shovel(index:39)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 223 - Take for item Mixed Chemicals - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 42| CHE |
| Condition| ConditionID 1 ArgID 40| item 'Mixed Chemicals(index:40)' in room with player |
| Action| ActionID 52 ArgID 40| get item 'Mixed Chemicals(index:40)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 224 - Drop for item Mixed Chemicals - Input: DRO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 42| CHE |
| Condition| ConditionID 0 ArgID 40| item 'Mixed Chemicals(index:40)' carried |
| Action| ActionID 53 ArgID 40| drops item 'Mixed Chemicals(index:40)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 225 - Take for item Nails - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 75| NAI |
| Condition| ConditionID 1 ArgID 42| item 'Nails(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Nails(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 226 - Drop for item Nails - Input: DRO NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 75| NAI |
| Condition| ConditionID 0 ArgID 42| item 'Nails(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Nails(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 227 - Take for item Dusty Idol - Input: GET IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 9| IDO |
| Condition| ConditionID 1 ArgID 43| item 'Dusty Idol(index:43)' in room with player |
| Action| ActionID 52 ArgID 43| get item 'Dusty Idol(index:43)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 228 - Drop for item Dusty Idol - Input: DRO IDO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 9| IDO |
| Condition| ConditionID 0 ArgID 43| item 'Dusty Idol(index:43)' carried |
| Action| ActionID 53 ArgID 43| drops item 'Dusty Idol(index:43)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 229 - Take for item Doll - Input: GET DOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 55| DOL |
| Condition| ConditionID 1 ArgID 44| item 'Doll(index:44)' in room with player |
| Action| ActionID 52 ArgID 44| get item 'Doll(index:44)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 230 - Drop for item Doll - Input: DRO DOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 55| DOL |
| Condition| ConditionID 0 ArgID 44| item 'Doll(index:44)' carried |
| Action| ActionID 53 ArgID 44| drops item 'Doll(index:44)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 231 - Take for item Wooden boards - Input: GET BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 56| BOA |
| Condition| ConditionID 1 ArgID 45| item 'Wooden boards(index:45)' in room with player |
| Action| ActionID 52 ArgID 45| get item 'Wooden boards(index:45)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 232 - Drop for item Wooden boards - Input: DRO BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 56| BOA |
| Condition| ConditionID 0 ArgID 45| item 'Wooden boards(index:45)' carried |
| Action| ActionID 53 ArgID 45| drops item 'Wooden boards(index:45)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 233 - Take for item Antique hammer - Input: GET HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 57| HAM |
| Condition| ConditionID 1 ArgID 47| item 'Antique hammer(index:47)' in room with player |
| Action| ActionID 52 ArgID 47| get item 'Antique hammer(index:47)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 234 - Drop for item Antique hammer - Input: DRO HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 57| HAM |
| Condition| ConditionID 0 ArgID 47| item 'Antique hammer(index:47)' carried |
| Action| ActionID 53 ArgID 47| drops item 'Antique hammer(index:47)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 235 - Take for item Rusting SAW - Input: GET SAW
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 46| SAW |
| Condition| ConditionID 1 ArgID 49| item 'Rusting SAW(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item 'Rusting SAW(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 236 - Drop for item Rusting SAW - Input: DRO SAW
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 46| SAW |
| Condition| ConditionID 0 ArgID 49| item 'Rusting SAW(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item 'Rusting SAW(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 237 - Take for item Paper - Input: GET PAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 51| PAP |
| Condition| ConditionID 1 ArgID 51| item 'Paper(index:51)' in room with player |
| Action| ActionID 52 ArgID 51| get item 'Paper(index:51)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 238 - Drop for item Paper - Input: DRO PAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 51| PAP |
| Condition| ConditionID 0 ArgID 51| item 'Paper(index:51)' carried |
| Action| ActionID 53 ArgID 51| drops item 'Paper(index:51)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 239 - Take for item Voodoo book - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 63| BOO |
| Condition| ConditionID 1 ArgID 52| item 'Voodoo book(index:52)' in room with player |
| Action| ActionID 52 ArgID 52| get item 'Voodoo book(index:52)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 240 - Drop for item Voodoo book - Input: DRO BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 63| BOO |
| Condition| ConditionID 0 ArgID 52| item 'Voodoo book(index:52)' carried |
| Action| ActionID 53 ArgID 52| drops item 'Voodoo book(index:52)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 241 - Take for item Ju-Ju man statue - Input: GET STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 43| STA |
| Condition| ConditionID 1 ArgID 53| item 'Ju\-Ju man statue(index:53)' in room with player |
| Action| ActionID 52 ArgID 53| get item 'Ju-Ju man statue(index:53)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 242 - Drop for item Ju-Ju man statue - Input: DRO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 43| STA |
| Condition| ConditionID 0 ArgID 53| item 'Ju\-Ju man statue(index:53)' carried |
| Action| ActionID 53 ArgID 53| drops item 'Ju-Ju man statue(index:53)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 243 - Take for item Stick - Input: GET STI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 61| STI |
| Condition| ConditionID 1 ArgID 54| item 'Stick(index:54)' in room with player |
| Action| ActionID 52 ArgID 54| get item 'Stick(index:54)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 244 - Drop for item Stick - Input: DRO STI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 61| STI |
| Condition| ConditionID 0 ArgID 54| item 'Stick(index:54)' carried |
| Action| ActionID 53 ArgID 54| drops item 'Stick(index:54)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 245 - Take for item Broken grating - Input: GET GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 20| GRA |
| Condition| ConditionID 1 ArgID 59| item 'Broken grating(index:59)' in room with player |
| Action| ActionID 52 ArgID 59| get item 'Broken grating(index:59)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 246 - Drop for item Broken grating - Input: DRO GRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 20| GRA |
| Condition| ConditionID 0 ArgID 59| item 'Broken grating(index:59)' carried |
| Action| ActionID 53 ArgID 59| drops item 'Broken grating(index:59)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 247 - Take for item Advertising leaflet - Input: GET LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 87| LEA |
| Condition| ConditionID 1 ArgID 60| item 'Advertising leaflet(index:60)' in room with player |
| Action| ActionID 52 ArgID 60| get item 'Advertising leaflet(index:60)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 248 - Drop for item Advertising leaflet - Input: DRO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 87| LEA |
| Condition| ConditionID 0 ArgID 60| item 'Advertising leaflet(index:60)' carried |
| Action| ActionID 53 ArgID 60| drops item 'Advertising leaflet(index:60)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 249 - Take for item Pieces of rock - Input: GET ROC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 79| ROC |
| Condition| ConditionID 1 ArgID 63| item 'Pieces of rock(index:63)' in room with player |
| Action| ActionID 52 ArgID 63| get item 'Pieces of rock(index:63)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 250 - Drop for item Pieces of rock - Input: DRO ROC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 79| ROC |
| Condition| ConditionID 0 ArgID 63| item 'Pieces of rock(index:63)' carried |
| Action| ActionID 53 ArgID 63| drops item 'Pieces of rock(index:63)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 251 - Take for item Page torn from a book - Input: GET PAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 89| PAG |
| Condition| ConditionID 1 ArgID 64| item 'Page torn from a book(index:64)' in room with player |
| Action| ActionID 52 ArgID 64| get item 'Page torn from a book(index:64)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 252 - Drop for item Page torn from a book - Input: DRO PAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 89| PAG |
| Condition| ConditionID 0 ArgID 64| item 'Page torn from a book(index:64)' carried |
| Action| ActionID 53 ArgID 64| drops item 'Page torn from a book(index:64)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 253 - Manually added load game action - Input: LOA GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 92| LOA |
| Noun| 49| GAM |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUT| 0|  |
| GO| 1| ENT, WAL, CLI, RUN |
| \.| 6|  |
| | 7|  |
| | 8|  |
| | 9|  |
| GET| 10| TAK, PIC, REM, PUL |
| HEL| 15| RES |
| \.| 17|  |
| DRO| 18| PUT, LEA, THR |
| DIG| 22|  |
| ON| 23|  |
| WAV| 24|  |
| DUS| 25| CLE |
| PRE| 27| PUS |
| MOV| 29| SHO, KIC |
| BRE| 32| SMA |
| SAV| 34|  |
| REA| 35|  |
| \.| 36|  |
| | 37|  |
| OPE| 38|  |
| CLO| 39|  |
| TUR| 40| DIA |
| LOO| 42| EXA |
| INV| 44|  |
| CIR| 45|  |
| \.| 46|  |
| QUI| 47|  |
| DRI| 48| EAT |
| SAW| 50|  |
| MIX| 51|  |
| HAM| 52|  |
| \.| 53|  |
| SHR| 54|  |
| \.| 55|  |
| LIS| 56| HEA |
| STA| 58|  |
| | 59|  |
| SHA| 60|  |
| | 61|  |
| SLI| 62|  |
| DAN| 63|  |
| YEL| 64| SCR, SUM, SAY, CRY |
| CUT| 69| STA |
| | 71|  |
| RUB| 72|  |
| SMO| 73|  |
| \.| 74|  |
| HUG| 75|  |
| | 76|  |
| | 77|  |
| | 78|  |
| | 79|  |
| | 80|  |
| | 81|  |
| | 82|  |
| | 83|  |
| | 84|  |
| | 85|  |
| | 86|  |
| | 87|  |
| | 88|  |
| | 89|  |
| LOA| 92|  |
### Nouns
| Word| Index| Aliases |
| ----| -----| ------- |
| ANY| 0|  |
| NOR| 1|  |
| SOU| 2|  |
| EAS| 3|  |
| WES| 4|  |
| UP| 5|  |
| DOW| 6|  |
| KNI| 7|  |
| COF| 8|  |
| IDO| 9|  |
| INV| 10|  |
| KET| 11|  |
| HOL| 12|  |
| SWO| 13|  |
| PAT| 14|  |
| WIN| 15|  |
| CLO| 16|  |
| DOO| 17|  |
| CHU| 18|  |
| LAB| 19|  |
| GRA| 20|  |
| WAL| 21|  |
| BAL| 22|  |
| MED| 23|  |
| CHI| 24|  |
| WRI| 25| PLA |
| SHI| 27|  |
| SAF| 28|  |
| BRE| 29|  |
| ARM| 30|  |
| GLA| 31|  |
| RIN| 32|  |
| TUB| 33|  |
| FIR| 34|  |
| FLU| 35| CHI |
| 38| 37|  |
| SOO| 38|  |
| 33| 39|  |
| HEA| 40| ANI |
| CHE| 42|  |
| STA| 43|  |
| BAG| 44|  |
| PIN| 45|  |
| SAW| 46|  |
| FOO| 47| RAB |
| GAM| 49|  |
| SHO| 50|  |
| PAP| 51|  |
| SWE| 52|  |
| MAN| 53| CRI |
| DOL| 55|  |
| BOA| 56|  |
| HAM| 57|  |
| GRA| 58|  |
| BUT| 59|  |
| PUP| 60|  |
| STI| 61|  |
| STA| 62|  |
| BOO| 63|  |
| CHA| 64|  |
| ZAP| 65|  |
| POT| 66|  |
| CEL| 67|  |
| BAR| 68|  |
| LOC| 69|  |
| LED| 70|  |
| WOO| 71|  |
| VOI| 72|  |
| SIG| 73|  |
| FLO| 74|  |
| NAI| 75|  |
| MUM| 76|  |
| CRA| 77|  |
| SAP| 78|  |
| ROC| 79|  |
| ARO| 80|  |
| CRY| 81| RAV |
| 34| 83|  |
| 35| 84|  |
| 36| 85|  |
| 37| 86|  |
| LEA| 87|  |
| MOA| 88|  |
| PAG| 89|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| chapel| North: 9, South: 2, East: 4, West: 10 |
| 2| Dingy Looking Stairwell| North: 1, South: 24, East: 3, West: 11 |
| 3| room in the castle| North: 5, West: 2 |
| 4| Tunnel| West: 1 |
| 5| room in the castle| South: 3, East: 7 |
| 6| \*I'm in Medium Maegen's Mad Room| West: 8 |
| 7| room in the castle| East: 17, West: 5 |
| 8| room in the castle|  |
| 9| room in the castle| South: 1 |
| 10| Ballroom| East: 1 |
| 11| dungeon| South: 13, East: 2 |
| 12| \*I'm in the Armory| West: 13 |
| 13| torture chamber| North: 11, East: 12 |
| 14| Chimney| Down: 15 |
| 15| large fireplace| South: 10 |
| 16| room in the castle| Up: 3 |
| 17| Lab| West: 7 |
| 18| narrow part of the chimney| Down: 14 |
| 19| Graveyard| East: 13 |
| 20| parlor| Down: 2 |
| 21| Jail Cell|  |
| 22| \*I'm on a ledge| South: 9 |
| 23| hidden VOODOO room| South: 8 |
| 24| room in the castle| North: 2 |
| 25| lot of TROUBLE\!|  |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| Count Cristo's been CURSED\! There's one way for him to flee\! Find it, and he'll go FREE\! |
| 2| It belongs to the medium |
| 3| Spirit vibrations drive me from room\. |
| 4| Prints too small for the unaided eye\. |
| 5| I can't do that |
| 6| Nothing happened |
| 7| Windows open |
| 8| Window just slAmmed shut |
| 9| For a reading just `SUMMON MEDIUM MAEGEN` today\!\! |
| 10| I see nothing very special\. |
| 11| Phosphorescent letters are very hard to read in bright light\! |
| 12| Amongst the GRAVES is a four leaf clover\. |
| 13| Raven crys something outside |
| 14| One of the test tubes EXPLODED\! |
| 15| This glass can't be broken |
| 16| \. |
| 17| They appear to be mixable\. |
| 18| There's something written there |
| 19| A sepulchral voice says: |
| 20| OK |
| 21| Safe's combination lock is numbered from 33 to 38\. |
| 22| Ring glows briefly & door vanishes |
| 23| OUCH |
| 24| A sign here says: |
| 25| There's a man here |
| 26| Wearing a sapphire ring |
| 27| I slide back down |
| 28| A beam of light shines on grave |
| 29| Pins fall out of doll |
| 30| Plaque says: `safe \-\-\> 38 33` |
| 31| This grAve reserved for you\! |
| 32| There's a CLAP OF THUNDER\! |
| 33| Ju\-Ju man says:`My bag is now yours\! Its magic will help you \-CRACK\- the curse\!`\. |
| 34| HURRAH\! Look who is in the room\! |
| 35| I'm now 4 feet tall\! |
| 36| It's much to heavy to LIFT\! |
| 37| I'm too big |
| 38| You startled medium & she vanished |
| 39| On what? |
| 40| Maid chased me with broom for tracking soot through the Ball\- room\. I wonder where I am? |
| 41| Sweep pops out, thanks me, hands me a piece of paper then vanishes\! |
| 42| As I dust of the Idol it begins to glow\! |
| 43| He's wearing a rabbit's foot |
| 44| \. |
| 45| HELP ME, I'm stuck\! |
| 46| Luck wasn't with me\! |
| 47| Doll looks like Count Cristo\. There're pins in it\! |
| 48| \. |
| 49| Bird says: `ask for ADVENTURE 5, \-THE COUNT\- at your favorite computer dealer\. It will be LOVE AT FIRST BYTE\!`  |
| 50| There's some soup here\. |
| 51| I see a hole under it\! |
| 52| Nails were rusted but I got them out\. |
| 53| It's hArd work but it seems to be coming loose |
| 54| I hear strange sounds, as if someone were moaning\. |
| 55| I've got it\! |
| 56| Heavy duty exhaust fan comes on & sucks me up\! |
| 57| \. |
| 58| says: `SAY ZAP   to restore someone changed to stone\!` |
| 59| Statue is made of stone |
| 60| I hear nothing\. |
| 61| won't budge\! |
| 62| I'll need something to pry it off the wall\! |
| 63| It's a book on removing curses\. Says: `With knife in hand you take a stand\. Circle coffin and\.\.\.` The rest of the page is missing\!\!\! |
| 64| Its very dark, the only light is from the idol\. |
| 65| That's illegal\! |
| 66| Double bubble toil & trouble the encAntAtions Are About to peAk\! |
| 67| There's an antique hammer here |
| 68| There's a Clap of Thunder & then suddenly the stone statue begins to crack\. I may be in trouble now, there's someone in the room with me\! |
| 69| Looks almost like lemonade\. Yummy\! |
| 70| You've been turned into a broomstick & a witch rides off on you\! |
| 71| There's witch's brew there |
| 72| Cell door slams shut |
| 73| You've been sprung |
| 74| \.\.\.wave the stick and hold the lamp and don't forget to yell `CHANT`\! Oh yes, to help it succeed, a doll you'll need\.\.\. |
| 75| Welcome to ADVENTURE:4, `VOODOO CASTLE` by Alexis ADAMS\. Dedicated to all MOMS\! |
| 76| how? |
| 77| It appears stuck to the floor\! |
| 78| There's no room in there for me\! |
| 79| My idol acted strange |
| 80| I've no container\. |
| 81| Some dust fell off it and it glowed briefly\. |
| 82| Its very faint\. |
| 83| Its much louder up here\. |
| 84| There's a book there\. |
| 85| There's a stick there\. |
| 86| Boy it looks dusty\. |
| 87| Its glowing\. |
| 88| Strange hobby you have |
| 89| Check out the fireplace\. |
| 90| Its empty\. |
| 91| I hear someone mumbling\. |
| 92| \. |
| 93| Saw grating\! |
| 94| I haven't got a knife\! |
| 95| Inscription on ring says: `WAVE ME\!` |
| 96| Medium appears, says: `Keep a good luck charm on you & your friend\. I also see a \-moving\- bag helping you through a tight squeeze\!` |
| 97| It will take some strong magic to get me through that\! |
| 98| Use a number\! |
| 99| Knife made no impression on it\! |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Bloody Knife| KNI| 4 |
| 1| Ledge| | 0 |
| 2| Plaque| WRI| 8 |
| 3| Animal heads| HEA| 5 |
| 4| Broken glass| GLA| 2 |
| 5| Big kettle| | 3 |
| 6| Dark hole| | 0 |
| 7| Shield| SHI| 12 |
| 8| Stairs| | 2 |
| 9| Brightly glowing idol| IDO| 0 |
| 10| Open Window| | 9 |
| 11| Dark Chimney| | 0 |
| 12| Closed Flue| | 15 |
| 13| Open Flue| | 0 |
| 14| Four leaf clover| CLO| 0 |
| 15| GrAves| | 19 |
| 16| Cast iron pot| POT| 7 |
| 17| Closed Coffin| | 1 |
| 18| Crystal Ball| | 6 |
| 19| Closed Window| | 0 |
| 20| Large fireplace| | 10 |
| 21| Soot| SOO| 14 |
| 22| Tiny open door| | 13 |
| 23| Spirit Medium| | 0 |
| 24| Massive stone door with a SAPPHIRE set into it| | 4 |
| 25| Sapphire ring| RIN| 0 |
| 26| Ju\-Ju bag| BAG| 17 |
| 27| Open Coffin| | 0 |
| 28| Slick chute leading downward| | 0 |
| 29| Ju\-Ju man| | 0 |
| 30| Slippery chute leading up| | 8 |
| 31| Wide crack in the wall| | 0 |
| 32| Rabbit's foot| FOO| 16 |
| 33| Dull & broken sword| SWO| 12 |
| 34| Open SAfe| | 0 |
| 35| Stuck Chimney Sweep| | 18 |
| 36| Chem tubes| TUB| 17 |
| 37| Closed SAfe| | 0 |
| 38| Labeled chemicals| CHE| 17 |
| 39| Pocket Shovel| SHO| 11 |
| 40| Mixed Chemicals| CHE| 0 |
| 41| Wide open door| | 0 |
| 42| Nails| NAI| 0 |
| 43| Dusty Idol| IDO| 15 |
| 44| Doll| DOL| 22 |
| 45| Wooden boards| BOA| 0 |
| 46| Wood boards nailed to chimney wall| | 14 |
| 47| Antique hammer| HAM| 0 |
| 48| GrAting| | 0 |
| 49| Rusting SAW| SAW| 19 |
| 50| Button in the wall| | 0 |
| 51| Paper| PAP| 0 |
| 52| Voodoo book| BOO| 0 |
| 53| Ju\-Ju man statue| STA| 20 |
| 54| Stick| STI| 0 |
| 55| Open wall| | 0 |
| 56| Open jail cell| | 11 |
| 57| Knight's Suit of Armor| | 12 |
| 58| Closed cell door| | 21 |
| 59| Broken grating| GRA| 0 |
| 60| Advertising leaflet| LEA| 21 |
| 61| Crack in the wall| | 8 |
| 62| Hole in the wall| | 8 |
| 63| Pieces of rock| ROC| 0 |
| 64| Page torn from a book| PAG| 23 |
| 65| Smiling Count Cristo| | 0 |