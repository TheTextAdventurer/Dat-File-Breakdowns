# Ghost Town Datfile
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
| adventureNumber| 9 |
| Unknown| 4727 |
| numItems| 78 |
| numActions| 238 |
| numNounVerbs| 120 |
| numRooms| 39 |
| maxCarry| 7 |
| startRoom| 1 |
| totalTreasures| 13 |
| wordLength| 4 |
| lightDuration| 175 |
| numMessages| 98 |
| treasureRoom| 15 |
## Actions
### Action 0 - Probability: 3 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3, 193, 180, 520, 0, 0, 5472, 11400|  |
| Probability| 3%|  |
| Condition| ConditionID 12 ArgID 9| item 'Lit candle(index:9)' in game |
| Action| ActionID 36 | Print message 'Candle blew out\!' |
| Action| ActionID 72 ArgID 9, 26| swap item locations 'Lit candle(index:9)' and 'Unlit candle(index:26)' |
| Action| ActionID 76 | look |
### Action 1 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1402, 183, 1400, 0, 0, 8926, 1647|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 70| item 'Ghostly square dance(index:70)' in room with player |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Action| ActionID 59 ArgID 70| Item 'Ghostly square dance(index:70)' is removed from the game (put in room 0) |
| Action| ActionID 76 | look |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 147 | Print message 'scared them off\!' |
### Action 2 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 29, 0, 40, 240, 0, 11923, 12229|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 1| bitflag 1 is false |
| Action| ActionID 79 ArgID 0| set current counter value 0 |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
| Action| ActionID 79 ArgID 12| set current counter value 12 |
### Action 3 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 120, 0, 0, 0, 0, 12153, 600|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
| Action| ActionID 3 | Print message 'Welcome to Adventure 9 `GHOST TOWN`' |
| Action| ActionID 4 | Print message 'by Scott Adams dedicated: the Cherens' |
### Action 4 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 20, 500, 60, 3400, 0, 8779, 12229|  |
| Probability| 0%|  |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 79 ArgID 25| set current counter value 25 |
| Action| ActionID 81 ArgID 3| Select counter 3. Current counter is swapped with backup counter |
| Action| ActionID 79 ArgID 170| set current counter value 170 |
### Action 5 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 140, 480, 220, 0, 0, 12204, 12054|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 7| Select counter 7. Current counter is swapped with backup counter |
| Action| ActionID 54 ArgID 24| move room 24 |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 54 ArgID 11| move room 11 |
### Action 6 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 20, 20, 20, 0, 0, 11937, 8100|  |
| Probability| 0%|  |
| Action| ActionID 79 ArgID 1| set current counter value 1 |
| Action| ActionID 87 | Swap current location value with backup location-swap value |
| Action| ActionID 54 ArgID 1| move room 1 |
### Action 7 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 20, 140, 0, 0, 0, 12381, 11027|  |
| Probability| 100%|  |
| Action| ActionID 82 | add to current counter |
| Action| ActionID 81 ArgID 1| Select counter 1. Current counter is swapped with backup counter |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 77 | decrement current counter |
### Action 8 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 515, 309, 16, 0, 0, 15720, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 25| current counter less than 25 |
| Condition| ConditionID 8 ArgID 15| bitflag 15 is false |
| Condition| ConditionID 15 ArgID 0| current counter greater than '0' |
| Action| ActionID 104 | Print message 'Its getting' |
| Action| ActionID 120 | Print message 'dark\!' |
### Action 9 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 15, 340, 349, 0, 0, 15806, 11458|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Condition| ConditionID 8 ArgID 17| bitflag 17 is false |
| Action| ActionID 105 | Print message 'Sunset\!' |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 17| set 17 flag |
### Action 10 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 140, 60, 60, 0, 0, 12231, 11631|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 7| Select counter 7. Current counter is swapped with backup counter |
| Action| ActionID 81 ArgID 3| Select counter 3. Current counter is swapped with backup counter |
| Action| ActionID 77 | decrement current counter |
| Action| ActionID 81 ArgID 3| Select counter 3. Current counter is swapped with backup counter |
### Action 11 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 204, 349, 0, 0, 0, 8626, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Condition| ConditionID 8 ArgID 17| bitflag 17 is false |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 12 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 348, 1414, 224, 192, 1400, 7950, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 17| bitflag 17 is set |
| Condition| ConditionID 13 ArgID 70| item 'Ghostly square dance(index:70)' not in game |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Condition| ConditionID 11 ArgID 9| item 'Lit candle(index:9)' not carried or in room with player |
| Action| ActionID 53 ArgID 70| drops item 'Ghostly square dance(index:70)' into current room |
### Action 13 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 348, 227, 1414, 1400, 220, 9300, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 17| bitflag 17 is set |
| Condition| ConditionID 6 ArgID 11| player not in room 11 |
| Condition| ConditionID 13 ArgID 70| item 'Ghostly square dance(index:70)' not in game |
| Action| ActionID 62 ArgID 70, 11| item 'Ghostly square dance(index:70)' is moved to room 11 |
### Action 14 - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 4516, 120, 0, 0, 0, 8700, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 15 ArgID 225| current counter greater than '225' |
| Action| ActionID 58 ArgID 6| set 6 flag |
### Action 15 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 16 - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 60, 249, 0, 0, 0, 12223, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 8 ArgID 12| bitflag 12 is false |
| Action| ActionID 81 ArgID 3| Select counter 3. Current counter is swapped with backup counter |
| Action| ActionID 73 | continue with next action |
### Action 17 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 15, 460, 220, 0, 0, 4229, 9300|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Action| ActionID 28 | Print message 'Ding\-Ding' |
| Action| ActionID 29 | Print message 'Bell rings somewhere' |
| Action| ActionID 62 ArgID 23, 11| item 'Wraithlike figure playing equally ghostly piano(index:23)' is moved to room 11 |
### Action 18 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 15, 600, 80, 200, 80, 11931, 11931|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Action| ActionID 79 ArgID 30| set current counter value 30 |
| Action| ActionID 81 ArgID 4| Select counter 4. Current counter is swapped with backup counter |
| Action| ActionID 79 ArgID 10| set current counter value 10 |
| Action| ActionID 81 ArgID 4| Select counter 4. Current counter is swapped with backup counter |
### Action 19 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 60, 0, 0, 0, 0, 12150, 0|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 3| Select counter 3. Current counter is swapped with backup counter |
### Action 20 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 349, 1413, 1400, 0, 0, 8850, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 17| bitflag 17 is false |
| Condition| ConditionID 12 ArgID 70| item 'Ghostly square dance(index:70)' in game |
| Action| ActionID 59 ArgID 70| Item 'Ghostly square dance(index:70)' is removed from the game (put in room 0) |
### Action 21 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 473, 80, 0, 0, 0, 12227, 10950|  |
| Probability| 100%|  |
| Condition| ConditionID 12 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in game |
| Action| ActionID 81 ArgID 4| Select counter 4. Current counter is swapped with backup counter |
| Action| ActionID 77 | decrement current counter |
| Action| ActionID 73 | continue with next action |
### Action 22 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 15, 460, 0, 0, 0, 8920, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Action| ActionID 59 ArgID 23| Item 'Wraithlike figure playing equally ghostly piano(index:23)' is removed from the game (put in room 0) |
| Action| ActionID 70 | clear screen |
### Action 23 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 80, 0, 0, 0, 0, 12150, 0|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 4| Select counter 4. Current counter is swapped with backup counter |
### Action 24 - Probability: 4 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4, 494, 0, 0, 0, 0, 7551, 0|  |
| Probability| 4%|  |
| Condition| ConditionID 13 ArgID 24| item 'Piano with set of keys(index:24)' not in game |
| Action| ActionID 50 | Print message 'Ghostly voice whispers:' |
| Action| ActionID 51 | Print message 'Vain\.\.\.' |
### Action 25 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 368, 360, 120, 0, 0, 9081, 11623|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 18| bitflag 18 is set |
| Action| ActionID 60 ArgID 18| set 18 flag |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
| Action| ActionID 77 | decrement current counter |
| Action| ActionID 73 | continue with next action |
### Action 26 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 15, 280, 840, 0, 0, 10800, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 0| current counter less than 0 |
| Action| ActionID 72 ArgID 14, 42| swap item locations 'Matches(index:14)' and 'Empty matchbook(index:42)' |
### Action 27 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 120, 0, 0, 0, 0, 12150, 0|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
### Action 28 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1221, 181, 0, 0, 0, 19176, 9150|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 61| item 'Keg of gunpowder(index:61)' carried |
| Condition| ConditionID 0 ArgID 9| item 'Lit candle(index:9)' carried |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 126 | Print message 'TOO CLOSE\! Pieces of me rain down for days\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 29 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 30 - Probability: 15 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15, 44, 1434, 1413, 0, 0, 6160, 21900|  |
| Probability| 15%|  |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Condition| ConditionID 13 ArgID 71| item '\*SILVER CUP\*(index:71)' not in game |
| Condition| ConditionID 12 ArgID 70| item 'Ghostly square dance(index:70)' in game |
| Action| ActionID 41 | Print message 'I hear' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 146 | Print message 'in saloon' |
### Action 31 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 721, 706, 720, 0, 0, 8250, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 36| item 'Which I'm wearing(index:36)' carried |
| Condition| ConditionID 5 ArgID 35| item 'Stetson hat(index:35)' not carried |
| Action| ActionID 55 ArgID 36| Item 'Which I'm wearing(index:36)' is removed from the game (put in room 0) |
### Action 32 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 328, 320, 180, 0, 0, 9059, 11400|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 16| bitflag 16 is set |
| Action| ActionID 60 ArgID 16| set 16 flag |
| Action| ActionID 59 ArgID 9| Item 'Lit candle(index:9)' is removed from the game (put in room 0) |
| Action| ActionID 76 | look |
### Action 33 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 34 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 901, 0, 0, 0, 0, 18361, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 45| item 'Rattlesnake(index:45)' carried |
| Action| ActionID 122 | Print message 'I'm snake bit' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 35 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 36 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 764, 160, 0, 0, 0, 8700, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 38| player in room 38 |
| Action| ActionID 58 ArgID 8| set 8 flag |
### Action 37 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 168, 180, 0, 0, 0, 8700, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 8| bitflag 8 is set |
| Action| ActionID 58 ArgID 9| set 9 flag |
### Action 38 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 188, 180, 40, 0, 0, 9073, 12150|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 9| bitflag 9 is set |
| Action| ActionID 60 ArgID 9| set 9 flag |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
### Action 39 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 40, 0, 0, 0, 0, 2028, 2181|  |
| Probability| 0%|  |
| Action| ActionID 13 | Print message 'You've made' |
| Action| ActionID 78 | output current counter |
| Action| ActionID 14 | Print message 'BONUS points out of a possible 50 in' |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
### Action 40 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 11716, 9750|  |
| Probability| 0%|  |
| Action| ActionID 78 | output current counter |
| Action| ActionID 16 | Print message 'moves' |
| Action| ActionID 65 | score |
### Action 41 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 168, 0, 0, 0, 0, 9450, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 8| bitflag 8 is set |
| Action| ActionID 63 | game over |
### Action 42 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 40, 0, 0, 0, 0, 12223, 0|  |
| Probability| 100%|  |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
| Action| ActionID 73 | continue with next action |
### Action 43 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 128, 60, 120, 0, 0, 12510, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Action| ActionID 83 | subtract from current counter |
| Action| ActionID 60 ArgID 3| set 3 flag |
### Action 44 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 48, 60, 40, 0, 0, 12360, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Action| ActionID 82 | add to current counter |
| Action| ActionID 60 ArgID 3| set 3 flag |
### Action 45 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 68, 200, 60, 0, 0, 12360, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 82 | add to current counter |
| Action| ActionID 60 ArgID 10| set 10 flag |
### Action 46 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 108, 20, 100, 0, 0, 12360, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 5| bitflag 5 is set |
| Action| ActionID 82 | add to current counter |
| Action| ActionID 60 ArgID 1| set 1 flag |
### Action 47 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 40, 0, 0, 0, 0, 12150, 0|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
### Action 48 - Input: MIX FUSE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6100, 0, 0, 0, 0, 0, 7200, 0|  |
| Verb| 40| MIX |
| Noun| 100| FUSE |
| Action| ActionID 48 | Print message 'How?' |
### Action 49 - Input: GO SLEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 226, 0, 0, 0, 0, 0, 16200, 0|  |
| Verb| 1| GO |
| Noun| 76| SLEE |
| Action| ActionID 108 | Print message 'Try: SLEEP' |
### Action 50 - Input: SAVE GAME
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4507, 40, 40, 40, 0, 0, 12233, 12221|  |
| Verb| 30| SAVE |
| Noun| 7| GAME |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
| Action| ActionID 83 | subtract from current counter |
| Action| ActionID 81 ArgID 2| Select counter 2. Current counter is swapped with backup counter |
| Action| ActionID 71 | save game |
### Action 51 - Input: QUIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 160, 180, 0, 0, 0, 8758, 0|  |
| Verb| 31| QUIT |
| Noun| 0| ANY |
| Action| ActionID 58 ArgID 8| set 8 flag |
| Action| ActionID 58 ArgID 9| set 9 flag |
### Action 52 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 146, 0, 0, 0, 0, 905, 0|  |
| Verb| 38| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 7| item 'Shovel(index:7)' not carried |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 5 | Print message 'I've nothing to do that with' |
### Action 53 - Input: DIG MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5710, 141, 122, 160, 174, 0, 1060, 7950|  |
| Verb| 38| DIG |
| Noun| 10| MANU |
| Condition| ConditionID 0 ArgID 7| item 'Shovel(index:7)' carried |
| Condition| ConditionID 1 ArgID 6| item 'Manure pile(index:6)' in room with player |
| Condition| ConditionID 13 ArgID 8| item 'White crystals(index:8)' not in game |
| Action| ActionID 7 | Print message 'I found' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 53 ArgID 8| drops item 'White crystals(index:8)' into current room |
### Action 54 - Input: GET MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 122, 420, 120, 0, 0, 1351, 7858|  |
| Verb| 10| GET |
| Noun| 10| MANU |
| Condition| ConditionID 1 ArgID 6| item 'Manure pile(index:6)' in room with player |
| Action| ActionID 9 | Print message 'BARF\!' |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 52 ArgID 21| get item 'Male cow manure(index:21)', check if can carry |
| Action| ActionID 58 ArgID 6| set 6 flag |
### Action 55 - Input: GO MOUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 257, 0, 0, 0, 0, 0, 7200, 0|  |
| Verb| 1| GO |
| Noun| 107| MOUN |
| Action| ActionID 48 | Print message 'How?' |
### Action 56 - Input: SMEL SULF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6465, 203, 0, 0, 0, 0, 162, 21600|  |
| Verb| 43| SMEL |
| Noun| 15| SULF |
| Condition| ConditionID 2 ArgID 10| item 'Yellow powder(index:10)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 12 | Print message 'reminds me of' |
| Action| ActionID 144 | Print message 'rotten eggs' |
### Action 57 - Input: MIX ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6000, 163, 203, 223, 160, 200, 223, 8909|  |
| Verb| 40| MIX |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 8| item 'White crystals(index:8)' carried or in room with player |
| Condition| ConditionID 2 ArgID 10| item 'Yellow powder(index:10)' carried or in room with player |
| Condition| ConditionID 2 ArgID 11| item 'Sagebrush charcoal(index:11)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 59 ArgID 8| Item 'White crystals(index:8)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 10| Item 'Yellow powder(index:10)' is removed from the game (put in room 0) |
### Action 58 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 220, 240, 0, 0, 0, 8903, 0|  |
| Probability| 0%|  |
| Action| ActionID 59 ArgID 11| Item 'Sagebrush charcoal(index:11)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 12| drops item 'Pile of gunpowder(index:12)' into current room |
### Action 59 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1615, 60, 0, 0, 0, 8700, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 80| current counter less than 80 |
| Action| ActionID 58 ArgID 3| set 3 flag |
### Action 60 - Input: GO RAVI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 253, 164, 209, 0, 0, 0, 915, 0|  |
| Verb| 1| GO |
| Noun| 103| RAVI |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 15 | Print message 'its full of sage brush, tumbleweed & is impassable' |
### Action 61 - Input: GO RAVI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 253, 164, 208, 200, 0, 0, 204, 10500|  |
| Verb| 1| GO |
| Noun| 103| RAVI |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 10| move room 10 |
| Action| ActionID 70 | clear screen |
### Action 62 - Input: BURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 164, 209, 200, 283, 360, 167, 8758|  |
| Verb| 46| BURN |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 17 | Print message 'The dry wash is burnt clear' |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 58 ArgID 18| set 18 flag |
### Action 63 - Input: BREA MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10971, 302, 0, 0, 0, 0, 2868, 9150|  |
| Verb| 73| BREA |
| Noun| 21| MIRR |
| Condition| ConditionID 1 ArgID 15| item 'Mirror(index:15)' in room with player |
| Action| ActionID 19 | Print message 'Crack\!' |
| Action| ActionID 18 | Print message 'flying glass slices me up' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 64 - Input: LOOK MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3771, 302, 0, 0, 0, 0, 187, 0|  |
| Verb| 25| LOOK |
| Noun| 21| MIRR |
| Condition| ConditionID 1 ArgID 15| item 'Mirror(index:15)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 37 | Print message 'very pretty' |
### Action 65 - Input: SAY HOW
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5067, 1502, 600, 0, 0, 0, 7342, 8173|  |
| Verb| 33| SAY |
| Noun| 117| HOW |
| Condition| ConditionID 1 ArgID 75| item 'Indian ghost(index:75)' in room with player |
| Action| ActionID 48 | Print message 'How?' |
| Action| ActionID 142 | Print message 'Geronimo says: `Its easy\! Happy Landings\!`' |
| Action| ActionID 54 ArgID 30| move room 30 |
| Action| ActionID 73 | continue with next action |
### Action 66 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 2015, 60, 0, 0, 0, 11458, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 100| current counter less than 100 |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 3| set 3 flag |
### Action 67 - Input: GO HOLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 211, 362, 240, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 61| HOLE |
| Condition| ConditionID 1 ArgID 18| item 'Hole in the wall(index:18)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 12| move room 12 |
| Action| ActionID 76 | look |
### Action 68 - Input: LOOK COMP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3772, 383, 403, 0, 0, 0, 171, 3300|  |
| Verb| 25| LOOK |
| Noun| 22| COMP |
| Condition| ConditionID 2 ArgID 19| item 'Compass(index:19)' carried or in room with player |
| Condition| ConditionID 2 ArgID 20| item 'Horseshoe(index:20)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 21 | Print message 'its pointing to the' |
| Action| ActionID 22 | Print message 'horseshoe' |
### Action 69 - Input: GO JAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 42, 229, 0, 0, 0, 923, 0|  |
| Verb| 1| GO |
| Noun| 43| JAIL |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 8 ArgID 11| bitflag 11 is false |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 23 | Print message 'Doors closed, windows barred\!' |
### Action 70 - Input: HIT GHOS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9176, 462, 0, 0, 0, 0, 930, 0|  |
| Verb| 61| HIT |
| Noun| 26| GHOS |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 30 | Print message 'My hand passes thru\!' |
### Action 71 - Input: CLAP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 462, 240, 460, 480, 40, 8772, 8731|  |
| Verb| 66| CLAP |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 58 ArgID 12| set 12 flag |
| Action| ActionID 72 ArgID 23, 24| swap item locations 'Wraithlike figure playing equally ghostly piano(index:23)' and 'Piano with set of keys(index:24)' |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 31 | Print message 'Ghost stands, bows, vanishes\!' |
### Action 72 - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1531, 482, 745, 0, 0, 0, 4800, 0|  |
| Verb| 10| GET |
| Noun| 31| KEY |
| Condition| ConditionID 1 ArgID 24| item 'Piano with set of keys(index:24)' in room with player |
| Condition| ConditionID 4 ArgID 37| item 'Small key(index:37)' not in room with player |
| Action| ActionID 32 | Print message 'Silly, wrong type keys\!' |
### Action 73 - Input: GO JAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 42, 228, 260, 1133, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 43| JAIL |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Condition| ConditionID 12 ArgID 56| item '\* $200 \*(index:56)' in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 13| move room 13 |
| Action| ActionID 76 | look |
### Action 74 - Input: PLAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9600, 482, 269, 0, 0, 0, 183, 1534|  |
| Verb| 64| PLAY |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 24| item 'Piano with set of keys(index:24)' in room with player |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 33 | Print message 'Odd' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 34 | Print message 'goes thunk\!' |
### Action 75 - Input: PLAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9600, 482, 268, 0, 0, 0, 187, 0|  |
| Verb| 64| PLAY |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 24| item 'Piano with set of keys(index:24)' in room with player |
| Condition| ConditionID 7 ArgID 13| bitflag 13 is set |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 37 | Print message 'very pretty' |
### Action 76 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7565, 42, 229, 0, 0, 0, 3625, 0|  |
| Verb| 50| OPEN |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 8 ArgID 11| bitflag 11 is false |
| Action| ActionID 24 | Print message 'with what?' |
| Action| ActionID 25 | Print message 'Inside bolt is latched\!' |
### Action 77 - Input: WITH HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8723, 42, 229, 403, 220, 0, 10976, 8809|  |
| Verb| 58| WITH |
| Noun| 23| HORS |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 8 ArgID 11| bitflag 11 is false |
| Condition| ConditionID 2 ArgID 20| item 'Horseshoe(index:20)' carried or in room with player |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 26 | Print message 'Magnet\!' |
| Action| ActionID 58 ArgID 11| set 11 flag |
| Action| ActionID 109 | Print message 'it worked\!' |
### Action 78 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 615, 40, 0, 0, 0, 8700, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 30| current counter less than 30 |
| Action| ActionID 58 ArgID 2| set 2 flag |
### Action 79 - Input: HIT BELL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9175, 443, 544, 860, 874, 0, 18752, 1553|  |
| Verb| 61| HIT |
| Noun| 25| BELL |
| Condition| ConditionID 2 ArgID 22| item 'Large bell(index:22)' carried or in room with player |
| Condition| ConditionID 3 ArgID 27| player in room 27 |
| Condition| ConditionID 13 ArgID 43| item 'Bed(index:43)' not in game |
| Action| ActionID 125 | Print message 'Whoosh\!' |
| Action| ActionID 2 | Print message 'I see' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 53 ArgID 43| drops item 'Bed(index:43)' into current room |
### Action 80 - Input: WITH ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8700, 42, 229, 0, 0, 0, 12627, 0|  |
| Verb| 58| WITH |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 8 ArgID 11| bitflag 11 is false |
| Action| ActionID 84 | echo noun without cr |
| Action| ActionID 27 | Print message ' doesn't seem to do it\!' |
### Action 81 - Input: OPEN PIAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7587, 482, 260, 500, 269, 0, 1535, 8753|  |
| Verb| 50| OPEN |
| Noun| 87| PIAN |
| Condition| ConditionID 1 ArgID 24| item 'Piano with set of keys(index:24)' in room with player |
| Condition| ConditionID 8 ArgID 13| bitflag 13 is false |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 35 | Print message 'falls out' |
| Action| ActionID 58 ArgID 13| set 13 flag |
| Action| ActionID 53 ArgID 25| drops item 'Map(index:25)' into current room |
### Action 82 - Input: BURN CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6934, 523, 283, 520, 180, 360, 222, 11458|  |
| Verb| 46| BURN |
| Noun| 34| CAND |
| Condition| ConditionID 2 ArgID 26| item 'Unlit candle(index:26)' carried or in room with player |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 26, 9| swap item locations 'Unlit candle(index:26)' and 'Lit candle(index:9)' |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 18| set 18 flag |
### Action 83 - Input: UNLI CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10384, 183, 520, 180, 0, 0, 222, 11400|  |
| Verb| 69| UNLI |
| Noun| 34| CAND |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 26, 9| swap item locations 'Unlit candle(index:26)' and 'Lit candle(index:9)' |
| Action| ActionID 76 | look |
### Action 84 - Input: LIST ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10650, 462, 0, 0, 0, 0, 5550, 0|  |
| Verb| 71| LIST |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 37 | Print message 'very pretty' |
### Action 85 - Input: HIT BELL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9175, 443, 0, 0, 0, 0, 178, 7551|  |
| Verb| 61| HIT |
| Noun| 25| BELL |
| Condition| ConditionID 2 ArgID 22| item 'Large bell(index:22)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 28 | Print message 'Ding\-Ding' |
| Action| ActionID 50 | Print message 'Ghostly voice whispers:' |
| Action| ActionID 51 | Print message 'Vain\.\.\.' |
### Action 86 - Input: LOAD DERR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8439, 563, 0, 0, 0, 0, 189, 0|  |
| Verb| 56| LOAD |
| Noun| 39| DERR |
| Condition| ConditionID 2 ArgID 28| item '\*GOLDEN DERRINGER\*(index:28)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 39 | Print message 'it already is' |
### Action 87 - Input: GO STOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 192, 642, 300, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 42| STOR |
| Condition| ConditionID 1 ArgID 32| item 'Dry\-Goods store(index:32)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 76 | look |
### Action 88 - Input: READ SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10245, 663, 0, 0, 0, 0, 190, 0|  |
| Verb| 68| READ |
| Noun| 45| SIGN |
| Condition| ConditionID 2 ArgID 33| item 'Sign(index:33)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 40 | Print message 'Drop \*TREASURES\* then SCORE' |
### Action 89 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7565, 622, 620, 580, 743, 0, 222, 0|  |
| Verb| 50| OPEN |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 31| item 'Locked door(index:31)' in room with player |
| Condition| ConditionID 2 ArgID 37| item 'Small key(index:37)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 31, 29| swap item locations 'Locked door(index:31)' and 'Open door(index:29)' |
### Action 90 - Input: GO DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 215, 582, 280, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 29| item 'Open door(index:29)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 14| move room 14 |
| Action| ActionID 76 | look |
### Action 91 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7565, 622, 0, 0, 0, 0, 17100, 0|  |
| Verb| 50| OPEN |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 31| item 'Locked door(index:31)' in room with player |
| Action| ActionID 114 | Print message 'its locked\!' |
### Action 92 - Input: SCOR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4800, 180, 0, 0, 0, 0, 8700, 0|  |
| Verb| 32| SCOR |
| Noun| 0| ANY |
| Action| ActionID 58 ArgID 9| set 9 flag |
### Action 93 - Input: GO STAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 159, 82, 100, 0, 0, 0, 8176, 150|  |
| Verb| 1| GO |
| Noun| 9| STAB |
| Condition| ConditionID 1 ArgID 4| item 'Stable(index:4)' in room with player |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 76 | look |
| Action| ActionID 1 | Print message 'OK' |
### Action 94 - Input: GO SALO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 214, 62, 220, 0, 0, 0, 8176, 150|  |
| Verb| 1| GO |
| Noun| 64| SALO |
| Condition| ConditionID 1 ArgID 3| item 'Saloon(index:3)' in room with player |
| Action| ActionID 54 ArgID 11| move room 11 |
| Action| ActionID 76 | look |
| Action| ActionID 1 | Print message 'OK' |
### Action 95 - Input: LOOK COMP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3772, 383, 0, 0, 0, 0, 171, 3000|  |
| Verb| 25| LOOK |
| Noun| 22| COMP |
| Condition| ConditionID 2 ArgID 19| item 'Compass(index:19)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 21 | Print message 'its pointing to the' |
| Action| ActionID 20 | Print message 'north' |
### Action 96 - Input: GO BARB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 196, 22, 320, 0, 0, 0, 8176, 150|  |
| Verb| 1| GO |
| Noun| 46| BARB |
| Condition| ConditionID 1 ArgID 1| item 'Barbershop(index:1)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 76 | look |
| Action| ActionID 1 | Print message 'OK' |
### Action 97 - Input: LIST ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10650, 0, 0, 0, 0, 0, 191, 1650|  |
| Verb| 71| LIST |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 41 | Print message 'I hear' |
| Action| ActionID 11 | Print message 'nothing special' |
### Action 98 - Input: WITH NAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8799, 1203, 1243, 1240, 1200, 1180, 8922, 150|  |
| Verb| 58| WITH |
| Noun| 99| NAIL |
| Condition| ConditionID 2 ArgID 60| item 'Empty keg(index:60)' carried or in room with player |
| Condition| ConditionID 2 ArgID 62| item 'Nails(index:62)' carried or in room with player |
| Action| ActionID 59 ArgID 62| Item 'Nails(index:62)' is removed from the game (put in room 0) |
| Action| ActionID 72 ArgID 60, 59| swap item locations 'Empty keg(index:60)' and 'Keg of nails(index:59)' |
| Action| ActionID 1 | Print message 'OK' |
### Action 99 - Input: JUMP RAVI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11503, 164, 360, 0, 0, 0, 204, 11400|  |
| Verb| 76| JUMP |
| Noun| 103| RAVI |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 76 | look |
### Action 100 - Input: GO RAVI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 253, 364, 0, 0, 0, 0, 943, 0|  |
| Verb| 1| GO |
| Noun| 103| RAVI |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 43 | Print message 'Too steep\!' |
### Action 101 - Input: JUMP RAVI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11503, 364, 160, 0, 0, 0, 204, 11400|  |
| Verb| 76| JUMP |
| Noun| 103| RAVI |
| Condition| ConditionID 3 ArgID 18| player in room 18 |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 102 - Input: OPEN KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7598, 0, 0, 0, 0, 0, 5850, 0|  |
| Verb| 50| OPEN |
| Noun| 98| KEG |
| Action| ActionID 39 | Print message 'it already is' |
### Action 103 - Input: SMEL MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6460, 0, 0, 0, 0, 0, 1356, 0|  |
| Verb| 43| SMEL |
| Noun| 10| MANU |
| Action| ActionID 9 | Print message 'BARF\!' |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 104 - Input: SHAK HAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12068, 703, 754, 740, 40, 0, 8008, 1535|  |
| Verb| 80| SHAK |
| Noun| 68| HAT |
| Condition| ConditionID 2 ArgID 35| item 'Stetson hat(index:35)' carried or in room with player |
| Condition| ConditionID 13 ArgID 37| item 'Small key(index:37)' not in game |
| Action| ActionID 53 ArgID 37| drops item 'Small key(index:37)' into current room |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 35 | Print message 'falls out' |
### Action 105 - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1531, 743, 740, 0, 0, 0, 7801, 0|  |
| Verb| 10| GET |
| Noun| 31| KEY |
| Condition| ConditionID 2 ArgID 37| item 'Small key(index:37)' carried or in room with player |
| Action| ActionID 52 ArgID 37| get item 'Small key(index:37)', check if can carry |
| Action| ActionID 1 | Print message 'OK' |
### Action 106 - Input: WEAR HAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12518, 701, 720, 0, 0, 0, 11101, 10950|  |
| Verb| 83| WEAR |
| Noun| 68| HAT |
| Condition| ConditionID 0 ArgID 35| item 'Stetson hat(index:35)' carried |
| Action| ActionID 74 ArgID 36| take item 'Which I'm wearing(index:36)', no check done to see if can carry |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 73 | continue with next action |
### Action 107 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 754, 0, 0, 0, 0, 4960, 6600|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 37| item 'Small key(index:37)' not in game |
| Action| ActionID 33 | Print message 'Odd' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 44 | Print message 'feels strange' |
### Action 108 - Input: TAPE MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12321, 763, 302, 300, 780, 0, 222, 0|  |
| Verb| 82| TAPE |
| Noun| 21| MIRR |
| Condition| ConditionID 2 ArgID 38| item 'Roll of tape(index:38)' carried or in room with player |
| Condition| ConditionID 1 ArgID 15| item 'Mirror(index:15)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 15, 39| swap item locations 'Mirror(index:15)' and 'Taped up mirror(index:39)' |
### Action 109 - Input: BREA MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10971, 782, 780, 340, 360, 0, 222, 7950|  |
| Verb| 73| BREA |
| Noun| 21| MIRR |
| Condition| ConditionID 1 ArgID 39| item 'Taped up mirror(index:39)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 39, 17| swap item locations 'Taped up mirror(index:39)' and 'Broken mirror(index:17)' |
| Action| ActionID 53 ArgID 18| drops item 'Hole in the wall(index:18)' into current room |
### Action 110 - Input: LOOK HAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3818, 703, 0, 0, 0, 0, 152, 6750|  |
| Verb| 25| LOOK |
| Noun| 68| HAT |
| Condition| ConditionID 2 ArgID 35| item 'Stetson hat(index:35)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 2 | Print message 'I see' |
| Action| ActionID 45 | Print message 'its my size' |
### Action 111 - Input: GO STAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 213, 102, 380, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 63| STAL |
| Condition| ConditionID 1 ArgID 5| item 'Stall(index:5)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 19| move room 19 |
| Action| ActionID 76 | look |
### Action 112 - Input: KNOC GHOS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16676, 462, 0, 0, 0, 0, 930, 0|  |
| Verb| 111| KNOC |
| Noun| 26| GHOS |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 30 | Print message 'My hand passes thru\!' |
### Action 113 - Input: KNOC PIAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16737, 462, 0, 0, 0, 0, 930, 0|  |
| Verb| 111| KNOC |
| Noun| 87| PIAN |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 30 | Print message 'My hand passes thru\!' |
### Action 114 - Input: CROS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13200, 164, 0, 0, 0, 0, 7200, 0|  |
| Verb| 88| CROS |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 8| player in room 8 |
| Action| ActionID 48 | Print message 'How?' |
### Action 115 - Input: DIG ROOF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5744, 143, 464, 814, 800, 0, 7957, 1573|  |
| Verb| 38| DIG |
| Noun| 44| ROOF |
| Condition| ConditionID 2 ArgID 7| item 'Shovel(index:7)' carried or in room with player |
| Condition| ConditionID 3 ArgID 23| player in room 23 |
| Condition| ConditionID 13 ArgID 40| item '\*GOLD NUGGET\*(index:40)' not in game |
| Action| ActionID 53 ArgID 40| drops item '*GOLD NUGGET*(index:40)' into current room |
| Action| ActionID 7 | Print message 'I found' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 73 | continue with next action |
### Action 116 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1615, 60, 0, 0, 0, 8700, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 80| current counter less than 80 |
| Action| ActionID 58 ArgID 3| set 3 flag |
### Action 117 - Input: READ MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10233, 503, 0, 0, 0, 0, 199, 0|  |
| Verb| 68| READ |
| Noun| 33| MAP |
| Condition| ConditionID 2 ArgID 25| item 'Map(index:25)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 49 | Print message 'Its mine, dig roof\!' |
### Action 118 - Input: GO TELE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 223, 823, 480, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 73| TELE |
| Condition| ConditionID 2 ArgID 41| item 'Telegraph office(index:41)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 24| move room 24 |
| Action| ActionID 76 | look |
### Action 119 - Input: GO PAIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 225, 322, 500, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 75| PAIN |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 76 | look |
### Action 120 - Input: GET PAIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1575, 322, 0, 0, 0, 0, 6306, 16950|  |
| Verb| 10| GET |
| Noun| 75| PAIN |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Action| ActionID 42 | Print message 'What?' |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 113 | Print message 'Too big\!' |
### Action 121 - Input: GO HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 173, 322, 500, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 23| HORS |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 76 | look |
### Action 122 - Input: BURN MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6918, 283, 120, 360, 0, 0, 12223, 8700|  |
| Verb| 46| BURN |
| Noun| 18| MATC |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 58 ArgID 18| set 18 flag |
### Action 123 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 15388, 13200|  |
| Probability| 0%|  |
| Action| ActionID 102 | Print message 'Match flares up\.\.\.' |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
### Action 124 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 308, 280, 0, 0, 0, 8626, 8700|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
| Action| ActionID 58 ArgID 14| set 14 flag |
### Action 125 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 288, 0, 0, 0, 0, 13288, 13200|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 14| bitflag 14 is set |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
### Action 126 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 288, 280, 0, 0, 0, 9056, 11400|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 14| bitflag 14 is set |
| Action| ActionID 60 ArgID 14| set 14 flag |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 76 | look |
### Action 127 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 120, 0, 0, 0, 0, 12253, 0|  |
| Probability| 0%|  |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
| Action| ActionID 103 | Print message '\.\.\.and then goes out' |
### Action 128 - Input: SAY GIDD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5005, 504, 409, 0, 0, 0, 235, 17700|  |
| Verb| 33| SAY |
| Noun| 55| GIDD |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Condition| ConditionID 8 ArgID 20| bitflag 20 is false |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 118 | Print message 'He won't budge' |
### Action 129 - Input: GO MINE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 200, 262, 420, 0, 0, 0, 8454, 11401|  |
| Verb| 1| GO |
| Noun| 50| MINE |
| Condition| ConditionID 1 ArgID 13| item 'Entrance to a mine(index:13)' in room with player |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 76 | look |
| Action| ActionID 1 | Print message 'OK' |
### Action 130 - Input: SLEE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13350, 140, 3500, 140, 0, 0, 12229, 12223|  |
| Verb| 89| SLEE |
| Noun| 0| ANY |
| Action| ActionID 81 ArgID 7| Select counter 7. Current counter is swapped with backup counter |
| Action| ActionID 79 ArgID 175| set current counter value 175 |
| Action| ActionID 81 ArgID 7| Select counter 7. Current counter is swapped with backup counter |
| Action| ActionID 73 | continue with next action |
### Action 131 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 340, 0, 0, 0, 0, 17460, 13288|  |
| Probability| 0%|  |
| Action| ActionID 116 | Print message 'Good night' |
| Action| ActionID 60 ArgID 17| set 17 flag |
| Action| ActionID 88 | wait 2 seconds |
| Action| ActionID 88 | wait 2 seconds |
### Action 132 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 524, 0, 0, 0, 0, 17356, 8626|  |
| Probability| 0%|  |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Action| ActionID 115 | Print message 'Good Morning' |
| Action| ActionID 106 | Print message 'I feel refreshed' |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 133 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 527, 0, 0, 0, 0, 16111, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 6 ArgID 26| player not in room 26 |
| Action| ActionID 107 | Print message 'Nights are cold\! I caught Pneumonia' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 134 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 14, 0, 220, 0, 0, 9300, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 13 ArgID 0| item 'Worn out fiddle strings(index:0)' not in game |
| Action| ActionID 62 ArgID 0, 11| item 'Worn out fiddle strings(index:0)' is moved to room 11 |
### Action 135 - Input: GET UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1505, 524, 540, 0, 0, 0, 204, 11400|  |
| Verb| 10| GET |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 27| move room 27 |
| Action| ActionID 76 | look |
### Action 136 - Input: GO BED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 202, 862, 520, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 52| BED |
| Condition| ConditionID 1 ArgID 43| item 'Bed(index:43)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 26| move room 26 |
| Action| ActionID 76 | look |
### Action 137 - Input: GO HOTE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 203, 882, 560, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 53| HOTE |
| Condition| ConditionID 1 ArgID 44| item 'Hotel(index:44)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 28| move room 28 |
| Action| ActionID 76 | look |
### Action 138 - Input: SHOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8550, 903, 563, 900, 0, 0, 8888, 16460|  |
| Verb| 57| SHOO |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 45| item 'Rattlesnake(index:45)' carried or in room with player |
| Condition| ConditionID 2 ArgID 28| item '\*GOLDEN DERRINGER\*(index:28)' carried or in room with player |
| Action| ActionID 59 ArgID 45| Item 'Rattlesnake(index:45)' is removed from the game (put in room 0) |
| Action| ActionID 38 | Print message 'shoots stream of water' |
| Action| ActionID 109 | Print message 'it worked\!' |
| Action| ActionID 110 | Print message 'its gone' |
### Action 139 - Input: KILL SNAK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9827, 903, 0, 0, 0, 0, 16650, 0|  |
| Verb| 65| KILL |
| Noun| 77| SNAK |
| Condition| ConditionID 2 ArgID 45| item 'Rattlesnake(index:45)' carried or in room with player |
| Action| ActionID 111 | Print message 'snake won't let me' |
### Action 140 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 903, 0, 0, 0, 0, 16650, 0|  |
| Verb| 38| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 45| item 'Rattlesnake(index:45)' carried or in room with player |
| Action| ActionID 111 | Print message 'snake won't let me' |
### Action 141 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 905, 920, 404, 0, 0, 203, 0|  |
| Verb| 38| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 4 ArgID 45| item 'Rattlesnake(index:45)' not in room with player |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 53 ArgID 46| drops item 'Open grave(index:46)' into current room |
### Action 142 - Input: GO GRAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 164, 922, 580, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 14| GRAV |
| Condition| ConditionID 1 ArgID 46| item 'Open grave(index:46)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 29| move room 29 |
| Action| ActionID 76 | look |
### Action 143 - Input: KILL WORM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9829, 963, 960, 980, 100, 0, 222, 16858|  |
| Verb| 65| KILL |
| Noun| 79| WORM |
| Condition| ConditionID 2 ArgID 48| item 'Purple worm(index:48)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 48, 49| swap item locations 'Purple worm(index:48)' and 'Purple Slime(index:49)' |
| Action| ActionID 112 | Print message 'That felt good\!' |
| Action| ActionID 58 ArgID 5| set 5 flag |
### Action 144 - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1531, 1003, 0, 0, 0, 0, 900, 0|  |
| Verb| 10| GET |
| Noun| 31| KEY |
| Condition| ConditionID 2 ArgID 50| item 'Telegraph key(index:50)' carried or in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 145 - Input: MOVE KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13981, 1054, 0, 0, 0, 0, 161, 7050|  |
| Verb| 93| MOVE |
| Noun| 31| KEY |
| Condition| ConditionID 13 ArgID 52| item 'Spliced wire(index:52)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 47 | Print message 'happens' |
### Action 146 - Input: CONN WIRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13541, 1023, 1020, 1040, 0, 0, 222, 10950|  |
| Verb| 90| CONN |
| Noun| 41| WIRE |
| Condition| ConditionID 2 ArgID 51| item '2 loose wires(index:51)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 51, 52| swap item locations '2 loose wires(index:51)' and 'Spliced wire(index:52)' |
| Action| ActionID 73 | continue with next action |
### Action 147 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 615, 60, 0, 0, 0, 8700, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 14 ArgID 30| current counter less than 30 |
| Action| ActionID 58 ArgID 3| set 3 flag |
### Action 148 - Input: MOVE SAFE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13970, 1020, 1082, 1034, 1054, 1074, 203, 0|  |
| Verb| 93| MOVE |
| Noun| 20| SAFE |
| Condition| ConditionID 1 ArgID 54| item 'Large safe(index:54)' in room with player |
| Condition| ConditionID 13 ArgID 51| item '2 loose wires(index:51)' not in game |
| Condition| ConditionID 13 ArgID 52| item 'Spliced wire(index:52)' not in game |
| Condition| ConditionID 13 ArgID 53| item 'Pieces of wire(index:53)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 53 ArgID 51| drops item '2 loose wires(index:51)' into current room |
### Action 149 - Input: GET SAFE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 1082, 0, 0, 0, 0, 1013, 0|  |
| Verb| 10| GET |
| Noun| 20| SAFE |
| Condition| ConditionID 1 ArgID 54| item 'Large safe(index:54)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 113 | Print message 'Too big\!' |
### Action 150 - Input: OPEN SAFE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7520, 1082, 0, 0, 0, 0, 1014, 0|  |
| Verb| 50| OPEN |
| Noun| 20| SAFE |
| Condition| ConditionID 1 ArgID 54| item 'Large safe(index:54)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 114 | Print message 'its locked\!' |
### Action 151 - Input: GET WIRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1541, 1063, 1060, 0, 0, 0, 7801, 0|  |
| Verb| 10| GET |
| Noun| 41| WIRE |
| Condition| ConditionID 2 ArgID 53| item 'Pieces of wire(index:53)' carried or in room with player |
| Action| ActionID 52 ArgID 53| get item 'Pieces of wire(index:53)', check if can carry |
| Action| ActionID 1 | Print message 'OK' |
### Action 152 - Input: MOVE SAFE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13970, 1082, 0, 0, 0, 0, 150, 0|  |
| Verb| 93| MOVE |
| Noun| 20| SAFE |
| Condition| ConditionID 1 ArgID 54| item 'Large safe(index:54)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
### Action 153 - Input: MOVE PAIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14025, 322, 0, 0, 0, 0, 17700, 0|  |
| Verb| 93| MOVE |
| Noun| 75| PAIN |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Action| ActionID 118 | Print message 'He won't budge' |
### Action 154 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 184, 254, 214, 200, 0, 203, 1060|  |
| Verb| 38| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 13 ArgID 12| item 'Pile of gunpowder(index:12)' not in game |
| Condition| ConditionID 13 ArgID 10| item 'Yellow powder(index:10)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 53 ArgID 10| drops item 'Yellow powder(index:10)' into current room |
| Action| ActionID 7 | Print message 'I found' |
| Action| ActionID 10 | Print message 'something' |
### Action 155 - Input: GO JAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 42, 228, 1134, 260, 0, 7554, 11446|  |
| Verb| 1| GO |
| Noun| 43| JAIL |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Condition| ConditionID 13 ArgID 56| item '\* $200 \*(index:56)' not in game |
| Action| ActionID 50 | Print message 'Ghostly voice whispers:' |
| Action| ActionID 54 ArgID 13| move room 13 |
| Action| ActionID 76 | look |
| Action| ActionID 46 | Print message 'Don't collect $200 then don't pass GO\! CONTRAPOSITIVE\.' |
### Action 156 - Input: PASS GO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14639, 1134, 1120, 1143, 0, 0, 8000, 16350|  |
| Verb| 97| PASS |
| Noun| 89| GO |
| Condition| ConditionID 13 ArgID 56| item '\* $200 \*(index:56)' not in game |
| Condition| ConditionID 2 ArgID 57| item '\*ORIENTAL GO BOARD\*(index:57)' carried or in room with player |
| Action| ActionID 53 ArgID 56| drops item '* $200 *(index:56)' into current room |
| Action| ActionID 50 | Print message 'Ghostly voice whispers:' |
| Action| ActionID 109 | Print message 'it worked\!' |
### Action 157 - Input: MOVE PIAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14037, 482, 0, 0, 0, 0, 150, 0|  |
| Verb| 93| MOVE |
| Noun| 87| PIAN |
| Condition| ConditionID 1 ArgID 24| item 'Piano with set of keys(index:24)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
### Action 158 - Input: GET WIRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1541, 1023, 1020, 1060, 0, 0, 8924, 150|  |
| Verb| 10| GET |
| Noun| 41| WIRE |
| Condition| ConditionID 2 ArgID 51| item '2 loose wires(index:51)' carried or in room with player |
| Action| ActionID 59 ArgID 51| Item '2 loose wires(index:51)' is removed from the game (put in room 0) |
| Action| ActionID 74 ArgID 53| take item 'Pieces of wire(index:53)', no check done to see if can carry |
| Action| ActionID 1 | Print message 'OK' |
### Action 159 - Input: OPEN DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7565, 42, 228, 0, 0, 0, 5850, 0|  |
| Verb| 50| OPEN |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Action| ActionID 39 | Print message 'it already is' |
### Action 160 - Input: WAIT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14700, 900, 140, 900, 140, 0, 12381, 12531|  |
| Verb| 98| WAIT |
| Noun| 0| ANY |
| Action| ActionID 82 | add to current counter |
| Action| ActionID 81 ArgID 45| Select counter 45. Current counter is swapped with backup counter |
| Action| ActionID 83 | subtract from current counter |
| Action| ActionID 81 ArgID 7| Select counter 7. Current counter is swapped with backup counter |
### Action 161 - Input: WEAR SPUR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12517, 681, 0, 0, 0, 0, 150, 0|  |
| Verb| 83| WEAR |
| Noun| 67| SPUR |
| Condition| ConditionID 0 ArgID 34| item '\*SILVER SPURS\*(index:34)' carried |
| Action| ActionID 1 | Print message 'OK' |
### Action 162 - Input: CLEA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14850, 0, 0, 0, 0, 0, 7200, 0|  |
| Verb| 99| CLEA |
| Noun| 0| ANY |
| Action| ActionID 48 | Print message 'How?' |
### Action 163 - Input: LOOK MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3768, 283, 120, 120, 0, 0, 12228, 17931|  |
| Verb| 25| LOOK |
| Noun| 18| MATC |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
| Action| ActionID 78 | output current counter |
| Action| ActionID 119 | Print message 'left\!' |
| Action| ActionID 81 ArgID 6| Select counter 6. Current counter is swapped with backup counter |
### Action 164 - Input: JUMP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11400, 0, 0, 0, 0, 0, 6300, 0|  |
| Verb| 76| JUMP |
| Noun| 0| ANY |
| Action| ActionID 42 | Print message 'What?' |
### Action 165 - Input: BURN MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6933, 283, 360, 500, 503, 0, 8759, 150|  |
| Verb| 46| BURN |
| Noun| 33| MAP |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Condition| ConditionID 2 ArgID 25| item 'Map(index:25)' carried or in room with player |
| Action| ActionID 58 ArgID 18| set 18 flag |
| Action| ActionID 59 ArgID 25| Item 'Map(index:25)' is removed from the game (put in room 0) |
| Action| ActionID 1 | Print message 'OK' |
### Action 166 - Input: BURN MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6933, 183, 503, 500, 0, 0, 209, 0|  |
| Verb| 46| BURN |
| Noun| 33| MAP |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Condition| ConditionID 2 ArgID 25| item 'Map(index:25)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 59 ArgID 25| Item 'Map(index:25)' is removed from the game (put in room 0) |
### Action 167 - Input: BURN GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6913, 242, 183, 240, 0, 0, 209, 18750|  |
| Verb| 46| BURN |
| Noun| 13| GUNP |
| Condition| ConditionID 1 ArgID 12| item 'Pile of gunpowder(index:12)' in room with player |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 59 ArgID 12| Item 'Pile of gunpowder(index:12)' is removed from the game (put in room 0) |
| Action| ActionID 125 | Print message 'Whoosh\!' |
### Action 168 - Input: BURN GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6913, 242, 283, 360, 240, 0, 8701, 8975|  |
| Verb| 46| BURN |
| Noun| 13| GUNP |
| Condition| ConditionID 1 ArgID 12| item 'Pile of gunpowder(index:12)' in room with player |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 58 ArgID 18| set 18 flag |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 59 ArgID 12| Item 'Pile of gunpowder(index:12)' is removed from the game (put in room 0) |
| Action| ActionID 125 | Print message 'Whoosh\!' |
### Action 169 - Input: BURN GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6913, 1223, 183, 0, 0, 0, 277, 18961|  |
| Verb| 46| BURN |
| Noun| 13| GUNP |
| Condition| ConditionID 2 ArgID 61| item 'Keg of gunpowder(index:61)' carried or in room with player |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 126 | Print message 'TOO CLOSE\! Pieces of me rain down for days\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 170 - Input: BURN GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6913, 1223, 283, 0, 0, 0, 277, 18961|  |
| Verb| 46| BURN |
| Noun| 13| GUNP |
| Condition| ConditionID 2 ArgID 61| item 'Keg of gunpowder(index:61)' carried or in room with player |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 126 | Print message 'TOO CLOSE\! Pieces of me rain down for days\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 171 - Input: MOVE KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13981, 1053, 1002, 0, 0, 0, 19629, 19273|  |
| Verb| 93| MOVE |
| Noun| 31| KEY |
| Condition| ConditionID 12 ArgID 52| item 'Spliced wire(index:52)' in game |
| Condition| ConditionID 1 ArgID 50| item 'Telegraph key(index:50)' in room with player |
| Action| ActionID 130 | Print message 'Click' |
| Action| ActionID 129 | Print message 'SPARK\! \* \* \* \*' |
| Action| ActionID 128 | Print message '\.\.\. \.\.\.\. \.\-  \-\.\-  \.  \- \-\-\-  \.\-\-\.  \.\-\-\.  \.  \.\-\.' |
| Action| ActionID 73 | continue with next action |
### Action 172 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1223, 0, 0, 0, 0, 19477, 18961|  |
| Probability| 0%|  |
| Condition| ConditionID 2 ArgID 61| item 'Keg of gunpowder(index:61)' carried or in room with player |
| Action| ActionID 129 | Print message 'SPARK\! \* \* \* \*' |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 126 | Print message 'TOO CLOSE\! Pieces of me rain down for days\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 173 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 243, 240, 0, 0, 0, 19475, 8850|  |
| Probability| 0%|  |
| Condition| ConditionID 2 ArgID 12| item 'Pile of gunpowder(index:12)' carried or in room with player |
| Action| ActionID 129 | Print message 'SPARK\! \* \* \* \*' |
| Action| ActionID 125 | Print message 'Whoosh\!' |
| Action| ActionID 59 ArgID 12| Item 'Pile of gunpowder(index:12)' is removed from the game (put in room 0) |
### Action 174 - Input: SAY GIDD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5005, 504, 408, 0, 0, 0, 235, 11090|  |
| Verb| 33| SAY |
| Noun| 55| GIDD |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Condition| ConditionID 7 ArgID 20| bitflag 20 is set |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 73 | continue with next action |
| Action| ActionID 140 | Print message 'after a long ride' |
### Action 175 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 400, 0, 0, 0, 0, 18741, 9000|  |
| Probability| 0%|  |
| Action| ActionID 124 | Print message 'He bucks, I'm thrown' |
| Action| ActionID 141 | Print message 'he rides off without me' |
| Action| ActionID 60 ArgID 20| set 20 flag |
### Action 176 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 720, 320, 0, 0, 0, 8176, 8850|  |
| Probability| 0%|  |
| Action| ActionID 54 ArgID 36| move room 36 |
| Action| ActionID 76 | look |
| Action| ActionID 59 ArgID 16| Item ''ole Paint(index:16)' is removed from the game (put in room 0) |
### Action 177 - Input: GET INVE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1562, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 10| GET |
| Noun| 62| INVE |
| Action| ActionID 66 | output inventory |
### Action 178 - Input: INVE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9000, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 60| INVE |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
### Action 179 - Input: FIND ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12750, 0, 0, 0, 0, 0, 900, 0|  |
| Verb| 85| FIND |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 180 - Input: WITH GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8713, 1203, 243, 1200, 240, 1220, 8922, 150|  |
| Verb| 58| WITH |
| Noun| 13| GUNP |
| Condition| ConditionID 2 ArgID 60| item 'Empty keg(index:60)' carried or in room with player |
| Condition| ConditionID 2 ArgID 12| item 'Pile of gunpowder(index:12)' carried or in room with player |
| Action| ActionID 59 ArgID 60| Item 'Empty keg(index:60)' is removed from the game (put in room 0) |
| Action| ActionID 72 ArgID 12, 61| swap item locations 'Pile of gunpowder(index:12)' and 'Keg of gunpowder(index:61)' |
| Action| ActionID 1 | Print message 'OK' |
### Action 181 - Input: SAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4950, 0, 0, 0, 0, 0, 235, 0|  |
| Verb| 33| SAY |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
### Action 182 - Input: HELP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4350, 0, 0, 0, 0, 0, 900, 0|  |
| Verb| 29| HELP |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 183 - Input: BURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 283, 0, 0, 0, 0, 17550, 0|  |
| Verb| 46| BURN |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 14| item 'Matches(index:14)' carried or in room with player |
| Action| ActionID 117 | Print message 'Its fireproof' |
### Action 184 - Input: BURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 183, 0, 0, 0, 0, 17550, 0|  |
| Verb| 46| BURN |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 9| item 'Lit candle(index:9)' carried or in room with player |
| Action| ActionID 117 | Print message 'Its fireproof' |
### Action 185 - Input: BURN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 0, 0, 0, 0, 0, 905, 0|  |
| Verb| 46| BURN |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 5 | Print message 'I've nothing to do that with' |
### Action 186 - Input: SHOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8550, 563, 0, 0, 0, 0, 188, 0|  |
| Verb| 57| SHOO |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 28| item '\*GOLDEN DERRINGER\*(index:28)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 38 | Print message 'shoots stream of water' |
### Action 187 - Input: SPUR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 17250, 681, 504, 600, 1160, 380, 18654, 9300|  |
| Verb| 115| SPUR |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 34| item '\*SILVER SPURS\*(index:34)' carried |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 124 | Print message 'He bucks, I'm thrown' |
| Action| ActionID 54 ArgID 30| move room 30 |
| Action| ActionID 62 ArgID 58, 19| item 'Hole kicked in wall & bare hoof print(index:58)' is moved to room 19 |
### Action 188 - Input: DROP ON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2719, 0, 0, 0, 0, 0, 8, 0|  |
| Verb| 18| DROP |
| Noun| 19| ON |
| Action| ActionID 8 | Print message 'Wear?' |
### Action 189 - Input: PLAY PIAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9687, 462, 0, 0, 0, 0, 930, 0|  |
| Verb| 64| PLAY |
| Noun| 87| PIAN |
| Condition| ConditionID 1 ArgID 23| item 'Wraithlike figure playing equally ghostly piano(index:23)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 30 | Print message 'My hand passes thru\!' |
### Action 190 - Input: COVE SNAK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15077, 902, 703, 0, 0, 0, 271, 18361|  |
| Verb| 100| COVE |
| Noun| 77| SNAK |
| Condition| ConditionID 1 ArgID 45| item 'Rattlesnake(index:45)' in room with player |
| Condition| ConditionID 2 ArgID 35| item 'Stetson hat(index:35)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 121 | Print message 'Thru the Hat\!' |
| Action| ActionID 122 | Print message 'I'm snake bit' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 191 - Input: MOVE BED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14002, 862, 760, 389, 380, 0, 203, 8700|  |
| Verb| 93| MOVE |
| Noun| 52| BED |
| Condition| ConditionID 1 ArgID 43| item 'Bed(index:43)' in room with player |
| Condition| ConditionID 8 ArgID 19| bitflag 19 is false |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 53 ArgID 38| drops item 'Roll of tape(index:38)' into current room |
| Action| ActionID 58 ArgID 19| set 19 flag |
### Action 192 - Input: GO MIRR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 171, 0, 0, 0, 0, 0, 1023, 0|  |
| Verb| 1| GO |
| Noun| 21| MIRR |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 123 | Print message 'I'm not Alice\!' |
### Action 193 - Input: EMPT KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15548, 1183, 1200, 1180, 1240, 0, 222, 7950|  |
| Verb| 103| EMPT |
| Noun| 98| KEG |
| Condition| ConditionID 2 ArgID 59| item 'Keg of nails(index:59)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 60, 59| swap item locations 'Empty keg(index:60)' and 'Keg of nails(index:59)' |
| Action| ActionID 53 ArgID 62| drops item 'Nails(index:62)' into current room |
### Action 194 - Input: EMPT KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15548, 1223, 1200, 1220, 240, 0, 222, 7950|  |
| Verb| 103| EMPT |
| Noun| 98| KEG |
| Condition| ConditionID 2 ArgID 61| item 'Keg of gunpowder(index:61)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 72 ArgID 60, 61| swap item locations 'Empty keg(index:60)' and 'Keg of gunpowder(index:61)' |
| Action| ActionID 53 ArgID 12| drops item 'Pile of gunpowder(index:12)' into current room |
### Action 195 - Input: GET GUNP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1513, 243, 0, 0, 0, 0, 7200, 0|  |
| Verb| 10| GET |
| Noun| 13| GUNP |
| Condition| ConditionID 2 ArgID 12| item 'Pile of gunpowder(index:12)' carried or in room with player |
| Action| ActionID 48 | Print message 'How?' |
### Action 196 - Input: CLAP ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9900, 0, 0, 0, 0, 0, 150, 0|  |
| Verb| 66| CLAP |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
### Action 197 - Input: MOVE BED
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 14002, 862, 0, 0, 0, 0, 150, 0|  |
| Verb| 93| MOVE |
| Noun| 52| BED |
| Condition| ConditionID 1 ArgID 43| item 'Bed(index:43)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
### Action 198 - Input: MOVE KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13981, 1263, 1053, 0, 0, 0, 19580, 10950|  |
| Verb| 93| MOVE |
| Noun| 31| KEY |
| Condition| ConditionID 2 ArgID 63| item 'Telegraph key(index:63)' carried or in room with player |
| Condition| ConditionID 12 ArgID 52| item 'Spliced wire(index:52)' in game |
| Action| ActionID 130 | Print message 'Click' |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 73 | continue with next action |
### Action 199 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1222, 820, 1280, 1040, 0, 10927, 8850|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 61| item 'Keg of gunpowder(index:61)' in room with player |
| Action| ActionID 72 ArgID 41, 64| swap item locations 'Telegraph office(index:41)' and 'Smoking open safe(index:64)' |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 59 ArgID 52| Item 'Spliced wire(index:52)' is removed from the game (put in room 0) |
### Action 200 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 242, 240, 0, 0, 0, 8850, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 1 ArgID 12| item 'Pile of gunpowder(index:12)' in room with player |
| Action| ActionID 59 ArgID 12| Item 'Pile of gunpowder(index:12)' is removed from the game (put in room 0) |
### Action 201 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 12076, 0|  |
| Probability| 0%|  |
| Action| ActionID 80 | swap location with saved location |
| Action| ActionID 76 | look |
### Action 202 - Input: MOVE KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 13981, 1263, 1054, 0, 0, 0, 1697, 0|  |
| Verb| 93| MOVE |
| Noun| 31| KEY |
| Condition| ConditionID 2 ArgID 63| item 'Telegraph key(index:63)' carried or in room with player |
| Condition| ConditionID 13 ArgID 52| item 'Spliced wire(index:52)' not in game |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 47 | Print message 'happens' |
### Action 203 - Input: SHAK TOPP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12101, 0, 0, 0, 0, 0, 19650, 0|  |
| Verb| 80| SHAK |
| Noun| 101| TOPP |
| Action| ActionID 131 | Print message 'Is he a ghost? Anyway wrong idea\.' |
### Action 204 - Input: BREA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10950, 0, 0, 0, 0, 0, 900, 0|  |
| Verb| 73| BREA |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 205 - Input: GO PAIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 225, 504, 0, 0, 0, 0, 20850, 0|  |
| Verb| 1| GO |
| Noun| 75| PAIN |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 139 | Print message 'may need to say a magic word here' |
### Action 206 - Input: LOOK DOOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3815, 42, 0, 0, 0, 0, 19800, 0|  |
| Verb| 25| LOOK |
| Noun| 65| DOOR |
| Condition| ConditionID 1 ArgID 2| item 'Jail(index:2)' in room with player |
| Action| ActionID 132 | Print message 'There's not even a keyhole\!' |
### Action 207 - Input: KNOC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16650, 0, 0, 0, 0, 0, 161, 7050|  |
| Verb| 111| KNOC |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 47 | Print message 'happens' |
### Action 208 - Input: TAPE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 12300, 763, 0, 0, 0, 0, 19977, 0|  |
| Verb| 82| TAPE |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 38| item 'Roll of tape(index:38)' carried or in room with player |
| Action| ActionID 133 | Print message 'masking tape' |
| Action| ActionID 27 | Print message ' doesn't seem to do it\!' |
### Action 209 - Input: GO HOLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 211, 1162, 620, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 61| HOLE |
| Condition| ConditionID 1 ArgID 58| item 'Hole kicked in wall & bare hoof print(index:58)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 31| move room 31 |
| Action| ActionID 76 | look |
### Action 210 - Input: GO SHAC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 255, 1302, 660, 0, 0, 0, 204, 11534|  |
| Verb| 1| GO |
| Noun| 105| SHAC |
| Condition| ConditionID 1 ArgID 65| item 'Line shack(index:65)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 33| move room 33 |
| Action| ActionID 76 | look |
| Action| ActionID 134 | Print message 'Floorboards sure are creaky' |
### Action 211 - Input: LOOK FLOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3858, 664, 1334, 0, 0, 0, 152, 20250|  |
| Verb| 25| LOOK |
| Noun| 108| FLOO |
| Condition| ConditionID 3 ArgID 33| player in room 33 |
| Condition| ConditionID 13 ArgID 66| item 'Plank(index:66)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 2 | Print message 'I see' |
| Action| ActionID 135 | Print message 'Loose plank here' |
### Action 212 - Input: GET PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1609, 1334, 1320, 1340, 0, 0, 11153, 150|  |
| Verb| 10| GET |
| Noun| 109| PLAN |
| Condition| ConditionID 13 ArgID 66| item 'Plank(index:66)' not in game |
| Action| ActionID 74 ArgID 66| take item 'Plank(index:66)', no check done to see if can carry |
| Action| ActionID 53 ArgID 67| drops item 'Hole in floor(index:67)' into current room |
| Action| ActionID 1 | Print message 'OK' |
### Action 213 - Input: GET PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1609, 1323, 1320, 0, 0, 0, 7801, 0|  |
| Verb| 10| GET |
| Noun| 109| PLAN |
| Condition| ConditionID 2 ArgID 66| item 'Plank(index:66)' carried or in room with player |
| Action| ActionID 52 ArgID 66| get item 'Plank(index:66)', check if can carry |
| Action| ActionID 1 | Print message 'OK' |
### Action 214 - Input: GO HOLE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 211, 1342, 680, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 61| HOLE |
| Condition| ConditionID 1 ArgID 67| item 'Hole in floor(index:67)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 34| move room 34 |
| Action| ActionID 76 | look |
### Action 215 - Input: SMEL CRYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6545, 163, 0, 0, 0, 0, 162, 20400|  |
| Verb| 43| SMEL |
| Noun| 95| CRYS |
| Condition| ConditionID 2 ArgID 8| item 'White crystals(index:8)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 12 | Print message 'reminds me of' |
| Action| ActionID 136 | Print message 'salt peter' |
### Action 216 - Input: GO COUN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 269, 1382, 700, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 119| COUN |
| Condition| ConditionID 1 ArgID 69| item 'Counter(index:69)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 35| move room 35 |
| Action| ActionID 76 | look |
### Action 217 - Input: GET UP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1505, 604, 100, 0, 0, 0, 204, 11400|  |
| Verb| 10| GET |
| Noun| 5| UP |
| Condition| ConditionID 3 ArgID 30| player in room 30 |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 76 | look |
### Action 218 - Input: DANC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15750, 1402, 1434, 1420, 0, 0, 224, 5687|  |
| Verb| 105| DANC |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 70| item 'Ghostly square dance(index:70)' in room with player |
| Condition| ConditionID 13 ArgID 71| item '\*SILVER CUP\*(index:71)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 74 ArgID 71| take item '*SILVER CUP*(index:71)', no check done to see if can carry |
| Action| ActionID 37 | Print message 'very pretty' |
| Action| ActionID 137 | Print message 'I won a prize\!' |
### Action 219 - Input: DANC ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 15750, 0, 0, 0, 0, 0, 187, 1697|  |
| Verb| 105| DANC |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 37 | Print message 'very pretty' |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 47 | Print message 'happens' |
### Action 220 - Input: LOOK SAFE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3770, 1282, 1454, 1440, 0, 0, 203, 1060|  |
| Verb| 25| LOOK |
| Noun| 20| SAFE |
| Condition| ConditionID 1 ArgID 64| item 'Smoking open safe(index:64)' in room with player |
| Condition| ConditionID 13 ArgID 72| item '\*BAG GOLD DUST\*(index:72)' not in game |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 53 ArgID 72| drops item '*BAG GOLD DUST*(index:72)' into current room |
| Action| ActionID 7 | Print message 'I found' |
| Action| ActionID 10 | Print message 'something' |
### Action 221 - Input: SHOE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16500, 1243, 322, 403, 400, 1463, 209, 10950|  |
| Verb| 110| SHOE |
| Noun| 0| ANY |
| Condition| ConditionID 2 ArgID 62| item 'Nails(index:62)' carried or in room with player |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Condition| ConditionID 2 ArgID 20| item 'Horseshoe(index:20)' carried or in room with player |
| Condition| ConditionID 2 ArgID 73| item 'Hammer(index:73)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 59 ArgID 20| Item 'Horseshoe(index:20)' is removed from the game (put in room 0) |
| Action| ActionID 73 | continue with next action |
### Action 222 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1240, 400, 0, 0, 0, 8908, 0|  |
| Probability| 0%|  |
| Action| ActionID 59 ArgID 62| Item 'Nails(index:62)' is removed from the game (put in room 0) |
| Action| ActionID 58 ArgID 20| set 20 flag |
### Action 223 - Input: SHOE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16500, 322, 1183, 0, 0, 0, 1038, 0|  |
| Verb| 110| SHOE |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Condition| ConditionID 2 ArgID 59| item 'Keg of nails(index:59)' carried or in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 138 | Print message 'reach a nail' |
### Action 224 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 141, 0, 0, 0, 0, 1061, 0|  |
| Verb| 38| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 7| item 'Shovel(index:7)' carried |
| Action| ActionID 7 | Print message 'I found' |
| Action| ActionID 11 | Print message 'nothing special' |
### Action 225 - Input: GO TEEP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 265, 1482, 740, 0, 0, 0, 204, 11400|  |
| Verb| 1| GO |
| Noun| 115| TEEP |
| Condition| ConditionID 1 ArgID 74| item 'TeePee(index:74)' in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 54 ArgID 37| move room 37 |
| Action| ActionID 76 | look |
### Action 226 - Input: HIT TOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9266, 1523, 1514, 1500, 0, 0, 19177, 8059|  |
| Verb| 61| HIT |
| Noun| 116| TOM |
| Condition| ConditionID 2 ArgID 76| item '\*SACRED TOM TOM\*(index:76)' carried or in room with player |
| Condition| ConditionID 13 ArgID 75| item 'Indian ghost(index:75)' not in game |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 53 ArgID 75| drops item 'Indian ghost(index:75)' into current room |
| Action| ActionID 109 | Print message 'it worked\!' |
### Action 227 - Input: HIT TOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9266, 1523, 1513, 0, 0, 0, 127, 19050|  |
| Verb| 61| HIT |
| Noun| 116| TOM |
| Condition| ConditionID 2 ArgID 76| item '\*SACRED TOM TOM\*(index:76)' carried or in room with player |
| Condition| ConditionID 12 ArgID 75| item 'Indian ghost(index:75)' in game |
| Action| ActionID 127 | Print message 'Boom\!' |
| Action| ActionID 127 | Print message 'Boom\!' |
### Action 228 - Input: SHOE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16500, 322, 0, 0, 0, 0, 910, 21450|  |
| Verb| 110| SHOE |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 16| item ''ole Paint(index:16)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 143 | Print message 'is missing' |
### Action 229 - Input: HIT GHOS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9176, 1502, 0, 0, 0, 0, 930, 0|  |
| Verb| 61| HIT |
| Noun| 26| GHOS |
| Condition| ConditionID 1 ArgID 75| item 'Indian ghost(index:75)' in room with player |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 30 | Print message 'My hand passes thru\!' |
### Action 230 - Input: FILL KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 16148, 1203, 0, 0, 0, 0, 174, 0|  |
| Verb| 107| FILL |
| Noun| 98| KEG |
| Condition| ConditionID 2 ArgID 60| item 'Empty keg(index:60)' carried or in room with player |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 24 | Print message 'with what?' |
### Action 231 - Input: LOOK ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 0, 0, 0, 0, 0, 152, 1726|  |
| Verb| 25| LOOK |
| Noun| 0| ANY |
| Action| ActionID 1 | Print message 'OK' |
| Action| ActionID 2 | Print message 'I see' |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 76 | look |
### Action 232 - Input: MIX ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6000, 0, 0, 0, 0, 0, 910, 21450|  |
| Verb| 40| MIX |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 10 | Print message 'something' |
| Action| ActionID 143 | Print message 'is missing' |
### Action 233 - Input: GO HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 173, 504, 0, 0, 0, 0, 20850, 0|  |
| Verb| 1| GO |
| Noun| 23| HORS |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 139 | Print message 'may need to say a magic word here' |
### Action 234 - Input: SPUR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 17250, 0, 0, 0, 0, 0, 1697, 0|  |
| Verb| 115| SPUR |
| Noun| 0| ANY |
| Action| ActionID 11 | Print message 'nothing special' |
| Action| ActionID 47 | Print message 'happens' |
### Action 235 - Input: WITH ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8700, 0, 0, 0, 0, 0, 984, 4050|  |
| Verb| 58| WITH |
| Noun| 0| ANY |
| Action| ActionID 6 | Print message 'Sorry I can't' |
| Action| ActionID 84 | echo noun without cr |
| Action| ActionID 27 | Print message ' doesn't seem to do it\!' |
### Action 236 - Input: GO MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 0, 0, 0, 0, 0, 1356, 0|  |
| Verb| 1| GO |
| Noun| 10| MANU |
| Action| ActionID 9 | Print message 'BARF\!' |
| Action| ActionID 6 | Print message 'Sorry I can't' |
### Action 237 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 239 - Take for item Worn out fiddle strings - Input: GET STRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 69| STRI |
| Condition| ConditionID 1 ArgID 0| item 'Worn out fiddle strings(index:0)' in room with player |
| Action| ActionID 52 ArgID 0| get item 'Worn out fiddle strings(index:0)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 240 - Drop for item Worn out fiddle strings - Input: DROP STRI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 69| STRI |
| Condition| ConditionID 0 ArgID 0| item 'Worn out fiddle strings(index:0)' carried |
| Action| ActionID 53 ArgID 0| drops item 'Worn out fiddle strings(index:0)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 241 - Take for item Shovel - Input: GET SHOV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 81| SHOV |
| Condition| ConditionID 1 ArgID 7| item 'Shovel(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Shovel(index:7)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 242 - Drop for item Shovel - Input: DROP SHOV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 81| SHOV |
| Condition| ConditionID 0 ArgID 7| item 'Shovel(index:7)' carried |
| Action| ActionID 53 ArgID 7| drops item 'Shovel(index:7)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 243 - Take for item White crystals - Input: GET CRYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 95| CRYS |
| Condition| ConditionID 1 ArgID 8| item 'White crystals(index:8)' in room with player |
| Action| ActionID 52 ArgID 8| get item 'White crystals(index:8)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 244 - Drop for item White crystals - Input: DROP CRYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 95| CRYS |
| Condition| ConditionID 0 ArgID 8| item 'White crystals(index:8)' carried |
| Action| ActionID 53 ArgID 8| drops item 'White crystals(index:8)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 245 - Take for item Lit candle - Input: GET CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| CAND |
| Condition| ConditionID 1 ArgID 9| item 'Lit candle(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Lit candle(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 246 - Drop for item Lit candle - Input: DROP CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 34| CAND |
| Condition| ConditionID 0 ArgID 9| item 'Lit candle(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Lit candle(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 247 - Take for item Yellow powder - Input: GET SULF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 15| SULF |
| Condition| ConditionID 1 ArgID 10| item 'Yellow powder(index:10)' in room with player |
| Action| ActionID 52 ArgID 10| get item 'Yellow powder(index:10)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 248 - Drop for item Yellow powder - Input: DROP SULF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 15| SULF |
| Condition| ConditionID 0 ArgID 10| item 'Yellow powder(index:10)' carried |
| Action| ActionID 53 ArgID 10| drops item 'Yellow powder(index:10)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 249 - Take for item Sagebrush charcoal - Input: GET CHAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 17| CHAR |
| Condition| ConditionID 1 ArgID 11| item 'Sagebrush charcoal(index:11)' in room with player |
| Action| ActionID 52 ArgID 11| get item 'Sagebrush charcoal(index:11)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 250 - Drop for item Sagebrush charcoal - Input: DROP CHAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 17| CHAR |
| Condition| ConditionID 0 ArgID 11| item 'Sagebrush charcoal(index:11)' carried |
| Action| ActionID 53 ArgID 11| drops item 'Sagebrush charcoal(index:11)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 251 - Take for item Matches - Input: GET MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 18| MATC |
| Condition| ConditionID 1 ArgID 14| item 'Matches(index:14)' in room with player |
| Action| ActionID 52 ArgID 14| get item 'Matches(index:14)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 252 - Drop for item Matches - Input: DROP MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 18| MATC |
| Condition| ConditionID 0 ArgID 14| item 'Matches(index:14)' carried |
| Action| ActionID 53 ArgID 14| drops item 'Matches(index:14)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 253 - Take for item Compass - Input: GET COMP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 22| COMP |
| Condition| ConditionID 1 ArgID 19| item 'Compass(index:19)' in room with player |
| Action| ActionID 52 ArgID 19| get item 'Compass(index:19)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 254 - Drop for item Compass - Input: DROP COMP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 22| COMP |
| Condition| ConditionID 0 ArgID 19| item 'Compass(index:19)' carried |
| Action| ActionID 53 ArgID 19| drops item 'Compass(index:19)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 255 - Take for item Horseshoe - Input: GET HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 23| HORS |
| Condition| ConditionID 1 ArgID 20| item 'Horseshoe(index:20)' in room with player |
| Action| ActionID 52 ArgID 20| get item 'Horseshoe(index:20)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 256 - Drop for item Horseshoe - Input: DROP HORS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 23| HORS |
| Condition| ConditionID 0 ArgID 20| item 'Horseshoe(index:20)' carried |
| Action| ActionID 53 ArgID 20| drops item 'Horseshoe(index:20)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 257 - Take for item Male cow manure - Input: GET MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 10| MANU |
| Condition| ConditionID 1 ArgID 21| item 'Male cow manure(index:21)' in room with player |
| Action| ActionID 52 ArgID 21| get item 'Male cow manure(index:21)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 258 - Drop for item Male cow manure - Input: DROP MANU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 10| MANU |
| Condition| ConditionID 0 ArgID 21| item 'Male cow manure(index:21)' carried |
| Action| ActionID 53 ArgID 21| drops item 'Male cow manure(index:21)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 259 - Take for item Large bell - Input: GET BELL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 25| BELL |
| Condition| ConditionID 1 ArgID 22| item 'Large bell(index:22)' in room with player |
| Action| ActionID 52 ArgID 22| get item 'Large bell(index:22)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 260 - Drop for item Large bell - Input: DROP BELL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 25| BELL |
| Condition| ConditionID 0 ArgID 22| item 'Large bell(index:22)' carried |
| Action| ActionID 53 ArgID 22| drops item 'Large bell(index:22)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 261 - Take for item Map - Input: GET MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 33| MAP |
| Condition| ConditionID 1 ArgID 25| item 'Map(index:25)' in room with player |
| Action| ActionID 52 ArgID 25| get item 'Map(index:25)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 262 - Drop for item Map - Input: DROP MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 33| MAP |
| Condition| ConditionID 0 ArgID 25| item 'Map(index:25)' carried |
| Action| ActionID 53 ArgID 25| drops item 'Map(index:25)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 263 - Take for item Unlit candle - Input: GET CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| CAND |
| Condition| ConditionID 1 ArgID 26| item 'Unlit candle(index:26)' in room with player |
| Action| ActionID 52 ArgID 26| get item 'Unlit candle(index:26)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 264 - Drop for item Unlit candle - Input: DROP CAND
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 34| CAND |
| Condition| ConditionID 0 ArgID 26| item 'Unlit candle(index:26)' carried |
| Action| ActionID 53 ArgID 26| drops item 'Unlit candle(index:26)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 265 - Take for item *SILVER BULLET* - Input: GET BULL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 37| BULL |
| Condition| ConditionID 1 ArgID 27| item '\*SILVER BULLET\*(index:27)' in room with player |
| Action| ActionID 52 ArgID 27| get item '*SILVER BULLET*(index:27)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 266 - Drop for item *SILVER BULLET* - Input: DROP BULL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 37| BULL |
| Condition| ConditionID 0 ArgID 27| item '\*SILVER BULLET\*(index:27)' carried |
| Action| ActionID 53 ArgID 27| drops item '*SILVER BULLET*(index:27)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 267 - Take for item *GOLDEN DERRINGER* - Input: GET DERR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 39| DERR |
| Condition| ConditionID 1 ArgID 28| item '\*GOLDEN DERRINGER\*(index:28)' in room with player |
| Action| ActionID 52 ArgID 28| get item '*GOLDEN DERRINGER*(index:28)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 268 - Drop for item *GOLDEN DERRINGER* - Input: DROP DERR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 39| DERR |
| Condition| ConditionID 0 ArgID 28| item '\*GOLDEN DERRINGER\*(index:28)' carried |
| Action| ActionID 53 ArgID 28| drops item '*GOLDEN DERRINGER*(index:28)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 269 - Take for item Sign-`Ring for ROOM service` - Input: GET SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 45| SIGN |
| Condition| ConditionID 1 ArgID 30| item 'Sign\-`Ring for ROOM service`(index:30)' in room with player |
| Action| ActionID 52 ArgID 30| get item 'Sign-`Ring for ROOM service`(index:30)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 270 - Drop for item Sign-`Ring for ROOM service` - Input: DROP SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 45| SIGN |
| Condition| ConditionID 0 ArgID 30| item 'Sign\-`Ring for ROOM service`(index:30)' carried |
| Action| ActionID 53 ArgID 30| drops item 'Sign-`Ring for ROOM service`(index:30)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 271 - Take for item Sign - Input: GET SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 45| SIGN |
| Condition| ConditionID 1 ArgID 33| item 'Sign(index:33)' in room with player |
| Action| ActionID 52 ArgID 33| get item 'Sign(index:33)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 272 - Drop for item Sign - Input: DROP SIGN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 45| SIGN |
| Condition| ConditionID 0 ArgID 33| item 'Sign(index:33)' carried |
| Action| ActionID 53 ArgID 33| drops item 'Sign(index:33)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 273 - Take for item *SILVER SPURS* - Input: GET SPUR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 67| SPUR |
| Condition| ConditionID 1 ArgID 34| item '\*SILVER SPURS\*(index:34)' in room with player |
| Action| ActionID 52 ArgID 34| get item '*SILVER SPURS*(index:34)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 274 - Drop for item *SILVER SPURS* - Input: DROP SPUR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 67| SPUR |
| Condition| ConditionID 0 ArgID 34| item '\*SILVER SPURS\*(index:34)' carried |
| Action| ActionID 53 ArgID 34| drops item '*SILVER SPURS*(index:34)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 275 - Take for item Stetson hat - Input: GET HAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 68| HAT |
| Condition| ConditionID 1 ArgID 35| item 'Stetson hat(index:35)' in room with player |
| Action| ActionID 52 ArgID 35| get item 'Stetson hat(index:35)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 276 - Drop for item Stetson hat - Input: DROP HAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 68| HAT |
| Condition| ConditionID 0 ArgID 35| item 'Stetson hat(index:35)' carried |
| Action| ActionID 53 ArgID 35| drops item 'Stetson hat(index:35)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 277 - Take for item Small key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 31| KEY |
| Condition| ConditionID 1 ArgID 37| item 'Small key(index:37)' in room with player |
| Action| ActionID 52 ArgID 37| get item 'Small key(index:37)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 278 - Drop for item Small key - Input: DROP KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 31| KEY |
| Condition| ConditionID 0 ArgID 37| item 'Small key(index:37)' carried |
| Action| ActionID 53 ArgID 37| drops item 'Small key(index:37)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 279 - Take for item Roll of tape - Input: GET TAPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 70| TAPE |
| Condition| ConditionID 1 ArgID 38| item 'Roll of tape(index:38)' in room with player |
| Action| ActionID 52 ArgID 38| get item 'Roll of tape(index:38)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 280 - Drop for item Roll of tape - Input: DROP TAPE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 70| TAPE |
| Condition| ConditionID 0 ArgID 38| item 'Roll of tape(index:38)' carried |
| Action| ActionID 53 ArgID 38| drops item 'Roll of tape(index:38)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 281 - Take for item *GOLD NUGGET* - Input: GET GOLD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 96| GOLD |
| Condition| ConditionID 1 ArgID 40| item '\*GOLD NUGGET\*(index:40)' in room with player |
| Action| ActionID 52 ArgID 40| get item '*GOLD NUGGET*(index:40)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 282 - Drop for item *GOLD NUGGET* - Input: DROP GOLD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 96| GOLD |
| Condition| ConditionID 0 ArgID 40| item '\*GOLD NUGGET\*(index:40)' carried |
| Action| ActionID 53 ArgID 40| drops item '*GOLD NUGGET*(index:40)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 283 - Take for item Empty matchbook - Input: GET MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 18| MATC |
| Condition| ConditionID 1 ArgID 42| item 'Empty matchbook(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Empty matchbook(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 284 - Drop for item Empty matchbook - Input: DROP MATC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 18| MATC |
| Condition| ConditionID 0 ArgID 42| item 'Empty matchbook(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Empty matchbook(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 285 - Take for item Rattlesnake - Input: GET SNAK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 77| SNAK |
| Condition| ConditionID 1 ArgID 45| item 'Rattlesnake(index:45)' in room with player |
| Action| ActionID 52 ArgID 45| get item 'Rattlesnake(index:45)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 286 - Drop for item Rattlesnake - Input: DROP SNAK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 77| SNAK |
| Condition| ConditionID 0 ArgID 45| item 'Rattlesnake(index:45)' carried |
| Action| ActionID 53 ArgID 45| drops item 'Rattlesnake(index:45)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 287 - Take for item *GOLD COIN* - Input: GET COIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 59| COIN |
| Condition| ConditionID 1 ArgID 47| item '\*GOLD COIN\*(index:47)' in room with player |
| Action| ActionID 52 ArgID 47| get item '*GOLD COIN*(index:47)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 288 - Drop for item *GOLD COIN* - Input: DROP COIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 59| COIN |
| Condition| ConditionID 0 ArgID 47| item '\*GOLD COIN\*(index:47)' carried |
| Action| ActionID 53 ArgID 47| drops item '*GOLD COIN*(index:47)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 289 - Take for item Purple worm - Input: GET WORM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 79| WORM |
| Condition| ConditionID 1 ArgID 48| item 'Purple worm(index:48)' in room with player |
| Action| ActionID 52 ArgID 48| get item 'Purple worm(index:48)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 290 - Drop for item Purple worm - Input: DROP WORM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 79| WORM |
| Condition| ConditionID 0 ArgID 48| item 'Purple worm(index:48)' carried |
| Action| ActionID 53 ArgID 48| drops item 'Purple worm(index:48)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 291 - Take for item Purple Slime - Input: GET WORM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 79| WORM |
| Condition| ConditionID 1 ArgID 49| item 'Purple Slime(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item 'Purple Slime(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 292 - Drop for item Purple Slime - Input: DROP WORM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 79| WORM |
| Condition| ConditionID 0 ArgID 49| item 'Purple Slime(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item 'Purple Slime(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 293 - Take for item Pieces of wire - Input: GET WIRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 41| WIRE |
| Condition| ConditionID 1 ArgID 53| item 'Pieces of wire(index:53)' in room with player |
| Action| ActionID 52 ArgID 53| get item 'Pieces of wire(index:53)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 294 - Drop for item Pieces of wire - Input: DROP WIRE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 41| WIRE |
| Condition| ConditionID 0 ArgID 53| item 'Pieces of wire(index:53)' carried |
| Action| ActionID 53 ArgID 53| drops item 'Pieces of wire(index:53)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 295 - Take for item *CASHBOX* - Input: GET BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 82| BOX |
| Condition| ConditionID 1 ArgID 55| item '\*CASHBOX\*(index:55)' in room with player |
| Action| ActionID 52 ArgID 55| get item '*CASHBOX*(index:55)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 296 - Drop for item *CASHBOX* - Input: DROP BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 82| BOX |
| Condition| ConditionID 0 ArgID 55| item '\*CASHBOX\*(index:55)' carried |
| Action| ActionID 53 ArgID 55| drops item '*CASHBOX*(index:55)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 297 - Take for item * $200 * - Input: GET $200
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 88| $200 |
| Condition| ConditionID 1 ArgID 56| item '\* $200 \*(index:56)' in room with player |
| Action| ActionID 52 ArgID 56| get item '* $200 *(index:56)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 298 - Drop for item * $200 * - Input: DROP $200
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 88| $200 |
| Condition| ConditionID 0 ArgID 56| item '\* $200 \*(index:56)' carried |
| Action| ActionID 53 ArgID 56| drops item '* $200 *(index:56)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 299 - Take for item *ORIENTAL GO BOARD* - Input: GET GO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 89| GO |
| Condition| ConditionID 1 ArgID 57| item '\*ORIENTAL GO BOARD\*(index:57)' in room with player |
| Action| ActionID 52 ArgID 57| get item '*ORIENTAL GO BOARD*(index:57)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 300 - Drop for item *ORIENTAL GO BOARD* - Input: DROP GO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 89| GO |
| Condition| ConditionID 0 ArgID 57| item '\*ORIENTAL GO BOARD\*(index:57)' carried |
| Action| ActionID 53 ArgID 57| drops item '*ORIENTAL GO BOARD*(index:57)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 301 - Take for item Keg of nails - Input: GET KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 98| KEG |
| Condition| ConditionID 1 ArgID 59| item 'Keg of nails(index:59)' in room with player |
| Action| ActionID 52 ArgID 59| get item 'Keg of nails(index:59)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 302 - Drop for item Keg of nails - Input: DROP KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 98| KEG |
| Condition| ConditionID 0 ArgID 59| item 'Keg of nails(index:59)' carried |
| Action| ActionID 53 ArgID 59| drops item 'Keg of nails(index:59)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 303 - Take for item Empty keg - Input: GET KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 98| KEG |
| Condition| ConditionID 1 ArgID 60| item 'Empty keg(index:60)' in room with player |
| Action| ActionID 52 ArgID 60| get item 'Empty keg(index:60)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 304 - Drop for item Empty keg - Input: DROP KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 98| KEG |
| Condition| ConditionID 0 ArgID 60| item 'Empty keg(index:60)' carried |
| Action| ActionID 53 ArgID 60| drops item 'Empty keg(index:60)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 305 - Take for item Keg of gunpowder - Input: GET KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 98| KEG |
| Condition| ConditionID 1 ArgID 61| item 'Keg of gunpowder(index:61)' in room with player |
| Action| ActionID 52 ArgID 61| get item 'Keg of gunpowder(index:61)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 306 - Drop for item Keg of gunpowder - Input: DROP KEG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 98| KEG |
| Condition| ConditionID 0 ArgID 61| item 'Keg of gunpowder(index:61)' carried |
| Action| ActionID 53 ArgID 61| drops item 'Keg of gunpowder(index:61)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 307 - Take for item Nails - Input: GET NAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 99| NAIL |
| Condition| ConditionID 1 ArgID 62| item 'Nails(index:62)' in room with player |
| Action| ActionID 52 ArgID 62| get item 'Nails(index:62)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 308 - Drop for item Nails - Input: DROP NAIL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 99| NAIL |
| Condition| ConditionID 0 ArgID 62| item 'Nails(index:62)' carried |
| Action| ActionID 53 ArgID 62| drops item 'Nails(index:62)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 309 - Take for item Plank - Input: GET PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 109| PLAN |
| Condition| ConditionID 1 ArgID 66| item 'Plank(index:66)' in room with player |
| Action| ActionID 52 ArgID 66| get item 'Plank(index:66)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 310 - Drop for item Plank - Input: DROP PLAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 109| PLAN |
| Condition| ConditionID 0 ArgID 66| item 'Plank(index:66)' carried |
| Action| ActionID 53 ArgID 66| drops item 'Plank(index:66)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 311 - Take for item *PELTS* - Input: GET PELT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 110| PELT |
| Condition| ConditionID 1 ArgID 68| item '\*PELTS\*(index:68)' in room with player |
| Action| ActionID 52 ArgID 68| get item '*PELTS*(index:68)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 312 - Drop for item *PELTS* - Input: DROP PELT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 110| PELT |
| Condition| ConditionID 0 ArgID 68| item '\*PELTS\*(index:68)' carried |
| Action| ActionID 53 ArgID 68| drops item '*PELTS*(index:68)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 313 - Take for item *SILVER CUP* - Input: GET CUP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 111| CUP |
| Condition| ConditionID 1 ArgID 71| item '\*SILVER CUP\*(index:71)' in room with player |
| Action| ActionID 52 ArgID 71| get item '*SILVER CUP*(index:71)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 314 - Drop for item *SILVER CUP* - Input: DROP CUP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 111| CUP |
| Condition| ConditionID 0 ArgID 71| item '\*SILVER CUP\*(index:71)' carried |
| Action| ActionID 53 ArgID 71| drops item '*SILVER CUP*(index:71)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 315 - Take for item *BAG GOLD DUST* - Input: GET BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 112| BAG |
| Condition| ConditionID 1 ArgID 72| item '\*BAG GOLD DUST\*(index:72)' in room with player |
| Action| ActionID 52 ArgID 72| get item '*BAG GOLD DUST*(index:72)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 316 - Drop for item *BAG GOLD DUST* - Input: DROP BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 112| BAG |
| Condition| ConditionID 0 ArgID 72| item '\*BAG GOLD DUST\*(index:72)' carried |
| Action| ActionID 53 ArgID 72| drops item '*BAG GOLD DUST*(index:72)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 317 - Take for item Hammer - Input: GET HAMM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 114| HAMM |
| Condition| ConditionID 1 ArgID 73| item 'Hammer(index:73)' in room with player |
| Action| ActionID 52 ArgID 73| get item 'Hammer(index:73)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 318 - Drop for item Hammer - Input: DROP HAMM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 114| HAMM |
| Condition| ConditionID 0 ArgID 73| item 'Hammer(index:73)' carried |
| Action| ActionID 53 ArgID 73| drops item 'Hammer(index:73)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 319 - Take for item *SACRED TOM TOM* - Input: GET TOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 116| TOM |
| Condition| ConditionID 1 ArgID 76| item '\*SACRED TOM TOM\*(index:76)' in room with player |
| Action| ActionID 52 ArgID 76| get item '*SACRED TOM TOM*(index:76)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 320 - Drop for item *SACRED TOM TOM* - Input: DROP TOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 116| TOM |
| Condition| ConditionID 0 ArgID 76| item '\*SACRED TOM TOM\*(index:76)' carried |
| Action| ActionID 53 ArgID 76| drops item '*SACRED TOM TOM*(index:76)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 321 - Take for item *TURQUOISE NECKLACE* - Input: GET NECK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 118| NECK |
| Condition| ConditionID 1 ArgID 77| item '\*TURQUOISE NECKLACE\*(index:77)' in room with player |
| Action| ActionID 52 ArgID 77| get item '*TURQUOISE NECKLACE*(index:77)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 322 - Drop for item *TURQUOISE NECKLACE* - Input: DROP NECK
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DROP |
| Noun| 118| NECK |
| Condition| ConditionID 0 ArgID 77| item '\*TURQUOISE NECKLACE\*(index:77)' carried |
| Action| ActionID 53 ArgID 77| drops item '*TURQUOISE NECKLACE*(index:77)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 323 - Manually added load game action - Input: LOAD GAME
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 56| LOAD |
| Noun| 7| GAME |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUTO| 0|  |
| GO| 1| WALK, RUN, CLIM, ENTE, MOUN, RIDE |
| \.| 8|  |
| \.| 9|  |
| GET| 10| TAKE, PICK, GRAB, COLL, LIFT |
| \.| 16|  |
| \.| 17|  |
| DROP| 18| PUT, THRO, LEAV, REMO, TOSS |
| \.| 24|  |
| LOOK| 25| EXAM, DESC, CHEC |
| HELP| 29|  |
| SAVE| 30|  |
| QUIT| 31|  |
| SCOR| 32|  |
| SAY| 33| YELL, SCRE, WHIS, SING |
| DIG| 38| SHOV |
| MIX| 40| MAKE |
| \.| 42|  |
| SMEL| 43| TAST, EAT |
| BURN| 46| IGNI, LIGH |
| \.| 49|  |
| OPEN| 50| UNLO |
| LOCK| 52|  |
| \.| 53|  |
| CLOS| 54| SHUT |
| LOAD| 56|  |
| SHOO| 57|  |
| WITH| 58| USE |
| INVE| 60|  |
| HIT| 61| RING, BEAT |
| PLAY| 64|  |
| KILL| 65|  |
| CLAP| 66| APPL |
| READ| 68|  |
| UNLI| 69| EXTI |
| LIST| 71| HEAR |
| BREA| 73| SMAS, BUST |
| JUMP| 76| LEAP |
| CUT| 78| SLIC |
| SHAK| 80| WAVE |
| TAPE| 82|  |
| WEAR| 83| PUTO |
| FIND| 85| LOCA, SEEK |
| CROS| 88|  |
| SLEE| 89|  |
| CONN| 90| SPLI, REPA |
| MOVE| 93| PUSH, PRES, TAP |
| PASS| 97|  |
| WAIT| 98|  |
| CLEA| 99|  |
| COVE| 100|  |
| | 101|  |
| \.| 102|  |
| EMPT| 103| SPIL |
| DANC| 105|  |
| | 106|  |
| FILL| 107|  |
| | 108|  |
| | 109|  |
| SHOE| 110|  |
| KNOC| 111| TOUC, FEEL, KISS |
| SPUR| 115| KICK |
| | 117|  |
| | 118|  |
| | 119|  |
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
| GAME| 7|  |
| AROU| 8|  |
| STAB| 9|  |
| MANU| 10| PILE |
| HILL| 12|  |
| GUNP| 13|  |
| GRAV| 14|  |
| SULF| 15| POWD |
| CHAR| 17|  |
| MATC| 18|  |
| ON| 19|  |
| SAFE| 20|  |
| MIRR| 21|  |
| COMP| 22|  |
| HORS| 23| MAGN |
| BELL| 25|  |
| GHOS| 26| FIGU |
| HAND| 28| FEET |
| HEAD| 30|  |
| KEY| 31| KEYS |
| MAP| 33|  |
| CAND| 34| LIGH |
| MUSI| 36|  |
| BULL| 37|  |
| STAB| 38|  |
| DERR| 39| GUN |
| WIRE| 41|  |
| STOR| 42|  |
| JAIL| 43|  |
| ROOF| 44|  |
| SIGN| 45|  |
| BARB| 46|  |
| TUMB| 47| SAGE, BRUS |
| MINE| 50| ENTR |
| BED| 52|  |
| HOTE| 53|  |
| ROOM| 54|  |
| GIDD| 55| GITT, GIDY, GITY |
| COIN| 59|  |
| TOWN| 60|  |
| HOLE| 61|  |
| INVE| 62|  |
| STAL| 63|  |
| SALO| 64|  |
| DOOR| 65|  |
| WIND| 66|  |
| SPUR| 67|  |
| HAT| 68|  |
| STRI| 69|  |
| TAPE| 70| ROLL |
| WALL| 72|  |
| TELE| 73| OFFI |
| PAIN| 75|  |
| SLEE| 76|  |
| SNAK| 77| RATT |
| WORM| 79| SLIM |
| SHOV| 81|  |
| BOX| 82| CASH |
| ROAD| 84|  |
| FORK| 85|  |
| VAIN| 86|  |
| PIAN| 87|  |
| $200| 88|  |
| GO| 89| BOAR |
| PATH| 91|  |
| HELL| 92|  |
| HI| 93|  |
| FIEL| 94|  |
| CRYS| 95|  |
| GOLD| 96| NUGG |
| KEG| 98|  |
| NAIL| 99|  |
| FUSE| 100|  |
| TOPP| 101|  |
| LOBB| 102|  |
| RAVI| 103| RIDG |
| SHAC| 105|  |
| TRAI| 106|  |
| MOUN| 107|  |
| FLOO| 108|  |
| PLAN| 109|  |
| PELT| 110|  |
| CUP| 111|  |
| BAG| 112| DUST |
| HAMM| 114|  |
| TEEP| 115|  |
| TOM| 116|  |
| HOW| 117|  |
| NECK| 118|  |
| COUN| 119|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| Ghost Town| East: 17, West: 2 |
| 2| Ghost Town| East: 1, West: 3 |
| 3| Ghost Town| East: 2, West: 4 |
| 4| Ghost Town| East: 3, West: 6 |
| 5| stable| South: 4 |
| 6| road| East: 4, West: 7 |
| 7| fork in the road| North: 9, South: 8, East: 6 |
| 8| \*I'm on a ridge above a narrow ravine I see mountains in the distance| North: 7 |
| 9| large field| South: 7 |
| 10| ravine| Up: 8 |
| 11| saloon| South: 2 |
| 12| hidden office| East: 11 |
| 13| Jail| North: 1 |
| 14| cell| North: 13 |
| 15| Dry Goods store| North: 2 |
| 16| Barbershop| South: 1 |
| 17| road| East: 20, West: 1 |
| 18| \*I'm on a ridge above a ravine| West: 32 |
| 19| stall| South: 5 |
| 20| \*I'm on Boot hill| West: 17 |
| 21| Mine| Up: 10, Down: 22 |
| 22| Mine| South: 23, Up: 21 |
| 23| Mine| North: 22 |
| 24| Telegraph office| South: 3 |
| 25| \*I'm on back of 'Ole Paint| Down: 19 |
| 26| warm bed|  |
| 27| hotel room| West: 28 |
| 28| lobby| North: 3, East: 27 |
| 29| grave| Up: 20 |
| 30| \*I'm flat on my back in a manure pile|  |
| 31| storeroom| North: 19 |
| 32| mountain trail| East: 18 |
| 33| line shack| South: 32 |
| 34| root cellar| Up: 33 |
| 35| \*I'm behind the counter| North: 28 |
| 36| hidden canyon|  |
| 37| teepee| North: 36 |
| 38| lot of trouble\!|  |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| OK |
| 2| I see |
| 3| Welcome to Adventure 9 `GHOST TOWN` |
| 4| by Scott Adams dedicated: the Cherens |
| 5| I've nothing to do that with |
| 6| Sorry I can't |
| 7| I found |
| 8| Wear? |
| 9| BARF\! |
| 10| something |
| 11| nothing special |
| 12| reminds me of |
| 13| You've made |
| 14| BONUS points out of a possible 50 in |
| 15| its full of sage brush, tumbleweed & is impassable |
| 16| moves |
| 17| The dry wash is burnt clear |
| 18| flying glass slices me up |
| 19| Crack\! |
| 20| north |
| 21| its pointing to the |
| 22| horseshoe |
| 23| Doors closed, windows barred\! |
| 24| with what? |
| 25| Inside bolt is latched\! |
| 26| Magnet\! |
| 27|  doesn't seem to do it\! |
| 28| Ding\-Ding |
| 29| Bell rings somewhere |
| 30| My hand passes thru\! |
| 31| Ghost stands, bows, vanishes\! |
| 32| Silly, wrong type keys\! |
| 33| Odd |
| 34| goes thunk\! |
| 35| falls out |
| 36| Candle blew out\! |
| 37| very pretty |
| 38| shoots stream of water |
| 39| it already is |
| 40| Drop \*TREASURES\* then SCORE |
| 41| I hear |
| 42| What? |
| 43| Too steep\! |
| 44| feels strange |
| 45| its my size |
| 46| Don't collect $200 then don't pass GO\! CONTRAPOSITIVE\. |
| 47| happens |
| 48| How? |
| 49| Its mine, dig roof\! |
| 50| Ghostly voice whispers: |
| 51| Vain\.\.\. |
| 52| Match flares up\.\.\. |
| 53| \.\.\.and then goes out |
| 54| Its getting |
| 55| Sunset\! |
| 56| I feel refreshed |
| 57| Nights are cold\! I caught Pneumonia |
| 58| Try: SLEEP |
| 59| it worked\! |
| 60| its gone |
| 61| snake won't let me |
| 62| That felt good\! |
| 63| Too big\! |
| 64| its locked\! |
| 65| Good Morning |
| 66| Good night |
| 67| Its fireproof |
| 68| He won't budge |
| 69| left\! |
| 70| dark\! |
| 71| Thru the Hat\! |
| 72| I'm snake bit |
| 73| I'm not Alice\! |
| 74| He bucks, I'm thrown |
| 75| Whoosh\! |
| 76| TOO CLOSE\! Pieces of me rain down for days\! |
| 77| Boom\! |
| 78| \.\.\. \.\.\.\. \.\-  \-\.\-  \.  \- \-\-\-  \.\-\-\.  \.\-\-\.  \.  \.\-\. |
| 79| SPARK\! \* \* \* \* |
| 80| Click |
| 81| Is he a ghost? Anyway wrong idea\. |
| 82| There's not even a keyhole\! |
| 83| masking tape |
| 84| Floorboards sure are creaky |
| 85| Loose plank here |
| 86| salt peter |
| 87| I won a prize\! |
| 88| reach a nail |
| 89| may need to say a magic word here |
| 90| after a long ride |
| 91| he rides off without me |
| 92| Geronimo says: `Its easy\! Happy Landings\!` |
| 93| is missing |
| 94| rotten eggs |
| 95| \. |
| 96| in saloon |
| 97| scared them off\! |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Worn out fiddle strings| STRI| 0 |
| 1| Barbershop| | 1 |
| 2| Jail| | 1 |
| 3| Saloon| | 2 |
| 4| Stable| | 4 |
| 5| Stall| | 5 |
| 6| Manure pile| | 5 |
| 7| Shovel| SHOV| 15 |
| 8| White crystals| CRYS| 0 |
| 9| Lit candle| CAND| 0 |
| 10| Yellow powder| SULF| 0 |
| 11| Sagebrush charcoal| CHAR| 10 |
| 12| Pile of gunpowder| | 0 |
| 13| Entrance to a mine| | 10 |
| 14| Matches| MATC| 15 |
| 15| Mirror| | 11 |
| 16| 'ole Paint| | 19 |
| 17| Broken mirror| | 0 |
| 18| Hole in the wall| | 0 |
| 19| Compass| COMP| 15 |
| 20| Horseshoe| HORS| 19 |
| 21| Male cow manure| MANU| 0 |
| 22| Large bell| BELL| 11 |
| 23| Wraithlike figure playing equally ghostly piano| | 0 |
| 24| Piano with set of keys| | 0 |
| 25| Map| MAP| 0 |
| 26| Unlit candle| CAND| 22 |
| 27| \*SILVER BULLET\*| BULL| 21 |
| 28| \*GOLDEN DERRINGER\*| DERR| 13 |
| 29| Open door| | 0 |
| 30| Sign\-`Ring for ROOM service`| SIGN| 35 |
| 31| Locked door| | 13 |
| 32| Dry\-Goods store| | 2 |
| 33| Sign| SIGN| 15 |
| 34| \*SILVER SPURS\*| SPUR| 25 |
| 35| Stetson hat| HAT| 16 |
| 36| Which I'm wearing| | 0 |
| 37| Small key| KEY| 0 |
| 38| Roll of tape| TAPE| 0 |
| 39| Taped up mirror| | 0 |
| 40| \*GOLD NUGGET\*| GOLD| 0 |
| 41| Telegraph office| | 3 |
| 42| Empty matchbook| MATC| 0 |
| 43| Bed| | 0 |
| 44| Hotel| | 3 |
| 45| Rattlesnake| SNAK| 20 |
| 46| Open grave| | 0 |
| 47| \*GOLD COIN\*| COIN| 29 |
| 48| Purple worm| WORM| 29 |
| 49| Purple Slime| WORM| 0 |
| 50| Telegraph key| | 24 |
| 51| 2 loose wires| | 0 |
| 52| Spliced wire| | 0 |
| 53| Pieces of wire| WIRE| 0 |
| 54| Large safe| | 24 |
| 55| \*CASHBOX\*| BOX| 35 |
| 56| \* $200 \*| $200| 0 |
| 57| \*ORIENTAL GO BOARD\*| GO| 12 |
| 58| Hole kicked in wall & bare hoof print| | 0 |
| 59| Keg of nails| KEG| 31 |
| 60| Empty keg| KEG| 0 |
| 61| Keg of gunpowder| KEG| 0 |
| 62| Nails| NAIL| 0 |
| 63| Telegraph key| | 33 |
| 64| Smoking open safe| | 0 |
| 65| Line shack| | 32 |
| 66| Plank| PLAN| 0 |
| 67| Hole in floor| | 0 |
| 68| \*PELTS\*| PELT| 34 |
| 69| Counter| | 28 |
| 70| Ghostly square dance| | 0 |
| 71| \*SILVER CUP\*| CUP| 0 |
| 72| \*BAG GOLD DUST\*| BAG| 0 |
| 73| Hammer| HAMM| 14 |
| 74| TeePee| | 36 |
| 75| Indian ghost| | 0 |
| 76| \*SACRED TOM TOM\*| TOM| 37 |
| 77| \*TURQUOISE NECKLACE\*| NECK| 37 |