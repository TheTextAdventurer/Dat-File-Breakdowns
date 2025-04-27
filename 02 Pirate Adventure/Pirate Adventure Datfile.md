# Pirate Adventure Datfile
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
| adventureNumber| 2 |
| Unknown| 5724 |
| numItems| 67 |
| numActions| 178 |
| numNounVerbs| 80 |
| numRooms| 27 |
| maxCarry| 6 |
| startRoom| 1 |
| totalTreasures| 2 |
| wordLength| 3 |
| lightDuration| 150 |
| numMessages| 89 |
| treasureRoom| 1 |
## Actions
### Action 0 - CROCODILES - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 422, 342, 420, 340, 0, 16559, 8850|  |
| Probability| 80%|  |
| Condition| ConditionID 1 ArgID 21| item 'Fish(index:21)' in room with player |
| Condition| ConditionID 1 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' in room with player |
| Action| ActionID 110 | Print message 'Crocs eat fish and leave' |
| Action| ActionID 59 ArgID 21| Item 'Fish(index:21)' is removed from the game (put in room 0) |
| Action| ActionID 59 ArgID 17| Item 'Mean and hungry looking crocodiles(index:17)' is removed from the game (put in room 0) |
### Action 1 - SNAKES - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 462, 482, 460, 0, 0, 15712, 1705|  |
| Probability| 80%|  |
| Condition| ConditionID 1 ArgID 23| item 'Deadly mamba snakes(index:23)' in room with player |
| Condition| ConditionID 1 ArgID 24| item 'Parrot(index:24)' in room with player |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 112 | Print message '`Pieces of eight`' |
| Action| ActionID 11 | Print message 'Parrot attacks snakes and drives them off' |
| Action| ActionID 55 ArgID 23| Item 'Deadly mamba snakes(index:23)' is removed from the game (put in room 0) |
### Action 2 - RUG FLAG 11 GOT KEYS - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 521, 552, 540, 229, 220, 203, 8700|  |
| Probability| 100%|  |
| Condition| ConditionID 0 ArgID 26| item 'Rug(index:26)' carried |
| Condition| ConditionID 11 ArgID 27| item 'Ring of keys(index:27)' not carried or in room with player |
| Condition| ConditionID 8 ArgID 11| bitflag 11 is false |
| Action| ActionID 1 | Print message 'There's a strange sound' |
| Action| ActionID 53 ArgID 27| drops item 'Ring of keys(index:27)' into current room |
| Action| ActionID 58 ArgID 11| set 11 flag |
### Action 3 - PARROT PIECES 8 - Probability: 3 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3, 483, 0, 0, 0, 0, 15712, 0|  |
| Probability| 3%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 112 | Print message '`Pieces of eight`' |
### Action 4 - LITE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 284, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 5 - FLAG 1. BUILD BOAT. NEED SAIL/LUMBER/BEACH - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 663, 403, 40, 0, 8700, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Condition| ConditionID 2 ArgID 33| item 'Pile of precut lumber(index:33)' carried or in room with player |
| Condition| ConditionID 2 ArgID 20| item 'Pile of sails(index:20)' carried or in room with player |
| Action| ActionID 58 ArgID 2| set 2 flag |
### Action 6 - FLAG 2.READY TO BUILD BOAT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 48, 20, 660, 740, 220, 9055, 10902|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 55 ArgID 33| Item 'Pile of precut lumber(index:33)' is removed from the game (put in room 0) |
| Action| ActionID 72 ArgID 37, 11| swap item locations 'Pirate ship(index:37)' and 'Small ship's keel and mast(index:11)' |
| Action| ActionID 102 | Print message 'CONGRATULATIONS \!\!\! But your Adventure is not over yet\.\.\. ' |
### Action 7 - NOT READY TO BUILD - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 20, 0, 0, 0, 3810, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Action| ActionID 25 | Print message 'No, something is missing\!' |
| Action| ActionID 60 ArgID 1| set 1 flag |
### Action 8 - UNLOCK DOOR. FLAG 0 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 8, 700, 720, 0, 0, 10868, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 0| bitflag 0 is set |
| Action| ActionID 72 ArgID 35, 36| swap item locations 'Locked door(index:35)' and 'Open door with pit beyond(index:36)' |
| Action| ActionID 68 | Set bit 0 false |
### Action 9 - BUILDINg BOAT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 48, 40, 640, 400, 300, 9055, 8305|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Action| ActionID 60 ArgID 2| set 2 flag |
| Action| ActionID 55 ArgID 32| Item 'Nails(index:32)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 20| Item 'Pile of sails(index:20)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 15| Item 'Rusty anchor(index:15)' is removed from the game (put in room 0) |
### Action 10 - END GAME - Probability: 19 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 19, 524, 0, 0, 0, 0, 9778, 9450|  |
| Probability| 19%|  |
| Condition| ConditionID 3 ArgID 26| player in room 26 |
| Action| ActionID 65 | score |
| Action| ActionID 28 | Print message 'Since nothing is happening' |
| Action| ActionID 63 | game over |
### Action 11 - SLIPPED NO SHOES - Probability: 40 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 40, 104, 886, 0, 0, 0, 4411, 0|  |
| Probability| 40%|  |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 5 ArgID 44| item 'Safety sneakers(index:44)' not carried |
| Action| ActionID 29 | Print message 'I slipped and fell\.\.\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 12 - PIRATE RUM FLAG 0 - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 242, 502, 820, 80, 240, 9321, 10109|  |
| Probability| 80%|  |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Condition| ConditionID 1 ArgID 25| item 'Bottle of rum(index:25)' in room with player |
| Action| ActionID 62 ArgID 41, 4| item 'Sleeping pirate(index:41)' is moved to room 4 |
| Action| ActionID 21 | Print message 'Pirate grabs rum and scuttles off chortling' |
| Action| ActionID 67 | Set bit 0 true |
| Action| ActionID 59 ArgID 12| Item 'Wicked looking pirate(index:12)' is removed from the game (put in room 0) |
### Action 13 - PIRATE RUM ATTIC FLAG 0 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 8, 140, 80, 500, 0, 10262, 8850|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 0| bitflag 0 is set |
| Action| ActionID 68 | Set bit 0 false |
| Action| ActionID 62 ArgID 7, 4| item 'Empty bottle(index:7)' is moved to room 4 |
| Action| ActionID 59 ArgID 25| Item 'Bottle of rum(index:25)' is removed from the game (put in room 0) |
### Action 14 - FISH ESCAPE - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 421, 846, 420, 200, 0, 5162, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 0 ArgID 21| item 'Fish(index:21)' carried |
| Condition| ConditionID 5 ArgID 42| item 'Bottle of salt water(index:42)' not carried |
| Action| ActionID 34 | Print message 'Too dry, fish vanish\.' |
| Action| ActionID 62 ArgID 21, 10| item 'Fish(index:21)' is moved to room 10 |
### Action 15 - FLAG 6 INTRO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 129, 120, 0, 0, 0, 6508, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 6| bitflag 6 is false |
| Action| ActionID 43 | Print message '\* Welcome to Adventure number 2: `pirate adventure` by Alexis & Scott Adams, dedicated: Ted Heeren & Paul Sharland Remember you can always ask for `help`\. ' |
| Action| ActionID 58 ArgID 6| set 6 flag |
### Action 16 - PIRATE RUM AGAIN - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 242, 982, 820, 440, 240, 9321, 8850|  |
| Probability| 50%|  |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Condition| ConditionID 1 ArgID 49| item 'Bottles of rum(index:49)' in room with player |
| Action| ActionID 62 ArgID 41, 22| item 'Sleeping pirate(index:41)' is moved to room 22 |
| Action| ActionID 21 | Print message 'Pirate grabs rum and scuttles off chortling' |
| Action| ActionID 59 ArgID 12| Item 'Wicked looking pirate(index:12)' is removed from the game (put in room 0) |
### Action 17 - PARROT BAG - Probability: 35 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 35, 483, 69, 0, 0, 0, 15705, 0|  |
| Probability| 35%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 105 | Print message '`Check the bag matey`' |
### Action 18 - PARROT CHEST - Probability: 7 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7, 483, 249, 0, 0, 0, 15706, 0|  |
| Probability| 7%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 8 ArgID 12| bitflag 12 is false |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 106 | Print message '`Check the chest matey`' |
### Action 19 - TIDE IN DROWN - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 484, 1073, 1086, 0, 0, 17661, 9150|  |
| Probability| 50%|  |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Condition| ConditionID 12 ArgID 53| item 'The tide is coming in(index:53)' in game |
| Condition| ConditionID 5 ArgID 54| item 'Water wings(index:54)' not carried |
| Action| ActionID 117 | Print message 'The tide is coming in' |
| Action| ActionID 111 | Print message 'I'm underwater, I guess I don't swim well\. Blub Blub\.\.\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 20 - DROWN OCEAN - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 204, 1086, 0, 0, 0, 16711, 0|  |
| Probability| 50%|  |
| Condition| ConditionID 3 ArgID 10| player in room 10 |
| Condition| ConditionID 5 ArgID 54| item 'Water wings(index:54)' not carried |
| Action| ActionID 111 | Print message 'I'm underwater, I guess I don't swim well\. Blub Blub\.\.\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 21 - TIDE WITH ANCHOR - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 209, 1040, 1060, 300, 1100, 10872, 10050|  |
| Probability| 10%|  |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 72 ArgID 52, 53| swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)' |
| Action| ActionID 72 ArgID 15, 55| swap item locations 'Rusty anchor(index:15)' and 'Flotsam and jetsam(index:55)' |
| Action| ActionID 67 | Set bit 0 true |
### Action 22 - TIDE NO ANCHOR NOT T.I. - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 208, 1040, 1060, 89, 0, 10867, 0|  |
| Probability| 10%|  |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 72 ArgID 52, 53| swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)' |
| Action| ActionID 67 | Set bit 0 true |
### Action 23 - PARROT TIDE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 483, 8, 0, 0, 0, 15719, 10200|  |
| Probability| 100%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 7 ArgID 0| bitflag 0 is set |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 119 | Print message '`Tides be a changing matey`' |
| Action| ActionID 68 | Set bit 0 false |
### Action 24 - RESET FLAG 0 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 8, 0, 0, 0, 0, 10200, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 0| bitflag 0 is set |
| Action| ActionID 68 | Set bit 0 false |
### Action 25 - LITE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 104, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 26 - MONGOOSE - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 462, 282, 280, 1160, 0, 1422, 0|  |
| Probability| 80%|  |
| Condition| ConditionID 1 ArgID 23| item 'Deadly mamba snakes(index:23)' in room with player |
| Condition| ConditionID 1 ArgID 14| item 'Mongoose(index:14)' in room with player |
| Action| ActionID 9 | Print message 'I was wrong, I guess its not a mongoose cause the snakes bit it\!' |
| Action| ActionID 72 ArgID 14, 58| swap item locations 'Mongoose(index:14)' and 'Dead squirrel(index:58)' |
### Action 27 - BIRD & CROCS - Probability: 80 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 80, 342, 482, 480, 260, 0, 18725, 9300|  |
| Probability| 80%|  |
| Condition| ConditionID 1 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' in room with player |
| Condition| ConditionID 1 ArgID 24| item 'Parrot(index:24)' in room with player |
| Action| ActionID 124 | Print message 'Parrot attacks crocs but is beaten off' |
| Action| ActionID 125 | Print message 'Bird flys off looking very unhappy' |
| Action| ActionID 62 ArgID 24, 13| item 'Parrot(index:24)' is moved to room 13 |
### Action 28 - BIRD FOLLOWS CRACKERS - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 483, 1212, 252, 480, 1200, 18825, 0|  |
| Probability| 30%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 11 ArgID 60| item 'Sack of crackers(index:60)' not carried or in room with player |
| Condition| ConditionID 11 ArgID 12| item 'Wicked looking pirate(index:12)' not carried or in room with player |
| Action| ActionID 125 | Print message 'Bird flys off looking very unhappy' |
| Action| ActionID 75 ArgID 24, 60| put item 1 'Parrot(index:24)' with item2 'Sack of crackers(index:60)' |
### Action 29 - PARROT EAT CRACKS - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 483, 1203, 0, 0, 0, 18900, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 2 ArgID 60| item 'Sack of crackers(index:60)' carried or in room with player |
| Action| ActionID 126 | Print message 'Parrot ate a cracker\.' |
### Action 30 - PARROT BOOK - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 1234, 483, 63, 0, 0, 15733, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 13 ArgID 61| item 'Note(index:61)' not in game |
| Condition| ConditionID 2 ArgID 24| item 'Parrot(index:24)' carried or in room with player |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 133 | Print message '`Check the book, matey\!`' |
### Action 31 - BURNT LAMP - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 328, 1260, 180, 320, 0, 10860, 11400|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 16| bitflag 16 is set |
| Action| ActionID 72 ArgID 63, 9| swap item locations 'Burnt out torch(index:63)' and 'Lit torch(index:9)' |
| Action| ActionID 60 ArgID 16| set 16 flag |
| Action| ActionID 76 | look |
### Action 32 - Input: SAY YOH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1223, 107, 100, 61, 0, 0, 10507, 8164|  |
| Verb| 8| SAY |
| Noun| 23| YOH |
| Condition| ConditionID 6 ArgID 5| player not in room 5 |
| Condition| ConditionID 0 ArgID 3| item 'Large blood soaked book(index:3)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 7 | Print message 'Everything spins around and suddenly I'm elsewhere\.\.\.' |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 64 | look |
### Action 33 - NO SAIL WITH BOOK - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 242, 63, 903, 0, 2829, 0|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Condition| ConditionID 2 ArgID 45| item 'Map(index:45)' carried or in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 129 | Print message 'Pirate says: `First Yee be getting that ACCURSED thing off me ship\!` ' |
### Action 34 - Input: LIG TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5570, 163, 203, 160, 180, 0, 10870, 1264|  |
| Verb| 37| LIG |
| Noun| 20| TOR |
| Condition| ConditionID 2 ArgID 8| item 'Unlit torch(index:8)' carried or in room with player |
| Condition| ConditionID 2 ArgID 10| item 'Matches(index:10)' carried or in room with player |
| Action| ActionID 72 ArgID 8, 9| swap item locations 'Unlit torch(index:8)' and 'Lit torch(index:9)' |
| Action| ActionID 70 | clear screen |
| Action| ActionID 8 | Print message 'Torch is lit' |
| Action| ActionID 64 | look |
### Action 35 - Input: UNL TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6170, 183, 180, 160, 0, 0, 10914, 11400|  |
| Verb| 41| UNL |
| Noun| 20| TOR |
| Condition| ConditionID 2 ArgID 9| item 'Lit torch(index:9)' carried or in room with player |
| Action| ActionID 72 ArgID 9, 8| swap item locations 'Lit torch(index:9)' and 'Unlit torch(index:8)' |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 76 | look |
### Action 36 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 104, 0, 0, 0, 0, 900, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 6 | Print message 'I may need to say a MAGIC word here\!' |
### Action 37 - Input: GET DUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1529, 442, 465, 440, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 29| DUB |
| Condition| ConditionID 1 ArgID 22| item '\*DUBLEONS\*(index:22)' in room with player |
| Condition| ConditionID 4 ArgID 23| item 'Deadly mamba snakes(index:23)' not in room with player |
| Action| ActionID 52 ArgID 22| get item '*DUBLEONS*(index:22)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 38 - Input: GET DUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1529, 442, 462, 0, 0, 0, 760, 9150|  |
| Verb| 10| GET |
| Noun| 29| DUB |
| Condition| ConditionID 1 ArgID 22| item '\*DUBLEONS\*(index:22)' in room with player |
| Condition| ConditionID 1 ArgID 23| item 'Deadly mamba snakes(index:23)' in room with player |
| Action| ActionID 5 | Print message 'That's not very smart' |
| Action| ActionID 10 | Print message 'I'm snake bit' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 39 - Input: GO SHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 183, 322, 180, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 33| SHA |
| Condition| ConditionID 1 ArgID 16| item 'Grass shack(index:16)' in room with player |
| Action| ActionID 54 ArgID 9| move room 9 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 40 - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1538, 262, 242, 0, 0, 0, 1800, 0|  |
| Verb| 10| GET |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Action| ActionID 12 | Print message 'Pirate won't let me' |
### Action 41 - . - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1538, 262, 245, 260, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Condition| ConditionID 4 ArgID 12| item 'Wicked looking pirate(index:12)' not in room with player |
| Action| ActionID 52 ArgID 13| get item 'Treasure chest(index:13)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 42 - Input: OPE CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5888, 262, 242, 0, 0, 0, 1800, 0|  |
| Verb| 39| OPE |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Action| ActionID 12 | Print message 'Pirate won't let me' |
### Action 43 - Input: OPE CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5888, 262, 245, 0, 0, 0, 1950, 0|  |
| Verb| 39| OPE |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Condition| ConditionID 4 ArgID 12| item 'Wicked looking pirate(index:12)' not in room with player |
| Action| ActionID 13 | Print message 'Its locked' |
### Action 44 - Input: UNL CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6188, 262, 245, 541, 260, 560, 2155, 7950|  |
| Verb| 41| UNL |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Condition| ConditionID 4 ArgID 12| item 'Wicked looking pirate(index:12)' not in room with player |
| Condition| ConditionID 0 ArgID 27| item 'Ring of keys(index:27)' carried |
| Action| ActionID 14 | Print message 'Its open' |
| Action| ActionID 55 ArgID 13| Item 'Treasure chest(index:13)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 28| drops item 'Open treasure chest(index:28)' into current room |
### Action 45 - Input: OPE CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5888, 261, 0, 0, 0, 0, 2400, 0|  |
| Verb| 39| OPE |
| Noun| 38| CHE |
| Condition| ConditionID 0 ArgID 13| item 'Treasure chest(index:13)' carried |
| Action| ActionID 16 | Print message 'Not while I'm carrying it' |
### Action 46 - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4088, 561, 0, 0, 0, 0, 2400, 0|  |
| Verb| 27| LOO |
| Noun| 38| CHE |
| Condition| ConditionID 0 ArgID 28| item 'Open treasure chest(index:28)' carried |
| Action| ActionID 16 | Print message 'Not while I'm carrying it' |
### Action 47 - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4088, 263, 0, 0, 0, 0, 2713, 0|  |
| Verb| 27| LOO |
| Noun| 38| CHE |
| Condition| ConditionID 2 ArgID 13| item 'Treasure chest(index:13)' carried or in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 13 | Print message 'Its locked' |
### Action 48 - FLAG 12 CHEST EMPTY - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4088, 562, 580, 109, 100, 249, 2303, 8700|  |
| Verb| 27| LOO |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 28| item 'Open treasure chest(index:28)' in room with player |
| Condition| ConditionID 8 ArgID 5| bitflag 5 is false |
| Condition| ConditionID 8 ArgID 12| bitflag 12 is false |
| Action| ActionID 15 | Print message 'There are a set of plans in it' |
| Action| ActionID 53 ArgID 29| drops item 'Set of plans(index:29)' into current room |
| Action| ActionID 58 ArgID 5| set 5 flag |
### Action 49 - CHEST MAP - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4088, 249, 562, 108, 900, 240, 6203, 8700|  |
| Verb| 27| LOO |
| Noun| 38| CHE |
| Condition| ConditionID 8 ArgID 12| bitflag 12 is false |
| Condition| ConditionID 1 ArgID 28| item 'Open treasure chest(index:28)' in room with player |
| Condition| ConditionID 7 ArgID 5| bitflag 5 is set |
| Action| ActionID 41 | Print message 'There's a map in it' |
| Action| ActionID 53 ArgID 45| drops item 'Map(index:45)' into current room |
| Action| ActionID 58 ArgID 12| set 12 flag |
### Action 50 - EMPTY - Input: LOO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4088, 248, 562, 0, 0, 0, 6600, 0|  |
| Verb| 27| LOO |
| Noun| 38| CHE |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Condition| ConditionID 1 ArgID 28| item 'Open treasure chest(index:28)' in room with player |
| Action| ActionID 44 | Print message 'Its empty' |
### Action 51 - Input: LOO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4068, 103, 69, 0, 0, 0, 646, 0|  |
| Verb| 27| LOO |
| Noun| 18| BAG |
| Condition| ConditionID 2 ArgID 5| item 'Pirate's duffel bag(index:5)' carried or in room with player |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 46 | Print message 'open it?' |
### Action 52 - Input: LOO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4068, 103, 68, 0, 0, 0, 6600, 0|  |
| Verb| 27| LOO |
| Noun| 18| BAG |
| Condition| ConditionID 2 ArgID 5| item 'Pirate's duffel bag(index:5)' carried or in room with player |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 44 | Print message 'Its empty' |
### Action 53 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5887, 342, 0, 0, 0, 0, 2550, 0|  |
| Verb| 39| OPE |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' in room with player |
| Action| ActionID 17 | Print message 'Crocs stop me' |
### Action 54 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5887, 362, 0, 0, 0, 0, 2713, 0|  |
| Verb| 39| OPE |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 18| item 'Locked door(index:18)' in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 13 | Print message 'Its locked' |
### Action 55 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5887, 382, 0, 0, 0, 0, 2100, 0|  |
| Verb| 39| OPE |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 19| item 'Open door with hall beyond(index:19)' in room with player |
| Action| ActionID 14 | Print message 'Its open' |
### Action 56 - Input: GO HAL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 159, 382, 320, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 9| HAL |
| Condition| ConditionID 1 ArgID 19| item 'Open door with hall beyond(index:19)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 57 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6187, 342, 362, 0, 0, 0, 2550, 0|  |
| Verb| 41| UNL |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' in room with player |
| Condition| ConditionID 1 ArgID 18| item 'Locked door(index:18)' in room with player |
| Action| ActionID 17 | Print message 'Crocs stop me' |
### Action 58 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6187, 345, 362, 541, 360, 380, 8303, 10164|  |
| Verb| 41| UNL |
| Noun| 37| DOO |
| Condition| ConditionID 4 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' not in room with player |
| Condition| ConditionID 1 ArgID 18| item 'Locked door(index:18)' in room with player |
| Condition| ConditionID 0 ArgID 27| item 'Ring of keys(index:27)' carried |
| Action| ActionID 55 ArgID 18| Item 'Locked door(index:18)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 19| drops item 'Open door with hall beyond(index:19)' into current room |
| Action| ActionID 67 | Set bit 0 true |
| Action| ActionID 114 | Print message 'OK' |
### Action 59 - Input: DRI BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3461, 503, 0, 0, 0, 0, 19051, 3300|  |
| Verb| 23| DRI |
| Noun| 11| BOT |
| Condition| ConditionID 2 ArgID 25| item 'Bottle of rum(index:25)' carried or in room with player |
| Action| ActionID 127 | Print message 'Yummy' |
| Action| ActionID 1 | Print message 'There's a strange sound' |
| Action| ActionID 22 | Print message '\.\.\.I think its me, Hee Hee\.' |
### Action 60 - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 25| INV |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
### Action 61 - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1528, 0, 0, 0, 0, 0, 9900, 0|  |
| Verb| 10| GET |
| Noun| 28| INV |
| Action| ActionID 66 | output inventory |
### Action 62 - Input: LOO BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4108, 1143, 1012, 0, 0, 0, 646, 0|  |
| Verb| 27| LOO |
| Noun| 58| BOX |
| Condition| ConditionID 2 ArgID 57| item 'Wooden box(index:57)' carried or in room with player |
| Condition| ConditionID 11 ArgID 50| item '\*RARE STAMPS\*(index:50)' not carried or in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 46 | Print message 'open it?' |
### Action 63 - Input: SAY AWA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1271, 0, 0, 0, 0, 0, 2853, 0|  |
| Verb| 8| SAY |
| Noun| 71| AWA |
| Action| ActionID 19 | Print message 'Wrong game you silly goose\!' |
| Action| ActionID 3 | Print message 'Nothing happens' |
### Action 64 - Input: REA BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4510, 66, 0, 0, 0, 0, 2720, 0|  |
| Verb| 30| REA |
| Noun| 10| BOO |
| Condition| ConditionID 5 ArgID 3| item 'Large blood soaked book(index:3)' not carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 20 | Print message 'I don't have it' |
### Action 65 - Input: SCO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4950, 0, 0, 0, 0, 0, 9750, 0|  |
| Verb| 33| SCO |
| Noun| 0| ANY |
| Action| ActionID 65 | score |
### Action 66 - Input: SAV GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5114, 0, 0, 0, 0, 0, 10650, 0|  |
| Verb| 34| SAV |
| Noun| 14| GAM |
| Action| ActionID 71 | save game |
### Action 67 - . - Input: BUI BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7092, 592, 0, 0, 0, 0, 2745, 0|  |
| Verb| 47| BUI |
| Noun| 42| BOA |
| Condition| ConditionID 11 ArgID 29| item 'Set of plans(index:29)' not carried or in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 45 | Print message 'I've no plans\!' |
### Action 68 - Input: GO CAV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 185, 284, 140, 0, 0, 0, 8156, 10564|  |
| Verb| 1| GO |
| Noun| 35| CAV |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Action| ActionID 54 ArgID 7| move room 7 |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 69 - Input: LOO LAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4098, 1054, 0, 0, 0, 0, 647, 17550|  |
| Verb| 27| LOO |
| Noun| 48| LAG |
| Condition| ConditionID 13 ArgID 52| item 'The tide is out(index:52)' not in game |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
| Action| ActionID 117 | Print message 'The tide is coming in' |
### Action 70 - TIDE OUT - Input: LOO LAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4098, 1053, 0, 0, 0, 0, 647, 17400|  |
| Verb| 27| LOO |
| Noun| 48| LAG |
| Condition| ConditionID 12 ArgID 52| item 'The tide is out(index:52)' in game |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
| Action| ActionID 116 | Print message 'The tide is out' |
### Action 71 - Input: LOO SHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4083, 322, 0, 0, 0, 0, 647, 0|  |
| Verb| 27| LOO |
| Noun| 33| SHA |
| Condition| ConditionID 1 ArgID 16| item 'Grass shack(index:16)' in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
### Action 72 - Input: LOO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4095, 762, 0, 0, 0, 0, 647, 0|  |
| Verb| 27| LOO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 38| item 'Rock wall with narrow crack in it(index:38)' in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
### Action 73 - CARRYING SHOVEL - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 782, 921, 0, 0, 0, 2727, 0|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 39| item 'Narrow crack in the rock(index:39)' in room with player |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 27 | Print message 'Something won't fit' |
### Action 74 - CARRYING CHEST - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 762, 261, 0, 0, 0, 2727, 0|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 38| item 'Rock wall with narrow crack in it(index:38)' in room with player |
| Condition| ConditionID 0 ArgID 13| item 'Treasure chest(index:13)' carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 27 | Print message 'Something won't fit' |
### Action 75 - Input: QUI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 0, 0, 0, 0, 0, 9450, 0|  |
| Verb| 46| QUI |
| Noun| 0| ANY |
| Action| ActionID 63 | game over |
### Action 76 - Input: GET RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1526, 602, 0, 0, 0, 0, 2723, 0|  |
| Verb| 10| GET |
| Noun| 26| RUG |
| Condition| ConditionID 1 ArgID 30| item 'Rug(index:30)' in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 23 | Print message 'Its nailed to the floor\!' |
### Action 77 - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1541, 621, 602, 640, 520, 600, 7853, 8364|  |
| Verb| 10| GET |
| Noun| 41| NAI |
| Condition| ConditionID 0 ArgID 31| item 'Claw hammer(index:31)' carried |
| Condition| ConditionID 1 ArgID 30| item 'Rug(index:30)' in room with player |
| Action| ActionID 52 ArgID 32| get item 'Nails(index:32)', check if can carry |
| Action| ActionID 53 ArgID 26| drops item 'Rug(index:26)' into current room |
| Action| ActionID 55 ArgID 30| Item 'Rug(index:30)' is removed from the game (put in room 0) |
| Action| ActionID 114 | Print message 'OK' |
### Action 78 - CARRYING LUMBER - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 782, 661, 0, 0, 0, 2727, 0|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 39| item 'Narrow crack in the rock(index:39)' in room with player |
| Condition| ConditionID 0 ArgID 33| item 'Pile of precut lumber(index:33)' carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 27 | Print message 'Something won't fit' |
### Action 79 - Input: BUI BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7092, 623, 583, 303, 643, 20, 8700, 0|  |
| Verb| 47| BUI |
| Noun| 42| BOA |
| Condition| ConditionID 2 ArgID 31| item 'Claw hammer(index:31)' carried or in room with player |
| Condition| ConditionID 2 ArgID 29| item 'Set of plans(index:29)' carried or in room with player |
| Condition| ConditionID 2 ArgID 15| item 'Rusty anchor(index:15)' carried or in room with player |
| Condition| ConditionID 2 ArgID 32| item 'Nails(index:32)' carried or in room with player |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 80 - Input: BUI BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7092, 0, 0, 0, 0, 0, 3750, 0|  |
| Verb| 47| BUI |
| Noun| 42| BOA |
| Action| ActionID 25 | Print message 'No, something is missing\!' |
### Action 81 - Input: GO PIT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 200, 722, 220, 0, 0, 0, 10554, 9600|  |
| Verb| 1| GO |
| Noun| 50| PIT |
| Condition| ConditionID 1 ArgID 36| item 'Open door with pit beyond(index:36)' in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 54 ArgID 11| move room 11 |
| Action| ActionID 64 | look |
### Action 82 - CARRYING BOOK - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 762, 61, 0, 0, 0, 2727, 0|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 38| item 'Rock wall with narrow crack in it(index:38)' in room with player |
| Condition| ConditionID 0 ArgID 3| item 'Large blood soaked book(index:3)' carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 27 | Print message 'Something won't fit' |
### Action 83 - Input: SAY YOH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1223, 104, 120, 61, 0, 0, 10507, 8164|  |
| Verb| 8| SAY |
| Noun| 23| YOH |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 0 ArgID 3| item 'Large blood soaked book(index:3)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 7 | Print message 'Everything spins around and suddenly I'm elsewhere\.\.\.' |
| Action| ActionID 54 ArgID 6| move room 6 |
| Action| ActionID 64 | look |
### Action 84 - Input: GET RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1526, 523, 520, 0, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 26| RUG |
| Condition| ConditionID 2 ArgID 26| item 'Rug(index:26)' carried or in room with player |
| Action| ActionID 52 ArgID 26| get item 'Rug(index:26)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 85 - DARK - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 762, 340, 0, 0, 0, 8126, 8464|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 38| item 'Rock wall with narrow crack in it(index:38)' in room with player |
| Action| ActionID 54 ArgID 17| move room 17 |
| Action| ActionID 26 | Print message 'It was a tight squeeze\!' |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 64 | look |
### Action 86 - LITE - Input: GO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 195, 782, 360, 0, 0, 0, 8157, 10564|  |
| Verb| 1| GO |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 39| item 'Narrow crack in the rock(index:39)' in room with player |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 87 - WAIT FOR FOR TIDE - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 242, 1053, 89, 0, 17250, 0|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Condition| ConditionID 12 ArgID 52| item 'The tide is out(index:52)' in game |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 115 | Print message 'Pirate says: `Aye me Buckeroo, we be waiting for the tide to come in\!`' |
### Action 88 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 89 - FLAG 3 EMPTY BAG - Input: OPE BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5868, 103, 200, 69, 60, 0, 4553, 8700|  |
| Verb| 39| OPE |
| Noun| 18| BAG |
| Condition| ConditionID 2 ArgID 5| item 'Pirate's duffel bag(index:5)' carried or in room with player |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 30 | Print message 'Something falls out' |
| Action| ActionID 53 ArgID 10| drops item 'Matches(index:10)' into current room |
| Action| ActionID 58 ArgID 3| set 3 flag |
### Action 90 - Input: OPE BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5868, 68, 0, 0, 0, 0, 494, 0|  |
| Verb| 39| OPE |
| Noun| 18| BAG |
| Condition| ConditionID 7 ArgID 3| bitflag 3 is set |
| Action| ActionID 3 | Print message 'Nothing happens' |
| Action| ActionID 44 | Print message 'Its empty' |
### Action 91 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1546, 146, 0, 0, 0, 0, 4800, 0|  |
| Verb| 10| GET |
| Noun| 46| WAT |
| Condition| ConditionID 5 ArgID 7| item 'Empty bottle(index:7)' not carried |
| Action| ActionID 32 | Print message 'I've no container' |
### Action 92 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1546, 802, 141, 140, 840, 0, 8302, 17100|  |
| Verb| 10| GET |
| Noun| 46| WAT |
| Condition| ConditionID 1 ArgID 40| item 'Salt water(index:40)' in room with player |
| Condition| ConditionID 0 ArgID 7| item 'Empty bottle(index:7)' carried |
| Action| ActionID 55 ArgID 7| Item 'Empty bottle(index:7)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 42| get item 'Bottle of salt water(index:42)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 93 - Input: DRO WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2746, 841, 840, 140, 0, 0, 8302, 4950|  |
| Verb| 18| DRO |
| Noun| 46| WAT |
| Condition| ConditionID 0 ArgID 42| item 'Bottle of salt water(index:42)' carried |
| Action| ActionID 55 ArgID 42| Item 'Bottle of salt water(index:42)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 7| get item 'Empty bottle(index:7)', check if can carry |
| Action| ActionID 33 | Print message 'It soaks into the ground' |
### Action 94 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3496, 802, 0, 0, 0, 0, 811, 0|  |
| Verb| 23| DRI |
| Noun| 46| WAT |
| Condition| ConditionID 1 ArgID 40| item 'Salt water(index:40)' in room with player |
| Action| ActionID 5 | Print message 'That's not very smart' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 95 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3496, 841, 840, 140, 0, 0, 811, 8302|  |
| Verb| 23| DRI |
| Noun| 46| WAT |
| Condition| ConditionID 0 ArgID 42| item 'Bottle of salt water(index:42)' carried |
| Action| ActionID 5 | Print message 'That's not very smart' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
| Action| ActionID 55 ArgID 42| Item 'Bottle of salt water(index:42)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 7| get item 'Empty bottle(index:7)', check if can carry |
### Action 96 - Input: WAK PIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7366, 822, 820, 240, 400, 0, 5305, 9300|  |
| Verb| 49| WAK |
| Noun| 16| PIR |
| Condition| ConditionID 1 ArgID 41| item 'Sleeping pirate(index:41)' in room with player |
| Action| ActionID 35 | Print message 'Pirate awakens and says `Aye matey we be casting off soon` He then VANISHES\!' |
| Action| ActionID 55 ArgID 41| Item 'Sleeping pirate(index:41)' is removed from the game (put in room 0) |
| Action| ActionID 62 ArgID 12, 20| item 'Wicked looking pirate(index:12)' is moved to room 20 |
### Action 97 - Input: OPE BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5861, 503, 0, 0, 0, 0, 2100, 0|  |
| Verb| 39| OPE |
| Noun| 11| BOT |
| Condition| ConditionID 2 ArgID 25| item 'Bottle of rum(index:25)' carried or in room with player |
| Action| ActionID 14 | Print message 'Its open' |
### Action 98 - Input: EMP BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8411, 503, 500, 140, 0, 0, 5433, 10800|  |
| Verb| 56| EMP |
| Noun| 11| BOT |
| Condition| ConditionID 2 ArgID 25| item 'Bottle of rum(index:25)' carried or in room with player |
| Action| ActionID 36 | Print message 'What a waste\.\.\.' |
| Action| ActionID 33 | Print message 'It soaks into the ground' |
| Action| ActionID 72 ArgID 25, 7| swap item locations 'Bottle of rum(index:25)' and 'Empty bottle(index:7)' |
### Action 99 - Input: GO BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 192, 742, 400, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 42| BOA |
| Condition| ConditionID 1 ArgID 37| item 'Pirate ship(index:37)' in room with player |
| Action| ActionID 54 ArgID 20| move room 20 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 100 - FLAG 4 WE AT TREASUE ISLE - Input: GO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 201, 404, 88, 420, 240, 242, 8170, 8071|  |
| Verb| 1| GO |
| Noun| 51| SHO |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 7 ArgID 4| bitflag 4 is set |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 53 ArgID 12| drops item 'Wicked looking pirate(index:12)' into current room |
| Action| ActionID 121 | Print message 'Pirate follows me ashore as if expecting something' |
### Action 101 - Input: GO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 201, 404, 89, 120, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 51| SHO |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 54 ArgID 6| move room 6 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 102 - . - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 245, 0, 0, 0, 2737, 0|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 4 ArgID 12| item 'Wicked looking pirate(index:12)' not in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 37 | Print message 'I've no crew' |
### Action 103 - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 912, 0, 0, 0, 2738, 0|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 11 ArgID 45| item 'Map(index:45)' not carried or in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 38 | Print message 'Pirate says: `Aye matey we be needing a map first`\.' |
### Action 104 - GO TREASURE ISLE - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 89, 80, 740, 420, 10539, 8762|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 8 ArgID 4| bitflag 4 is false |
| Action| ActionID 70 | clear screen |
| Action| ActionID 39 | Print message 'After a day at sea we set anchor off of a sandy beach\. All Ashore who's going Ashore\.\.\.' |
| Action| ActionID 58 ArgID 4| set 4 flag |
| Action| ActionID 62 ArgID 37, 21| item 'Pirate ship(index:37)' is moved to room 21 |
### Action 105 - RETURN FROM TR ISLE - Input: SET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7530, 404, 88, 80, 740, 120, 10539, 9062|  |
| Verb| 50| SET |
| Noun| 30| SAI |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 7 ArgID 4| bitflag 4 is set |
| Action| ActionID 70 | clear screen |
| Action| ActionID 39 | Print message 'After a day at sea we set anchor off of a sandy beach\. All Ashore who's going Ashore\.\.\.' |
| Action| ActionID 60 ArgID 4| set 4 flag |
| Action| ActionID 62 ArgID 37, 6| item 'Pirate ship(index:37)' is moved to room 6 |
### Action 106 - Input: CAS OFF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7671, 0, 0, 0, 0, 0, 6000, 0|  |
| Verb| 51| CAS |
| Noun| 21| OFF |
| Action| ActionID 40 | Print message 'Try: `WEIGH ANCHOR`' |
### Action 107 - Input: REA MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4553, 903, 0, 0, 0, 0, 6300, 0|  |
| Verb| 30| REA |
| Noun| 53| MAP |
| Condition| ConditionID 2 ArgID 45| item 'Map(index:45)' carried or in room with player |
| Action| ActionID 42 | Print message 'Its a map to Treasure Island\. At the bottom it says: `30 paces then dig\!`' |
### Action 108 - Input: SAI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1350, 0, 0, 0, 0, 0, 6000, 0|  |
| Verb| 9| SAI |
| Noun| 0| ANY |
| Action| ActionID 40 | Print message 'Try: `WEIGH ANCHOR`' |
### Action 109 - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 62, 60, 0, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 10| BOO |
| Condition| ConditionID 1 ArgID 3| item 'Large blood soaked book(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Large blood soaked book(index:3)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 110 - Input: OPE BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5860, 63, 1254, 1240, 0, 0, 8064, 4500|  |
| Verb| 39| OPE |
| Noun| 10| BOO |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Condition| ConditionID 13 ArgID 62| item 'Small advertising flyer(index:62)' not in game |
| Action| ActionID 53 ArgID 62| drops item 'Small advertising flyer(index:62)' into current room |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 30 | Print message 'Something falls out' |
### Action 111 - AT T.I. - Input: GO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 201, 404, 88, 420, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 51| SHO |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 7 ArgID 4| bitflag 4 is set |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 112 - Input: GO PAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 218, 284, 360, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 68| PAT |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 113 - Input: GET PAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1539, 482, 242, 0, 0, 0, 1800, 0|  |
| Verb| 10| GET |
| Noun| 39| PAR |
| Condition| ConditionID 1 ArgID 24| item 'Parrot(index:24)' in room with player |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Action| ActionID 12 | Print message 'Pirate won't let me' |
### Action 114 - Input: GET PAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1539, 482, 480, 0, 0, 0, 7904, 16800|  |
| Verb| 10| GET |
| Noun| 39| PAR |
| Condition| ConditionID 1 ArgID 24| item 'Parrot(index:24)' in room with player |
| Action| ActionID 52 ArgID 24| get item 'Parrot(index:24)', check if can carry |
| Action| ActionID 104 | Print message 'The Parrot crys:' |
| Action| ActionID 112 | Print message '`Pieces of eight`' |
### Action 115 - Input: GO SHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 194, 682, 300, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 44| SHE |
| Condition| ConditionID 1 ArgID 34| item 'Tool shed(index:34)' in room with player |
| Action| ActionID 54 ArgID 15| move room 15 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 116 - FLAG 7. THIS IS IT - Input: GO 30
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 140, 464, 0, 0, 0, 8751, 0|  |
| Verb| 1| GO |
| Noun| 24| 30 |
| Condition| ConditionID 3 ArgID 23| player in room 23 |
| Action| ActionID 58 ArgID 7| set 7 flag |
| Action| ActionID 51 | Print message 'OK I walked off 30 paces\.' |
### Action 117 - PACE 30 BUT WRONG PLACE - Input: GO 30
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 174, 140, 0, 0, 0, 0, 9051, 0|  |
| Verb| 1| GO |
| Noun| 24| 30 |
| Action| ActionID 60 ArgID 7| set 7 flag |
| Action| ActionID 51 | Print message 'OK I walked off 30 paces\.' |
### Action 118 - BONES - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 444, 940, 921, 954, 0, 10548, 8014|  |
| Verb| 52| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Condition| ConditionID 13 ArgID 47| item 'Mouldy old bones(index:47)' not in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 48 | Print message 'I found something\!' |
| Action| ActionID 53 ArgID 47| drops item 'Mouldy old bones(index:47)' into current room |
| Action| ActionID 64 | look |
### Action 119 - EAT CRACKERRS - Input: DRI CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3495, 1203, 0, 0, 0, 0, 19050, 0|  |
| Verb| 23| DRI |
| Noun| 45| CRA |
| Condition| ConditionID 2 ArgID 60| item 'Sack of crackers(index:60)' carried or in room with player |
| Action| ActionID 127 | Print message 'Yummy' |
### Action 120 - BEACH TREASURE RUM - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 424, 994, 980, 921, 0, 10553, 7264|  |
| Verb| 52| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 13 ArgID 49| item 'Bottles of rum(index:49)' not in game |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Action| ActionID 70 | clear screen |
| Action| ActionID 53 ArgID 49| drops item 'Bottles of rum(index:49)' into current room |
| Action| ActionID 48 | Print message 'I found something\!' |
| Action| ActionID 64 | look |
### Action 121 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8250, 104, 0, 0, 0, 0, 10505, 9150|  |
| Verb| 55| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 5 | Print message 'That's not very smart' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 122 - GOT IT - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 464, 148, 1140, 921, 1154, 10553, 7264|  |
| Verb| 52| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 23| player in room 23 |
| Condition| ConditionID 7 ArgID 7| bitflag 7 is set |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Condition| ConditionID 13 ArgID 57| item 'Wooden box(index:57)' not in game |
| Action| ActionID 70 | clear screen |
| Action| ActionID 53 ArgID 57| drops item 'Wooden box(index:57)' into current room |
| Action| ActionID 48 | Print message 'I found something\!' |
| Action| ActionID 64 | look |
### Action 123 - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1541, 643, 640, 0, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 41| NAI |
| Condition| ConditionID 2 ArgID 32| item 'Nails(index:32)' carried or in room with player |
| Action| ActionID 52 ArgID 32| get item 'Nails(index:32)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 124 - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 163, 104, 40, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 13| WIN |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 54 ArgID 2| move room 2 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 125 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 44, 0, 0, 0, 0, 15456, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Action| ActionID 103 | Print message 'Reading expands the mind' |
| Action| ActionID 6 | Print message 'I may need to say a MAGIC word here\!' |
### Action 126 - Input: REA PLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4534, 583, 0, 0, 0, 0, 4650, 0|  |
| Verb| 30| REA |
| Noun| 34| PLA |
| Condition| ConditionID 2 ArgID 29| item 'Set of plans(index:29)' carried or in room with player |
| Action| ActionID 31 | Print message 'They're plans to build the Jolly Roger \(a Pirate ship\!\) You'll need: hammer, nails, lumber, anchor, sails, and a keel\.' |
### Action 127 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6187, 702, 541, 0, 0, 0, 2713, 16050|  |
| Verb| 41| UNL |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Locked door(index:35)' in room with player |
| Condition| ConditionID 0 ArgID 27| item 'Ring of keys(index:27)' carried |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 13 | Print message 'Its locked' |
| Action| ActionID 107 | Print message 'from the other side\!' |
### Action 128 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5887, 702, 0, 0, 0, 0, 2713, 0|  |
| Verb| 39| OPE |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 35| item 'Locked door(index:35)' in room with player |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 13 | Print message 'Its locked' |
### Action 129 - Input: OPE DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5887, 0, 722, 0, 0, 0, 2100, 0|  |
| Verb| 39| OPE |
| Noun| 37| DOO |
| Condition| ConditionID 1 ArgID 36| item 'Open door with pit beyond(index:36)' in room with player |
| Action| ActionID 14 | Print message 'Its open' |
### Action 130 - Input: GO LAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 198, 1022, 480, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 48| LAG |
| Condition| ConditionID 1 ArgID 51| item 'Lagoon(index:51)' in room with player |
| Action| ActionID 54 ArgID 24| move room 24 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 131 - Input: GO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 216, 2, 24, 40, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 66| STA |
| Condition| ConditionID 1 ArgID 0| item 'Flight of stairs(index:0)' in room with player |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 54 ArgID 2| move room 2 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 132 - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1510, 44, 60, 40, 80, 85, 7801, 10800|  |
| Verb| 10| GET |
| Noun| 10| BOO |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Condition| ConditionID 4 ArgID 4| item 'Bookcase with secret passage beyond(index:4)' not in room with player |
| Action| ActionID 52 ArgID 3| get item 'Large blood soaked book(index:3)', check if can carry |
| Action| ActionID 1 | Print message 'There's a strange sound' |
| Action| ActionID 72 ArgID 2, 4| swap item locations 'Books in a bookcase(index:2)' and 'Bookcase with secret passage beyond(index:4)' |
### Action 133 - Input: GET ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 302, 208, 300, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 32| ANC |
| Condition| ConditionID 1 ArgID 15| item 'Rusty anchor(index:15)' in room with player |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 52 ArgID 15| get item 'Rusty anchor(index:15)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 134 - Input: GET ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 302, 209, 0, 0, 0, 2813, 0|  |
| Verb| 10| GET |
| Noun| 32| ANC |
| Condition| ConditionID 1 ArgID 15| item 'Rusty anchor(index:15)' in room with player |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 113 | Print message 'Its stuck in the sand' |
### Action 135 - Input: GET ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 305, 0, 0, 0, 0, 10518, 7564|  |
| Verb| 10| GET |
| Noun| 32| ANC |
| Condition| ConditionID 4 ArgID 15| item 'Rusty anchor(index:15)' not in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 50 | Print message 'I don't see it here' |
| Action| ActionID 64 | look |
### Action 136 - DROP SALT WATER - Input: EMP BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8411, 843, 840, 140, 0, 0, 10914, 0|  |
| Verb| 56| EMP |
| Noun| 11| BOT |
| Condition| ConditionID 2 ArgID 42| item 'Bottle of salt water(index:42)' carried or in room with player |
| Action| ActionID 72 ArgID 42, 7| swap item locations 'Bottle of salt water(index:42)' and 'Empty bottle(index:7)' |
| Action| ActionID 114 | Print message 'OK' |
### Action 137 - Input: GO MON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 165, 1122, 500, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 15| MON |
| Condition| ConditionID 1 ArgID 56| item 'Monastary(index:56)' in room with player |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 138 - Input: SAI BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1392, 0, 0, 0, 0, 0, 6000, 0|  |
| Verb| 9| SAI |
| Noun| 42| BOA |
| Action| ActionID 40 | Print message 'Try: `WEIGH ANCHOR`' |
### Action 139 - . - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 284, 0, 0, 0, 0, 16350, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 14| player in room 14 |
| Action| ActionID 109 | Print message 'There's multiple exits here\!' |
### Action 140 - Input: WEI ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8582, 0, 0, 0, 0, 0, 17700, 0|  |
| Verb| 57| WEI |
| Noun| 32| ANC |
| Action| ActionID 118 | Print message 'About 20 pounds\. Try: `SET SAIL`' |
### Action 141 - FREE ANCHOR FLAG 10 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 921, 209, 302, 200, 0, 8814, 0|  |
| Verb| 52| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Condition| ConditionID 1 ArgID 15| item 'Rusty anchor(index:15)' in room with player |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 114 | Print message 'OK' |
### Action 142 - Input: BUR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 0, 0, 0, 0, 0, 2700, 0|  |
| Verb| 53| BUR |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
### Action 143 - Input: OPE BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5908, 621, 1143, 1000, 0, 0, 4553, 0|  |
| Verb| 39| OPE |
| Noun| 58| BOX |
| Condition| ConditionID 0 ArgID 31| item 'Claw hammer(index:31)' carried |
| Condition| ConditionID 2 ArgID 57| item 'Wooden box(index:57)' carried or in room with player |
| Action| ActionID 30 | Print message 'Something falls out' |
| Action| ActionID 53 ArgID 50| drops item '*RARE STAMPS*(index:50)' into current room |
### Action 144 - Input: KIL PIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5266, 0, 0, 0, 0, 0, 1800, 0|  |
| Verb| 35| KIL |
| Noun| 16| PIR |
| Action| ActionID 12 | Print message 'Pirate won't let me' |
### Action 145 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 342, 0, 0, 0, 0, 18450, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 17| item 'Mean and hungry looking crocodiles(index:17)' in room with player |
| Action| ActionID 123 | Print message 'Got anything to eat matey?' |
### Action 146 - Input: SAY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1200, 0, 0, 0, 0, 0, 17185, 450|  |
| Verb| 8| SAY |
| Noun| 0| ANY |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 85 | echo noun |
| Action| ActionID 3 | Print message 'Nothing happens' |
### Action 147 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 124, 0, 0, 0, 0, 16350, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 6| player in room 6 |
| Action| ActionID 109 | Print message 'There's multiple exits here\!' |
### Action 148 - Input: WAI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9450, 208, 1040, 1060, 0, 0, 10919, 0|  |
| Verb| 63| WAI |
| Noun| 0| ANY |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Action| ActionID 72 ArgID 52, 53| swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)' |
| Action| ActionID 119 | Print message '`Tides be a changing matey`' |
### Action 149 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 184, 242, 0, 0, 0, 3600, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Condition| ConditionID 1 ArgID 12| item 'Wicked looking pirate(index:12)' in room with player |
| Action| ActionID 24 | Print message 'Yoho ho and a \.\.\.' |
### Action 150 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 921, 140, 0, 0, 0, 7410, 0|  |
| Verb| 52| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Action| ActionID 49 | Print message 'I didn't find anything' |
| Action| ActionID 60 ArgID 7| set 7 flag |
### Action 151 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 24, 0, 0, 0, 0, 18300, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 122 | Print message 'Climb stairs\.\.\.' |
### Action 152 - Input: GO PAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 158, 82, 60, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 8| PAS |
| Condition| ConditionID 1 ArgID 4| item 'Bookcase with secret passage beyond(index:4)' in room with player |
| Action| ActionID 54 ArgID 3| move room 3 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 153 - Input: REA BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4510, 63, 0, 0, 0, 0, 300, 0|  |
| Verb| 30| REA |
| Noun| 10| BOO |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Action| ActionID 2 | Print message 'The book is in bad condtion but I can make out the title: `Treasure Island`\. There's a word written in blood in the flyleaf: `YOHO` and a message:  `Long John Silver left 2 treasures on Treasure Island`' |
### Action 154 - Input: DRI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3450, 0, 0, 0, 0, 0, 2700, 0|  |
| Verb| 23| DRI |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
### Action 155 - . - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6300, 0, 0, 0, 0, 0, 450, 0|  |
| Verb| 42| HEL |
| Noun| 0| ANY |
| Action| ActionID 3 | Print message 'Nothing happens' |
### Action 156 - Input: GO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 163, 22, 100, 0, 0, 0, 8170, 9600|  |
| Verb| 1| GO |
| Noun| 13| WIN |
| Condition| ConditionID 1 ArgID 1| item 'Open window(index:1)' in room with player |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 70 | clear screen |
| Action| ActionID 64 | look |
### Action 157 - Input: FIN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8100, 0, 0, 0, 0, 0, 2836, 0|  |
| Verb| 54| FIN |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 136 | Print message 'I don't know where to look\!' |
### Action 158 - Input: LIS ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4650, 0, 0, 0, 0, 0, 128, 0|  |
| Verb| 31| LIS |
| Noun| 0| ANY |
| Action| ActionID 128 | Print message 'I hear nothing now' |
### Action 159 - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1538, 563, 560, 0, 0, 0, 7914, 0|  |
| Verb| 10| GET |
| Noun| 38| CHE |
| Condition| ConditionID 2 ArgID 28| item 'Open treasure chest(index:28)' carried or in room with player |
| Action| ActionID 52 ArgID 28| get item 'Open treasure chest(index:28)', check if can carry |
| Action| ActionID 114 | Print message 'OK' |
### Action 160 - Input: OPE BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5860, 1253, 63, 1220, 1234, 0, 17153, 4500|  |
| Verb| 39| OPE |
| Noun| 10| BOO |
| Condition| ConditionID 12 ArgID 62| item 'Small advertising flyer(index:62)' in game |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Condition| ConditionID 13 ArgID 61| item 'Note(index:61)' not in game |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 53 ArgID 61| drops item 'Note(index:61)' into current room |
| Action| ActionID 30 | Print message 'Something falls out' |
### Action 161 - Input: LOO BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4060, 63, 0, 0, 0, 0, 730, 6900|  |
| Verb| 27| LOO |
| Noun| 10| BOO |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 130 | Print message 'read it?' |
| Action| ActionID 46 | Print message 'open it?' |
### Action 162 - Input: REA NOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4574, 1223, 0, 0, 0, 0, 18000, 0|  |
| Verb| 30| REA |
| Noun| 74| NOT |
| Condition| ConditionID 2 ArgID 61| item 'Note(index:61)' carried or in room with player |
| Action| ActionID 120 | Print message 'Note here says: `I be liking parrots, they be smart matey\!`' |
### Action 163 - Input: LOO MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4103, 903, 0, 0, 0, 0, 730, 0|  |
| Verb| 27| LOO |
| Noun| 53| MAP |
| Condition| ConditionID 2 ArgID 45| item 'Map(index:45)' carried or in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 130 | Print message 'read it?' |
### Action 164 - Input: REA FLY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4575, 1243, 0, 0, 0, 0, 10631, 0|  |
| Verb| 30| REA |
| Noun| 75| FLY |
| Condition| ConditionID 2 ArgID 62| item 'Small advertising flyer(index:62)' carried or in room with player |
| Action| ActionID 70 | clear screen |
| Action| ActionID 131 | Print message 'Ask for Adventure number 3: `MISSION IMPOSSIBLE` at your favorite computer dealer\. If they DON'T carry `ADVENTURE` have them call: 1\-305\-862\-6917  TODAY\! `ADVENTURE` also supports lower case\! ' |
### Action 165 - Input: OPE BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5860, 1233, 63, 0, 0, 0, 494, 0|  |
| Verb| 39| OPE |
| Noun| 10| BOO |
| Condition| ConditionID 12 ArgID 61| item 'Note(index:61)' in game |
| Condition| ConditionID 2 ArgID 3| item 'Large blood soaked book(index:3)' carried or in room with player |
| Action| ActionID 3 | Print message 'Nothing happens' |
| Action| ActionID 44 | Print message 'Its empty' |
### Action 166 - Input: LOO FLY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4125, 1243, 0, 0, 0, 0, 730, 0|  |
| Verb| 27| LOO |
| Noun| 75| FLY |
| Condition| ConditionID 2 ArgID 62| item 'Small advertising flyer(index:62)' carried or in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 130 | Print message 'read it?' |
### Action 167 - Input: FLY ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2550, 0, 0, 0, 0, 0, 2700, 0|  |
| Verb| 17| FLY |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
### Action 168 - Input: BRE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8850, 0, 0, 0, 0, 0, 2832, 0|  |
| Verb| 59| BRE |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 132 | Print message 'I'm not feeling destructive\!' |
### Action 169 - Input: LOO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4063, 22, 0, 0, 0, 0, 647, 0|  |
| Verb| 27| LOO |
| Noun| 13| WIN |
| Condition| ConditionID 1 ArgID 1| item 'Open window(index:1)' in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
### Action 170 - Input: LOO BOA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4092, 742, 0, 0, 0, 0, 647, 0|  |
| Verb| 27| LOO |
| Noun| 42| BOA |
| Condition| ConditionID 1 ArgID 37| item 'Pirate ship(index:37)' in room with player |
| Action| ActionID 4 | Print message 'There's something there all right\. Maybe I should' |
| Action| ActionID 47 | Print message 'go there?' |
### Action 171 - Input: FEE DES
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9676, 0, 0, 0, 0, 0, 20163, 0|  |
| Verb| 64| FEE |
| Noun| 76| DES |
| Action| ActionID 134 | Print message 'All right, POOF the GAME is destroyed\!' |
| Action| ActionID 63 | game over |
### Action 172 - Input: KIL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5250, 0, 0, 0, 0, 0, 2832, 0|  |
| Verb| 35| KIL |
| Noun| 0| ANY |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 132 | Print message 'I'm not feeling destructive\!' |
### Action 173 - Input: GET SNA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1578, 462, 0, 0, 0, 0, 760, 9150|  |
| Verb| 10| GET |
| Noun| 78| SNA |
| Condition| ConditionID 1 ArgID 23| item 'Deadly mamba snakes(index:23)' in room with player |
| Action| ActionID 5 | Print message 'That's not very smart' |
| Action| ActionID 10 | Print message 'I'm snake bit' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 174 - Input: CLO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10063, 0, 0, 0, 0, 0, 2837, 0|  |
| Verb| 67| CLO |
| Noun| 13| WIN |
| Action| ActionID 18 | Print message 'Sorry I can't' |
| Action| ActionID 137 | Print message 'Its stuck' |
### Action 175 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8250, 0, 0, 0, 0, 0, 17103, 0|  |
| Verb| 55| JUM |
| Noun| 0| ANY |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 3 | Print message 'Nothing happens' |
### Action 176 - Input: WAI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9450, 209, 1040, 1060, 300, 1100, 10872, 17100|  |
| Verb| 63| WAI |
| Noun| 0| ANY |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 72 ArgID 52, 53| swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)' |
| Action| ActionID 72 ArgID 15, 55| swap item locations 'Rusty anchor(index:15)' and 'Flotsam and jetsam(index:55)' |
| Action| ActionID 114 | Print message 'OK' |
### Action 177 - Input: LOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 0, 0, 0, 0, 0, 11514, 20250|  |
| Verb| 27| LOO |
| Noun| 0| ANY |
| Action| ActionID 76 | look |
| Action| ActionID 114 | Print message 'OK' |
| Action| ActionID 135 | Print message 'I see nothing special' |
### Action 179 - Take for item Large blood soaked book - Input: GET BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 10| BOO |
| Condition| ConditionID 1 ArgID 3| item 'Large blood soaked book(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Large blood soaked book(index:3)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 180 - Drop for item Large blood soaked book - Input: DRO BOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 10| BOO |
| Condition| ConditionID 0 ArgID 3| item 'Large blood soaked book(index:3)' carried |
| Action| ActionID 53 ArgID 3| drops item 'Large blood soaked book(index:3)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 181 - Take for item Pirate's duffel bag - Input: GET BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 18| BAG |
| Condition| ConditionID 1 ArgID 5| item 'Pirate's duffel bag(index:5)' in room with player |
| Action| ActionID 52 ArgID 5| get item 'Pirate's duffel bag(index:5)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 182 - Drop for item Pirate's duffel bag - Input: DRO BAG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 18| BAG |
| Condition| ConditionID 0 ArgID 5| item 'Pirate's duffel bag(index:5)' carried |
| Action| ActionID 53 ArgID 5| drops item 'Pirate's duffel bag(index:5)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 183 - Take for item Empty bottle - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 11| BOT |
| Condition| ConditionID 1 ArgID 7| item 'Empty bottle(index:7)' in room with player |
| Action| ActionID 52 ArgID 7| get item 'Empty bottle(index:7)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 184 - Drop for item Empty bottle - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 11| BOT |
| Condition| ConditionID 0 ArgID 7| item 'Empty bottle(index:7)' carried |
| Action| ActionID 53 ArgID 7| drops item 'Empty bottle(index:7)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 185 - Take for item Unlit torch - Input: GET TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 20| TOR |
| Condition| ConditionID 1 ArgID 8| item 'Unlit torch(index:8)' in room with player |
| Action| ActionID 52 ArgID 8| get item 'Unlit torch(index:8)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 186 - Drop for item Unlit torch - Input: DRO TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 20| TOR |
| Condition| ConditionID 0 ArgID 8| item 'Unlit torch(index:8)' carried |
| Action| ActionID 53 ArgID 8| drops item 'Unlit torch(index:8)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 187 - Take for item Lit torch - Input: GET TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 20| TOR |
| Condition| ConditionID 1 ArgID 9| item 'Lit torch(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Lit torch(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 188 - Drop for item Lit torch - Input: DRO TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 20| TOR |
| Condition| ConditionID 0 ArgID 9| item 'Lit torch(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Lit torch(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 189 - Take for item Matches - Input: GET MAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 22| MAT |
| Condition| ConditionID 1 ArgID 10| item 'Matches(index:10)' in room with player |
| Action| ActionID 52 ArgID 10| get item 'Matches(index:10)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 190 - Drop for item Matches - Input: DRO MAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 22| MAT |
| Condition| ConditionID 0 ArgID 10| item 'Matches(index:10)' carried |
| Action| ActionID 53 ArgID 10| drops item 'Matches(index:10)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 191 - Take for item Treasure chest - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 13| item 'Treasure chest(index:13)' in room with player |
| Action| ActionID 52 ArgID 13| get item 'Treasure chest(index:13)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 192 - Drop for item Treasure chest - Input: DRO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 38| CHE |
| Condition| ConditionID 0 ArgID 13| item 'Treasure chest(index:13)' carried |
| Action| ActionID 53 ArgID 13| drops item 'Treasure chest(index:13)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 193 - Take for item Mongoose - Input: GET MON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 15| MON |
| Condition| ConditionID 1 ArgID 14| item 'Mongoose(index:14)' in room with player |
| Action| ActionID 52 ArgID 14| get item 'Mongoose(index:14)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 194 - Drop for item Mongoose - Input: DRO MON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 15| MON |
| Condition| ConditionID 0 ArgID 14| item 'Mongoose(index:14)' carried |
| Action| ActionID 53 ArgID 14| drops item 'Mongoose(index:14)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 195 - Take for item Rusty anchor - Input: GET ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 32| ANC |
| Condition| ConditionID 1 ArgID 15| item 'Rusty anchor(index:15)' in room with player |
| Action| ActionID 52 ArgID 15| get item 'Rusty anchor(index:15)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 196 - Drop for item Rusty anchor - Input: DRO ANC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 32| ANC |
| Condition| ConditionID 0 ArgID 15| item 'Rusty anchor(index:15)' carried |
| Action| ActionID 53 ArgID 15| drops item 'Rusty anchor(index:15)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 197 - Take for item Pile of sails - Input: GET SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 30| SAI |
| Condition| ConditionID 1 ArgID 20| item 'Pile of sails(index:20)' in room with player |
| Action| ActionID 52 ArgID 20| get item 'Pile of sails(index:20)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 198 - Drop for item Pile of sails - Input: DRO SAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 30| SAI |
| Condition| ConditionID 0 ArgID 20| item 'Pile of sails(index:20)' carried |
| Action| ActionID 53 ArgID 20| drops item 'Pile of sails(index:20)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 199 - Take for item Fish - Input: GET FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 31| FIS |
| Condition| ConditionID 1 ArgID 21| item 'Fish(index:21)' in room with player |
| Action| ActionID 52 ArgID 21| get item 'Fish(index:21)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 200 - Drop for item Fish - Input: DRO FIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 31| FIS |
| Condition| ConditionID 0 ArgID 21| item 'Fish(index:21)' carried |
| Action| ActionID 53 ArgID 21| drops item 'Fish(index:21)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 201 - Take for item *DUBLEONS* - Input: GET DUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 29| DUB |
| Condition| ConditionID 1 ArgID 22| item '\*DUBLEONS\*(index:22)' in room with player |
| Action| ActionID 52 ArgID 22| get item '*DUBLEONS*(index:22)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 202 - Drop for item *DUBLEONS* - Input: DRO DUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 29| DUB |
| Condition| ConditionID 0 ArgID 22| item '\*DUBLEONS\*(index:22)' carried |
| Action| ActionID 53 ArgID 22| drops item '*DUBLEONS*(index:22)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 203 - Take for item Parrot - Input: GET PAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 39| PAR |
| Condition| ConditionID 1 ArgID 24| item 'Parrot(index:24)' in room with player |
| Action| ActionID 52 ArgID 24| get item 'Parrot(index:24)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 204 - Drop for item Parrot - Input: DRO PAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 39| PAR |
| Condition| ConditionID 0 ArgID 24| item 'Parrot(index:24)' carried |
| Action| ActionID 53 ArgID 24| drops item 'Parrot(index:24)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 205 - Take for item Bottle of rum - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 11| BOT |
| Condition| ConditionID 1 ArgID 25| item 'Bottle of rum(index:25)' in room with player |
| Action| ActionID 52 ArgID 25| get item 'Bottle of rum(index:25)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 206 - Drop for item Bottle of rum - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 11| BOT |
| Condition| ConditionID 0 ArgID 25| item 'Bottle of rum(index:25)' carried |
| Action| ActionID 53 ArgID 25| drops item 'Bottle of rum(index:25)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 207 - Take for item Rug - Input: GET RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 26| RUG |
| Condition| ConditionID 1 ArgID 26| item 'Rug(index:26)' in room with player |
| Action| ActionID 52 ArgID 26| get item 'Rug(index:26)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 208 - Drop for item Rug - Input: DRO RUG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 26| RUG |
| Condition| ConditionID 0 ArgID 26| item 'Rug(index:26)' carried |
| Action| ActionID 53 ArgID 26| drops item 'Rug(index:26)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 209 - Take for item Ring of keys - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 27| KEY |
| Condition| ConditionID 1 ArgID 27| item 'Ring of keys(index:27)' in room with player |
| Action| ActionID 52 ArgID 27| get item 'Ring of keys(index:27)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 210 - Drop for item Ring of keys - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 27| KEY |
| Condition| ConditionID 0 ArgID 27| item 'Ring of keys(index:27)' carried |
| Action| ActionID 53 ArgID 27| drops item 'Ring of keys(index:27)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 211 - Take for item Open treasure chest - Input: GET CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 38| CHE |
| Condition| ConditionID 1 ArgID 28| item 'Open treasure chest(index:28)' in room with player |
| Action| ActionID 52 ArgID 28| get item 'Open treasure chest(index:28)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 212 - Drop for item Open treasure chest - Input: DRO CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 38| CHE |
| Condition| ConditionID 0 ArgID 28| item 'Open treasure chest(index:28)' carried |
| Action| ActionID 53 ArgID 28| drops item 'Open treasure chest(index:28)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 213 - Take for item Set of plans - Input: GET PLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| PLA |
| Condition| ConditionID 1 ArgID 29| item 'Set of plans(index:29)' in room with player |
| Action| ActionID 52 ArgID 29| get item 'Set of plans(index:29)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 214 - Drop for item Set of plans - Input: DRO PLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 34| PLA |
| Condition| ConditionID 0 ArgID 29| item 'Set of plans(index:29)' carried |
| Action| ActionID 53 ArgID 29| drops item 'Set of plans(index:29)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 215 - Take for item Claw hammer - Input: GET HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 40| HAM |
| Condition| ConditionID 1 ArgID 31| item 'Claw hammer(index:31)' in room with player |
| Action| ActionID 52 ArgID 31| get item 'Claw hammer(index:31)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 216 - Drop for item Claw hammer - Input: DRO HAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 40| HAM |
| Condition| ConditionID 0 ArgID 31| item 'Claw hammer(index:31)' carried |
| Action| ActionID 53 ArgID 31| drops item 'Claw hammer(index:31)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 217 - Take for item Nails - Input: GET NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 41| NAI |
| Condition| ConditionID 1 ArgID 32| item 'Nails(index:32)' in room with player |
| Action| ActionID 52 ArgID 32| get item 'Nails(index:32)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 218 - Drop for item Nails - Input: DRO NAI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 41| NAI |
| Condition| ConditionID 0 ArgID 32| item 'Nails(index:32)' carried |
| Action| ActionID 53 ArgID 32| drops item 'Nails(index:32)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 219 - Take for item Pile of precut lumber - Input: GET LUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 25| LUM |
| Condition| ConditionID 1 ArgID 33| item 'Pile of precut lumber(index:33)' in room with player |
| Action| ActionID 52 ArgID 33| get item 'Pile of precut lumber(index:33)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 220 - Drop for item Pile of precut lumber - Input: DRO LUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 25| LUM |
| Condition| ConditionID 0 ArgID 33| item 'Pile of precut lumber(index:33)' carried |
| Action| ActionID 53 ArgID 33| drops item 'Pile of precut lumber(index:33)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 221 - Take for item Bottle of salt water - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 11| BOT |
| Condition| ConditionID 1 ArgID 42| item 'Bottle of salt water(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Bottle of salt water(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 222 - Drop for item Bottle of salt water - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 11| BOT |
| Condition| ConditionID 0 ArgID 42| item 'Bottle of salt water(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Bottle of salt water(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 223 - Take for item Safety sneakers - Input: GET SNE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 59| SNE |
| Condition| ConditionID 1 ArgID 44| item 'Safety sneakers(index:44)' in room with player |
| Action| ActionID 52 ArgID 44| get item 'Safety sneakers(index:44)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 224 - Drop for item Safety sneakers - Input: DRO SNE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 59| SNE |
| Condition| ConditionID 0 ArgID 44| item 'Safety sneakers(index:44)' carried |
| Action| ActionID 53 ArgID 44| drops item 'Safety sneakers(index:44)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 225 - Take for item Map - Input: GET MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 53| MAP |
| Condition| ConditionID 1 ArgID 45| item 'Map(index:45)' in room with player |
| Action| ActionID 52 ArgID 45| get item 'Map(index:45)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 226 - Drop for item Map - Input: DRO MAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 53| MAP |
| Condition| ConditionID 0 ArgID 45| item 'Map(index:45)' carried |
| Action| ActionID 53 ArgID 45| drops item 'Map(index:45)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 227 - Take for item Shovel - Input: GET SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 51| SHO |
| Condition| ConditionID 1 ArgID 46| item 'Shovel(index:46)' in room with player |
| Action| ActionID 52 ArgID 46| get item 'Shovel(index:46)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 228 - Drop for item Shovel - Input: DRO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 51| SHO |
| Condition| ConditionID 0 ArgID 46| item 'Shovel(index:46)' carried |
| Action| ActionID 53 ArgID 46| drops item 'Shovel(index:46)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 229 - Take for item Mouldy old bones - Input: GET BON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 55| BON |
| Condition| ConditionID 1 ArgID 47| item 'Mouldy old bones(index:47)' in room with player |
| Action| ActionID 52 ArgID 47| get item 'Mouldy old bones(index:47)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 230 - Drop for item Mouldy old bones - Input: DRO BON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 55| BON |
| Condition| ConditionID 0 ArgID 47| item 'Mouldy old bones(index:47)' carried |
| Action| ActionID 53 ArgID 47| drops item 'Mouldy old bones(index:47)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 231 - Take for item Sand - Input: GET SAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 57| SAN |
| Condition| ConditionID 1 ArgID 48| item 'Sand(index:48)' in room with player |
| Action| ActionID 52 ArgID 48| get item 'Sand(index:48)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 232 - Drop for item Sand - Input: DRO SAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 57| SAN |
| Condition| ConditionID 0 ArgID 48| item 'Sand(index:48)' carried |
| Action| ActionID 53 ArgID 48| drops item 'Sand(index:48)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 233 - Take for item Bottles of rum - Input: GET BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 11| BOT |
| Condition| ConditionID 1 ArgID 49| item 'Bottles of rum(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item 'Bottles of rum(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 234 - Drop for item Bottles of rum - Input: DRO BOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 11| BOT |
| Condition| ConditionID 0 ArgID 49| item 'Bottles of rum(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item 'Bottles of rum(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 235 - Take for item *RARE STAMPS* - Input: GET STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 66| STA |
| Condition| ConditionID 1 ArgID 50| item '\*RARE STAMPS\*(index:50)' in room with player |
| Action| ActionID 52 ArgID 50| get item '*RARE STAMPS*(index:50)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 236 - Drop for item *RARE STAMPS* - Input: DRO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 66| STA |
| Condition| ConditionID 0 ArgID 50| item '\*RARE STAMPS\*(index:50)' carried |
| Action| ActionID 53 ArgID 50| drops item '*RARE STAMPS*(index:50)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 237 - Take for item Water wings - Input: GET WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 13| WIN |
| Condition| ConditionID 1 ArgID 54| item 'Water wings(index:54)' in room with player |
| Action| ActionID 52 ArgID 54| get item 'Water wings(index:54)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 238 - Drop for item Water wings - Input: DRO WIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 13| WIN |
| Condition| ConditionID 0 ArgID 54| item 'Water wings(index:54)' carried |
| Action| ActionID 53 ArgID 54| drops item 'Water wings(index:54)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 239 - Take for item Wooden box - Input: GET BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 58| BOX |
| Condition| ConditionID 1 ArgID 57| item 'Wooden box(index:57)' in room with player |
| Action| ActionID 52 ArgID 57| get item 'Wooden box(index:57)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 240 - Drop for item Wooden box - Input: DRO BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 58| BOX |
| Condition| ConditionID 0 ArgID 57| item 'Wooden box(index:57)' carried |
| Action| ActionID 53 ArgID 57| drops item 'Wooden box(index:57)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 241 - Take for item Sack of crackers - Input: GET CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 45| CRA |
| Condition| ConditionID 1 ArgID 60| item 'Sack of crackers(index:60)' in room with player |
| Action| ActionID 52 ArgID 60| get item 'Sack of crackers(index:60)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 242 - Drop for item Sack of crackers - Input: DRO CRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 45| CRA |
| Condition| ConditionID 0 ArgID 60| item 'Sack of crackers(index:60)' carried |
| Action| ActionID 53 ArgID 60| drops item 'Sack of crackers(index:60)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 243 - Take for item Note - Input: GET NOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 74| NOT |
| Condition| ConditionID 1 ArgID 61| item 'Note(index:61)' in room with player |
| Action| ActionID 52 ArgID 61| get item 'Note(index:61)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 244 - Drop for item Note - Input: DRO NOT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 74| NOT |
| Condition| ConditionID 0 ArgID 61| item 'Note(index:61)' carried |
| Action| ActionID 53 ArgID 61| drops item 'Note(index:61)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 245 - Take for item Small advertising flyer - Input: GET FLY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 75| FLY |
| Condition| ConditionID 1 ArgID 62| item 'Small advertising flyer(index:62)' in room with player |
| Action| ActionID 52 ArgID 62| get item 'Small advertising flyer(index:62)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 246 - Drop for item Small advertising flyer - Input: DRO FLY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 75| FLY |
| Condition| ConditionID 0 ArgID 62| item 'Small advertising flyer(index:62)' carried |
| Action| ActionID 53 ArgID 62| drops item 'Small advertising flyer(index:62)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 247 - Take for item Burnt out torch - Input: GET TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 20| TOR |
| Condition| ConditionID 1 ArgID 63| item 'Burnt out torch(index:63)' in room with player |
| Action| ActionID 52 ArgID 63| get item 'Burnt out torch(index:63)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 248 - Drop for item Burnt out torch - Input: DRO TOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 20| TOR |
| Condition| ConditionID 0 ArgID 63| item 'Burnt out torch(index:63)' carried |
| Action| ActionID 53 ArgID 63| drops item 'Burnt out torch(index:63)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 249 - Manually added load game action - Input: LOA GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 82| LOA |
| Noun| 14| GAM |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUT| 0|  |
| GO| 1| CLI, WAL, RUN, ENT, PAC, FOL |
| SAY| 8|  |
| SAI| 9|  |
| GET| 10| TAK, CAT, PIC, REM, WEA, PUL |
| FLY| 17|  |
| DRO| 18| REL, THR, LEA, GIV |
| DRI| 23| EAT |
| INV| 25|  |
| SAI| 26|  |
| LOO| 27| EXA, WAT |
| REA| 30|  |
| LIS| 31|  |
| \.| 32|  |
| SCO| 33|  |
| SAV| 34|  |
| KIL| 35| ATT |
| LIG| 37|  |
| \.| 38|  |
| OPE| 39| SHA |
| UNL| 41|  |
| HEL| 42|  |
| \.| 43|  |
| \.| 44|  |
| SWI| 45|  |
| QUI| 46|  |
| BUI| 47| MAK |
| WAK| 49|  |
| SET| 50|  |
| CAS| 51|  |
| DIG| 52|  |
| BUR| 53|  |
| FIN| 54|  |
| JUM| 55|  |
| EMP| 56|  |
| WEI| 57|  |
| | 58|  |
| BRE| 59| SMA |
| \.| 61|  |
| | 62|  |
| WAI| 63|  |
| FEE| 64|  |
| | 65|  |
| | 66|  |
| CLO| 67| SHU |
| | 69|  |
| | 70|  |
| | 71|  |
| | 72|  |
| | 73|  |
| | 74|  |
| | 75|  |
| | 76|  |
| | 77|  |
| | 78|  |
| | 79|  |
| LOA| 82|  |
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
| \.| 7|  |
| PAS| 8|  |
| HAL| 9|  |
| BOO| 10|  |
| BOT| 11| RUM |
| WIN| 13|  |
| GAM| 14|  |
| MON| 15|  |
| PIR| 16|  |
| ARO| 17|  |
| BAG| 18| DUF |
| TOR| 20|  |
| OFF| 21|  |
| MAT| 22|  |
| YOH| 23|  |
| 30| 24|  |
| LUM| 25|  |
| RUG| 26|  |
| KEY| 27|  |
| INV| 28|  |
| DUB| 29|  |
| SAI| 30|  |
| FIS| 31|  |
| ANC| 32|  |
| SHA| 33|  |
| PLA| 34|  |
| CAV| 35|  |
| SIG| 36|  |
| DOO| 37|  |
| CHE| 38|  |
| PAR| 39|  |
| HAM| 40|  |
| NAI| 41|  |
| BOA| 42| SHI |
| SHE| 44|  |
| CRA| 45|  |
| WAT| 46| SAL |
| LAG| 48| TID |
| PIT| 50|  |
| SHO| 51| BEA |
| MAP| 53|  |
| PAC| 54|  |
| BON| 55|  |
| HOL| 56|  |
| SAN| 57|  |
| BOX| 58|  |
| SNE| 59|  |
| CRA| 60| SAC |
| PIE| 62|  |
| KEE| 63|  |
| FLO| 64| JET |
| STA| 66| UPS |
| PAT| 68| HIL |
| YOH| 70|  |
| AWA| 71| BUN |
| PIE| 73|  |
| NOT| 74|  |
| FLY| 75|  |
| DES| 76|  |
| CRO| 77|  |
| SNA| 78|  |
| TRE| 79|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| Flat in london|  |
| 2| alcove| Down: 1 |
| 3| secret passageway| East: 4, West: 2 |
| 4| musty attic| West: 3 |
| 5| \*I'M outside an open window on the ledge of a very tall building|  |
| 6| sandy beach on a tropical isle| East: 8 |
| 7| maze of caves| South: 12, East: 13, West: 14, Down: 11 |
| 8| meadow| East: 14, West: 6 |
| 9| grass shack| West: 8 |
| 10| \*I'm in the ocean| North: 10, South: 24, East: 10, West: 10 |
| 11| pit| Up: 7 |
| 12| maze of caves| North: 7, East: 14, West: 13 |
| 13| maze of caves| North: 7, South: 14, East: 12, West: 19 |
| 14| \*I'm at the foot of a cave ridden hill, a pathway leads on up to the top| West: 8 |
| 15| tool shed| North: 17 |
| 16| long hallway| East: 17 |
| 17| large cavern| West: 16 |
| 18| \*I'm on top of a hill\. Below is Pirates Island\. Across the sea way off in the distance I see Treasure Island| Down: 14 |
| 19| maze of caves| South: 14, East: 14, West: 13 |
| 20| \*I'm aboard Pirate ship anchored off shore|  |
| 21| \*I'm on the beach at \*Treasure\* Island| South: 22 |
| 22| spooky old graveyard filled with piles of empty and broken rum bottles| North: 21, East: 23 |
| 23| large barren field| West: 22 |
| 24| shallow lagoon\. to the north is the ocean| North: 10, South: 6, East: 6, West: 6 |
| 25| sacked and deserted monastary| West: 23 |
| 26| \*Welcome to Never Never Land|  |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| There's a strange sound |
| 2| The book is in bad condtion but I can make out the title: `Treasure Island`\. There's a word written in blood in the flyleaf: `YOHO` and a message:  `Long John Silver left 2 treasures on Treasure Island` |
| 3| Nothing happens |
| 4| There's something there all right\. Maybe I should |
| 5| That's not very smart |
| 6| I may need to say a MAGIC word here\! |
| 7| Everything spins around and suddenly I'm elsewhere\.\.\. |
| 8| Torch is lit |
| 9| I was wrong, I guess its not a mongoose cause the snakes bit it\! |
| 10| I'm snake bit |
| 11| Parrot attacks snakes and drives them off |
| 12| Pirate won't let me |
| 13| Its locked |
| 14| Its open |
| 15| There are a set of plans in it |
| 16| Not while I'm carrying it |
| 17| Crocs stop me |
| 18| Sorry I can't |
| 19| Wrong game you silly goose\! |
| 20| I don't have it |
| 21| Pirate grabs rum and scuttles off chortling |
| 22| \.\.\.I think its me, Hee Hee\. |
| 23| Its nailed to the floor\! |
| 24| Yoho ho and a \.\.\. |
| 25| No, something is missing\! |
| 26| It was a tight squeeze\! |
| 27| Something won't fit |
| 28| Since nothing is happening |
| 29| I slipped and fell\.\.\. |
| 30| Something falls out |
| 31| They're plans to build the Jolly Roger \(a Pirate ship\!\) You'll need: hammer, nails, lumber, anchor, sails, and a keel\. |
| 32| I've no container |
| 33| It soaks into the ground |
| 34| Too dry, fish vanish\. |
| 35| Pirate awakens and says `Aye matey we be casting off soon` He then VANISHES\! |
| 36| What a waste\.\.\. |
| 37| I've no crew |
| 38| Pirate says: `Aye matey we be needing a map first`\. |
| 39| After a day at sea we set anchor off of a sandy beach\. All Ashore who's going Ashore\.\.\. |
| 40| Try: `WEIGH ANCHOR` |
| 41| There's a map in it |
| 42| Its a map to Treasure Island\. At the bottom it says: `30 paces then dig\!` |
| 43| \* Welcome to Adventure number 2: `pirate adventure` by Alexis & Scott Adams, dedicated: Ted Heeren & Paul Sharland Remember you can always ask for `help`\.  |
| 44| Its empty |
| 45| I've no plans\! |
| 46| open it? |
| 47| go there? |
| 48| I found something\! |
| 49| I didn't find anything |
| 50| I don't see it here |
| 51| OK I walked off 30 paces\. |
| 52| CONGRATULATIONS \!\!\! But your Adventure is not over yet\.\.\.  |
| 53| Reading expands the mind |
| 54| The Parrot crys: |
| 55| `Check the bag matey` |
| 56| `Check the chest matey` |
| 57| from the other side\! |
| 58| Open the book\! |
| 59| There's multiple exits here\! |
| 60| Crocs eat fish and leave |
| 61| I'm underwater, I guess I don't swim well\. Blub Blub\.\.\. |
| 62| `Pieces of eight` |
| 63| Its stuck in the sand |
| 64| OK |
| 65| Pirate says: `Aye me Buckeroo, we be waiting for the tide to come in\!` |
| 66| The tide is out |
| 67| The tide is coming in |
| 68| About 20 pounds\. Try: `SET SAIL` |
| 69| `Tides be a changing matey` |
| 70| Note here says: `I be liking parrots, they be smart matey\!` |
| 71| Pirate follows me ashore as if expecting something |
| 72| Climb stairs\.\.\. |
| 73| Got anything to eat matey? |
| 74| Parrot attacks crocs but is beaten off |
| 75| Bird flys off looking very unhappy |
| 76| Parrot ate a cracker\. |
| 77| Yummy |
| 78| I hear nothing now |
| 79| Pirate says: `First Yee be getting that ACCURSED thing off me ship\!`  |
| 80| read it? |
| 81| Ask for Adventure number 3: `MISSION IMPOSSIBLE` at your favorite computer dealer\. If they DON'T carry `ADVENTURE` have them call: 1\-305\-862\-6917  TODAY\! `ADVENTURE` also supports lower case\!  |
| 82| I'm not feeling destructive\! |
| 83| `Check the book, matey\!` |
| 84| All right, POOF the GAME is destroyed\! |
| 85| I see nothing special |
| 86| I don't know where to look\! |
| 87| Its stuck |
| 88|  |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| Flight of stairs| | 1 |
| 1| Open window| | 2 |
| 2| Books in a bookcase| | 2 |
| 3| Large blood soaked book| BOO| 0 |
| 4| Bookcase with secret passage beyond| | 0 |
| 5| Pirate's duffel bag| BAG| 4 |
| 6| Sign says: `Bring \*TREASURES\* here, say: SCORE`| | 1 |
| 7| Empty bottle| BOT| 0 |
| 8| Unlit torch| TOR| 4 |
| 9| Lit torch| TOR| 0 |
| 10| Matches| MAT| 0 |
| 11| Small ship's keel and mast| | 6 |
| 12| Wicked looking pirate| | 9 |
| 13| Treasure chest| CHE| 9 |
| 14| Mongoose| MON| 8 |
| 15| Rusty anchor| ANC| 24 |
| 16| Grass shack| | 8 |
| 17| Mean and hungry looking crocodiles| | 11 |
| 18| Locked door| | 11 |
| 19| Open door with hall beyond| | 0 |
| 20| Pile of sails| SAI| 17 |
| 21| Fish| FIS| 10 |
| 22| \*DUBLEONS\*| DUB| 25 |
| 23| Deadly mamba snakes| | 25 |
| 24| Parrot| PAR| 9 |
| 25| Bottle of rum| BOT| 1 |
| 26| Rug| RUG| 0 |
| 27| Ring of keys| KEY| 0 |
| 28| Open treasure chest| CHE| 0 |
| 29| Set of plans| PLA| 0 |
| 30| Rug| | 1 |
| 31| Claw hammer| HAM| 15 |
| 32| Nails| NAI| 0 |
| 33| Pile of precut lumber| LUM| 17 |
| 34| Tool shed| | 17 |
| 35| Locked door| | 16 |
| 36| Open door with pit beyond| | 0 |
| 37| Pirate ship| | 0 |
| 38| Rock wall with narrow crack in it| | 18 |
| 39| Narrow crack in the rock| | 17 |
| 40| Salt water| | 10 |
| 41| Sleeping pirate| | 0 |
| 42| Bottle of salt water| BOT| 0 |
| 43| Rum bottle smashed into pieces\. Sign `Opposite of LIGHT is Unlight`| | 4 |
| 44| Safety sneakers| SNE| 1 |
| 45| Map| MAP| 0 |
| 46| Shovel| SHO| 15 |
| 47| Mouldy old bones| BON| 0 |
| 48| Sand| SAN| 6 |
| 49| Bottles of rum| BOT| 0 |
| 50| \*RARE STAMPS\*| STA| 0 |
| 51| Lagoon| | 6 |
| 52| The tide is out| | 24 |
| 53| The tide is coming in| | 0 |
| 54| Water wings| WIN| 15 |
| 55| Flotsam and jetsam| | 0 |
| 56| Monastary| | 23 |
| 57| Wooden box| BOX| 0 |
| 58| Dead squirrel| | 0 |
| 59| Sign in the sand says: `Welcome to Pirates Island, watch out for the tide\!`| | 6 |
| 60| Sack of crackers| CRA| 1 |
| 61| Note| NOT| 0 |
| 62| Small advertising flyer| FLY| 0 |
| 63| Burnt out torch| TOR| 0 |
| 64| | | 0 |
| 65| | | 0 |
| 66| | | 0 |