# Pyramid of Doom Datfile
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
| adventureNumber| 8 |
| Unknown| 4877 |
| numItems| 101 |
| numActions| 230 |
| numNounVerbs| 85 |
| numRooms| 28 |
| maxCarry| 8 |
| startRoom| 3 |
| totalTreasures| 13 |
| wordLength| 3 |
| lightDuration| 555 |
| numMessages| 89 |
| treasureRoom| 15 |
## Actions
### Action 0 - INTRO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 69, 60, 0, 0, 0, 8707, 1200|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 3| bitflag 3 is false |
| Action| ActionID 58 ArgID 3| set 3 flag |
| Action| ActionID 7 | Print message 'Welcome to Adventure: 8 `PYRAMID OF DOOM`' |
| Action| ActionID 8 | Print message 'By Alvin Files & Scott Adams Dedicated to Ray Harshaw\!' |
### Action 1 - RATS HOLD - Probability: 50 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 50, 1421, 0, 0, 0, 0, 6864, 9150|  |
| Probability| 50%|  |
| Condition| ConditionID 0 ArgID 71| item 'Starving rats(index:71)' carried |
| Action| ActionID 45 | Print message 'Rats' |
| Action| ActionID 114 | Print message 'attacks\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 2 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 328, 193, 180, 160, 0, 10876, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 16| bitflag 16 is set |
| Condition| ConditionID 12 ArgID 9| item 'Lit flashlite(index:9)' in game |
| Action| ActionID 72 ArgID 9, 8| swap item locations 'Lit flashlite(index:9)' and 'Unlit flashlite(index:8)' |
| Action| ActionID 76 | look |
### Action 3 - ARAB - Probability: 2 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2, 554, 540, 0, 0, 0, 7971, 0|  |
| Probability| 2%|  |
| Condition| ConditionID 13 ArgID 27| item 'Small Nomad(index:27)' not in game |
| Action| ActionID 53 ArgID 27| drops item 'Small Nomad(index:27)' into current room |
| Action| ActionID 21 | Print message 'A small desert nomad appears\.\.\.' |
### Action 4 - AMMO - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 289, 280, 80, 0, 0, 8779, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 8 ArgID 14| bitflag 14 is false |
| Action| ActionID 58 ArgID 14| set 14 flag |
| Action| ActionID 79 ArgID 4| set current counter value 4 |
### Action 5 - PISTOL - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 248, 561, 36, 0, 0, 3978, 4050|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Condition| ConditionID 0 ArgID 28| item 'Pistol(index:28)' carried |
| Condition| ConditionID 15 ArgID 1| current counter greater than '1' |
| Action| ActionID 26 | Print message 'Pistol has' |
| Action| ActionID 78 | output current counter |
| Action| ActionID 27 | Print message 'bullets' |
### Action 6 - PISTOL - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 248, 240, 0, 0, 0, 9000, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 12| bitflag 12 is set |
| Action| ActionID 60 ArgID 12| set 12 flag |
### Action 7 - SHOOT ARAB - Probability: 70 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 70, 228, 220, 540, 0, 0, 4374, 9055|  |
| Probability| 70%|  |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Action| ActionID 29 | Print message 'Got him\!\!' |
| Action| ActionID 24 | Print message 'Nomad vanishes in a puff of yellow smoke\.' |
| Action| ActionID 60 ArgID 11| set 11 flag |
| Action| ActionID 55 ArgID 27| Item 'Small Nomad(index:27)' is removed from the game (put in room 0) |
### Action 8 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 228, 220, 0, 0, 0, 9115, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 11| bitflag 11 is set |
| Action| ActionID 60 ArgID 11| set 11 flag |
| Action| ActionID 115 | Print message 'Missed\.\.\.' |
### Action 9 - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 582, 580, 640, 0, 0, 10831, 0|  |
| Probability| 10%|  |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 72 ArgID 29, 32| swap item locations 'Fearsome mummy(index:29)' and 'Enraged mummy(index:32)' |
| Action| ActionID 31 | Print message 'Mummy moves toward me\.' |
### Action 10 - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 642, 0, 0, 0, 0, 4861, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 1 ArgID 32| item 'Enraged mummy(index:32)' in room with player |
| Action| ActionID 32 | Print message 'Mummy has me by the throat\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 11 - GLOVE - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 381, 380, 1020, 0, 0, 8903, 19350|  |
| Probability| 10%|  |
| Condition| ConditionID 0 ArgID 19| item 'I'm wearing an iron glove(index:19)' carried |
| Action| ActionID 59 ArgID 19| Item 'I'm wearing an iron glove(index:19)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 51| drops item 'Iron glove(index:51)' into current room |
| Action| ActionID 129 | Print message 'Glove falls off my sweaty hand' |
### Action 12 - ARAB HELP - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 542, 224, 400, 1194, 408, 18960, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Condition| ConditionID 13 ArgID 59| item 'Glowing skeleton(index:59)' not in game |
| Condition| ConditionID 7 ArgID 20| bitflag 20 is set |
| Action| ActionID 126 | Print message 'Nomad: `Look up decapitated\!`' |
| Action| ActionID 60 ArgID 20| set 20 flag |
### Action 13 - HEAD - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1082, 962, 1180, 1160, 0, 7249, 8003|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 54| item 'Decapitated skeleton(index:54)' in room with player |
| Condition| ConditionID 1 ArgID 48| item 'Skull(index:48)' in room with player |
| Action| ActionID 48 | Print message 'Skeleton places skull on his shoulders, grasps' |
| Action| ActionID 49 | Print message 'metal bar, pulls down ladder' |
| Action| ActionID 53 ArgID 59| drops item 'Glowing skeleton(index:59)' into current room |
| Action| ActionID 53 ArgID 58| drops item 'Ladder(index:58)' into current room |
### Action 14 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1082, 962, 1080, 960, 1060, 8305, 8250|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 54| item 'Decapitated skeleton(index:54)' in room with player |
| Condition| ConditionID 1 ArgID 48| item 'Skull(index:48)' in room with player |
| Action| ActionID 55 ArgID 54| Item 'Decapitated skeleton(index:54)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 48| Item 'Skull(index:48)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 53| Item 'Metal bar protruding from ceiling(index:53)' is removed from the game (put in room 0) |
### Action 15 - ARAB FOLLOWS - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 553, 545, 540, 0, 0, 7950, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 12 ArgID 27| item 'Small Nomad(index:27)' in game |
| Condition| ConditionID 4 ArgID 27| item 'Small Nomad(index:27)' not in room with player |
| Action| ActionID 53 ArgID 27| drops item 'Small Nomad(index:27)' into current room |
### Action 16 - CLAM - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 1262, 62, 60, 200, 1280, 8353, 8753|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 63| item 'Giant Oyster(index:63)' in room with player |
| Condition| ConditionID 1 ArgID 3| item 'Dried Camel Jerky(index:3)' in room with player |
| Action| ActionID 55 ArgID 3| Item 'Dried Camel Jerky(index:3)' is removed from the game (put in room 0) |
| Action| ActionID 103 | Print message 'Oyster makes a slobbering noise' |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 53 ArgID 64| drops item '* BLACK PEARL *(index:64)' into current room |
### Action 17 - ARAB RUN - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 542, 384, 0, 0, 0, 19050, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Condition| ConditionID 3 ArgID 19| player in room 19 |
| Action| ActionID 127 | Print message 'Nomad: `RUN YOU FOOL\!`' |
### Action 18 - OYSTER CLUE - Probability: 25 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 25, 542, 1262, 1294, 408, 400, 19260, 0|  |
| Probability| 25%|  |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Condition| ConditionID 1 ArgID 63| item 'Giant Oyster(index:63)' in room with player |
| Condition| ConditionID 13 ArgID 64| item '\* BLACK PEARL \*(index:64)' not in game |
| Condition| ConditionID 7 ArgID 20| bitflag 20 is set |
| Action| ActionID 128 | Print message 'Nomad: `Oyster thirsty?`' |
| Action| ActionID 60 ArgID 20| set 20 flag |
### Action 19 - STAT FINI - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 348, 1934, 1920, 420, 1720, 9359, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 17| bitflag 17 is set |
| Condition| ConditionID 13 ArgID 96| item 'Pile of Melted iron(index:96)' not in game |
| Action| ActionID 62 ArgID 96, 21| item 'Pile of Melted iron(index:96)' is moved to room 21 |
| Action| ActionID 59 ArgID 86| Item 'Iron statue of Pharoah seated on throne(index:86)' is removed from the game (put in room 0) |
### Action 20 - RATS EAT - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 62, 1422, 60, 1420, 1380, 8322, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 1 ArgID 3| item 'Dried Camel Jerky(index:3)' in room with player |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Action| ActionID 55 ArgID 3| Item 'Dried Camel Jerky(index:3)' is removed from the game (put in room 0) |
| Action| ActionID 72 ArgID 71, 69| swap item locations 'Starving rats(index:71)' and 'Satisfied rats(index:69)' |
### Action 21 - Probability: 30 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 30, 1462, 0, 0, 0, 0, 16914, 9150|  |
| Probability| 30%|  |
| Condition| ConditionID 1 ArgID 73| item 'Hissing cobra(index:73)' in room with player |
| Action| ActionID 112 | Print message 'Cobra' |
| Action| ActionID 114 | Print message 'attacks\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 22 - RATS ATTACK - Probability: 10 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10, 1422, 0, 0, 0, 0, 6864, 9150|  |
| Probability| 10%|  |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Action| ActionID 45 | Print message 'Rats' |
| Action| ActionID 114 | Print message 'attacks\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 23 - WORM - Probability: 40 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 40, 1602, 0, 0, 0, 0, 6211, 0|  |
| Probability| 40%|  |
| Condition| ConditionID 1 ArgID 80| item 'Purple Worm(index:80)' in room with player |
| Action| ActionID 41 | Print message 'Purple worm devours me\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 24 - STATUE - Probability: 20 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 20, 1902, 0, 0, 0, 0, 18061, 0|  |
| Probability| 20%|  |
| Condition| ConditionID 1 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' in room with player |
| Action| ActionID 120 | Print message 'Iron Statue tears me apart\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 25 - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 464, 308, 0, 0, 0, 8626, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 23| player in room 23 |
| Condition| ConditionID 7 ArgID 15| bitflag 15 is set |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 26 - MIRROR ROOM - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 504, 183, 180, 160, 0, 10934, 11400|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Condition| ConditionID 2 ArgID 9| item 'Lit flashlite(index:9)' carried or in room with player |
| Action| ActionID 72 ArgID 9, 8| swap item locations 'Lit flashlite(index:9)' and 'Unlit flashlite(index:8)' |
| Action| ActionID 134 | Print message 'Mirrors EVERYWHERE\! Light blinds me, so I shut it OFF\!' |
| Action| ActionID 76 | look |
### Action 27 - DEATH - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 544, 0, 0, 0, 0, 9813, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 3 ArgID 27| player in room 27 |
| Action| ActionID 65 | score |
| Action| ActionID 63 | game over |
### Action 28 - AMMO USE - Probability: 100 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 100, 28, 20, 20, 0, 0, 9083, 0|  |
| Probability| 100%|  |
| Condition| ConditionID 7 ArgID 1| bitflag 1 is set |
| Action| ActionID 60 ArgID 1| set 1 flag |
| Action| ActionID 83 | subtract from current counter |
### Action 29 - ARAB ATTACK - Probability: 1 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1, 542, 566, 0, 0, 0, 3511, 0|  |
| Probability| 1%|  |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Condition| ConditionID 5 ArgID 28| item 'Pistol(index:28)' not carried |
| Action| ActionID 23 | Print message 'What\! The nomad jumped me while my back was turned\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 30 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 31 - Input: LOO HIE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4527, 304, 0, 0, 0, 0, 19763, 0|  |
| Verb| 30| LOO |
| Noun| 27| HIE |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 113 | Print message 'Strange markings are present\.' |
### Action 32 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 404, 0, 0, 0, 0, 19766, 9150|  |
| Verb| 52| JUM |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 116 | Print message 'Liquid is acid\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 33 - Input: JUM ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7800, 0, 0, 0, 0, 0, 19696, 0|  |
| Verb| 52| JUM |
| Noun| 0| ANY |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 46 | Print message 'Strange \. \. \. Nothing happens\.' |
### Action 34 - Input: SAW BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6218, 224, 1101, 0, 0, 0, 7500, 0|  |
| Verb| 41| SAW |
| Noun| 68| BAR |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Action| ActionID 50 | Print message 'I can't reach it\.' |
### Action 35 - Input: LOO STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4546, 23, 0, 0, 0, 0, 19763, 0|  |
| Verb| 30| LOO |
| Noun| 46| STO |
| Condition| ConditionID 2 ArgID 1| item 'Stone(index:1)' carried or in room with player |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 113 | Print message 'Strange markings are present\.' |
### Action 36 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 0, 0, 0, 0, 0, 0, 0|  |
| Probability| 0%|  |
### Action 37 - Input: SWI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 484, 0, 0, 0, 0, 19694, 0|  |
| Verb| 51| SWI |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 44 | Print message 'That feels good\.' |
### Action 38 - Input: SWI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7650, 404, 0, 0, 0, 0, 19766, 9150|  |
| Verb| 51| SWI |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 116 | Print message 'Liquid is acid\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 39 - Input: THR STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6046, 21, 20, 0, 0, 0, 8081, 0|  |
| Verb| 40| THR |
| Noun| 46| STO |
| Condition| ConditionID 0 ArgID 1| item 'Stone(index:1)' carried |
| Action| ActionID 53 ArgID 1| drops item 'Stone(index:1)' into current room |
| Action| ActionID 131 | Print message 'OK' |
### Action 40 - Input: LOO FIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4583, 1122, 274, 1814, 260, 349, 203, 0|  |
| Verb| 30| LOO |
| Noun| 83| FIR |
| Condition| ConditionID 1 ArgID 56| item 'Fireplace(index:56)' in room with player |
| Condition| ConditionID 13 ArgID 13| item 'Lump of coal(index:13)' not in game |
| Condition| ConditionID 13 ArgID 90| item ' \* RUBY \*(index:90)' not in game |
| Condition| ConditionID 8 ArgID 17| bitflag 17 is false |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 13| drops item 'Lump of coal(index:13)' into current room |
### Action 41 - DIG - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 221, 254, 24, 240, 0, 203, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Condition| ConditionID 13 ArgID 12| item 'Tiny key(index:12)' not in game |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 12| drops item 'Tiny key(index:12)' into current room |
### Action 42 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 226, 0, 0, 0, 0, 300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 11| item 'Shovel(index:11)' not carried |
| Action| ActionID 2 | Print message 'Bare\-handed?' |
### Action 43 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 221, 253, 24, 0, 0, 18300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Condition| ConditionID 12 ArgID 12| item 'Tiny key(index:12)' in game |
| Condition| ConditionID 3 ArgID 1| player in room 1 |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
### Action 44 - SEARCH - Input: LOO EXP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4557, 1522, 1634, 1620, 0, 0, 5753, 0|  |
| Verb| 30| LOO |
| Noun| 57| EXP |
| Condition| ConditionID 1 ArgID 76| item 'Dead explorer chained to wall(index:76)' in room with player |
| Condition| ConditionID 13 ArgID 81| item '\* GOLD PIN \*(index:81)' not in game |
| Action| ActionID 38 | Print message 'Something falls out\.' |
| Action| ActionID 53 ArgID 81| drops item '* GOLD PIN *(index:81)' into current room |
### Action 45 - INVENTORY - Input: GET INV
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1516, 240, 0, 0, 0, 0, 9958, 0|  |
| Verb| 10| GET |
| Noun| 16| INV |
| Action| ActionID 66 | output inventory |
| Action| ActionID 58 ArgID 12| set 12 flag |
### Action 46 - INVENTORY - Input: INV ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6900, 240, 0, 0, 0, 0, 9958, 0|  |
| Verb| 46| INV |
| Noun| 0| ANY |
| Action| ActionID 66 | output inventory |
| Action| ActionID 58 ArgID 12| set 12 flag |
### Action 47 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 44, 0, 0, 0, 0, 18300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
### Action 48 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 44, 273, 0, 0, 0, 18300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 2| player in room 2 |
| Condition| ConditionID 12 ArgID 13| item 'Lump of coal(index:13)' in game |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
### Action 49 - Input: GET STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1546, 84, 22, 334, 320, 20, 7960, 7800|  |
| Verb| 10| GET |
| Noun| 46| STO |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Condition| ConditionID 1 ArgID 1| item 'Stone(index:1)' in room with player |
| Condition| ConditionID 13 ArgID 16| item 'Door with large keyhole(index:16)' not in game |
| Action| ActionID 53 ArgID 16| drops item 'Door with large keyhole(index:16)' into current room |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
| Action| ActionID 52 ArgID 1| get item 'Stone(index:1)', check if can carry |
### Action 50 - WATER - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 484, 81, 80, 100, 0, 8302, 0|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Condition| ConditionID 0 ArgID 4| item 'Empty canteen(index:4)' carried |
| Action| ActionID 55 ArgID 4| Item 'Empty canteen(index:4)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 5| get item 'Full canteen(index:5)', check if can carry |
### Action 51 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 282, 86, 0, 0, 0, 750, 0|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 1 ArgID 14| item 'Pool of liquid(index:14)' in room with player |
| Condition| ConditionID 5 ArgID 4| item 'Empty canteen(index:4)' not carried |
| Action| ActionID 5 | Print message 'No container\.' |
### Action 52 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 282, 101, 0, 0, 0, 0, 900|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 1 ArgID 14| item 'Pool of liquid(index:14)' in room with player |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 6 | Print message 'Canteen is full\.' |
### Action 53 - POOL - Input: GO POO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 162, 64, 480, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 12| POO |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Action| ActionID 54 ArgID 24| move room 24 |
| Action| ActionID 76 | look |
### Action 54 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 64, 81, 80, 100, 0, 8302, 0|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 3| player in room 3 |
| Condition| ConditionID 0 ArgID 4| item 'Empty canteen(index:4)' carried |
| Action| ActionID 55 ArgID 4| Item 'Empty canteen(index:4)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 5| get item 'Full canteen(index:5)', check if can carry |
### Action 55 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 342, 84, 120, 0, 0, 8156, 11400|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 17| item 'Open door(index:17)' in room with player |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 54 ArgID 6| move room 6 |
| Action| ActionID 56 | set darkness flag |
| Action| ActionID 76 | look |
### Action 56 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 322, 84, 0, 0, 0, 1950, 0|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Door with large keyhole(index:16)' in room with player |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 13 | Print message 'The right key could help \(maybe\)\.' |
### Action 57 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 221, 134, 84, 120, 0, 7950, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Condition| ConditionID 13 ArgID 6| item 'Hole(index:6)' not in game |
| Condition| ConditionID 3 ArgID 4| player in room 4 |
| Action| ActionID 53 ArgID 6| drops item 'Hole(index:6)' into current room |
### Action 58 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 221, 122, 0, 0, 0, 18300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Condition| ConditionID 1 ArgID 6| item 'Hole(index:6)' in room with player |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
### Action 59 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 203, 122, 100, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 53| HOL |
| Condition| ConditionID 1 ArgID 6| item 'Hole(index:6)' in room with player |
| Action| ActionID 54 ArgID 5| move room 5 |
| Action| ActionID 76 | look |
### Action 60 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2110, 322, 361, 128, 340, 320, 10800, 0|  |
| Verb| 14| UNL |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Door with large keyhole(index:16)' in room with player |
| Condition| ConditionID 0 ArgID 18| item 'Large key(index:18)' carried |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Action| ActionID 72 ArgID 17, 16| swap item locations 'Open door(index:17)' and 'Door with large keyhole(index:16)' |
### Action 61 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2110, 322, 366, 0, 0, 0, 1950, 0|  |
| Verb| 14| UNL |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Door with large keyhole(index:16)' in room with player |
| Condition| ConditionID 5 ArgID 18| item 'Large key(index:18)' not carried |
| Action| ActionID 13 | Print message 'The right key could help \(maybe\)\.' |
### Action 62 - Input: REA SIG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1809, 302, 0, 0, 0, 0, 1350, 0|  |
| Verb| 12| REA |
| Noun| 9| SIG |
| Condition| ConditionID 1 ArgID 15| item 'Sign(index:15)' in room with player |
| Action| ActionID 9 | Print message 'Sign: He who defiles the tombs of Egypt shall surely perish\!' |
### Action 63 - QUIT - Input: QUI ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2550, 0, 0, 0, 0, 0, 9450, 0|  |
| Verb| 17| QUI |
| Noun| 0| ANY |
| Action| ActionID 63 | game over |
### Action 64 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2110, 322, 361, 129, 0, 0, 2161, 0|  |
| Verb| 14| UNL |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 16| item 'Door with large keyhole(index:16)' in room with player |
| Condition| ConditionID 0 ArgID 18| item 'Large key(index:18)' carried |
| Condition| ConditionID 8 ArgID 6| bitflag 6 is false |
| Action| ActionID 14 | Print message 'Large stone falls on me\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 65 - TRAP OFF - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2110, 104, 241, 120, 140, 520, 1660, 8772|  |
| Verb| 14| UNL |
| Noun| 10| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 0 ArgID 12| item 'Tiny key(index:12)' carried |
| Action| ActionID 11 | Print message 'I hear strange noises\!' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
| Action| ActionID 58 ArgID 6| set 6 flag |
| Action| ActionID 72 ArgID 7, 26| swap item locations 'Tiny locked door(index:7)' and 'Tiny open door(index:26)' |
### Action 66 - Input: UNL DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2110, 104, 246, 0, 0, 0, 1950, 0|  |
| Verb| 14| UNL |
| Noun| 10| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 5 ArgID 12| item 'Tiny key(index:12)' not carried |
| Action| ActionID 13 | Print message 'The right key could help \(maybe\)\.' |
### Action 67 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 104, 128, 0, 0, 0, 2250, 0|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Condition| ConditionID 7 ArgID 6| bitflag 6 is set |
| Action| ActionID 15 | Print message 'Something won't fit\.' |
### Action 68 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6607, 101, 100, 80, 0, 0, 2622, 0|  |
| Verb| 44| DRI |
| Noun| 7| WAT |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 17 | Print message 'Thanks\.' |
| Action| ActionID 72 ArgID 5, 4| swap item locations 'Full canteen(index:5)' and 'Empty canteen(index:4)' |
### Action 69 - Input: UNL SAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2114, 402, 440, 400, 0, 0, 10800, 0|  |
| Verb| 14| UNL |
| Noun| 14| SAR |
| Condition| ConditionID 1 ArgID 20| item 'Closed sarcophagus(index:20)' in room with player |
| Action| ActionID 72 ArgID 22, 20| swap item locations 'Open sarcophagus(index:22)' and 'Closed sarcophagus(index:20)' |
### Action 70 - Input: GO SAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 164, 442, 140, 0, 0, 0, 8176, 8400|  |
| Verb| 1| GO |
| Noun| 14| SAR |
| Condition| ConditionID 1 ArgID 22| item 'Open sarcophagus(index:22)' in room with player |
| Action| ActionID 54 ArgID 7| move room 7 |
| Action| ActionID 76 | look |
| Action| ActionID 56 | set darkness flag |
### Action 71 - Input: BRE SKE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1963, 1082, 480, 1080, 0, 0, 2719, 10800|  |
| Verb| 13| BRE |
| Noun| 13| SKE |
| Condition| ConditionID 1 ArgID 54| item 'Decapitated skeleton(index:54)' in room with player |
| Action| ActionID 18 | Print message 'Crash\!\!\!' |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 24, 54| swap item locations 'Bones(index:24)' and 'Decapitated skeleton(index:54)' |
### Action 72 - Input: ATT SKE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3313, 1082, 480, 1080, 0, 0, 2719, 10800|  |
| Verb| 22| ATT |
| Noun| 13| SKE |
| Condition| ConditionID 1 ArgID 54| item 'Decapitated skeleton(index:54)' in room with player |
| Action| ActionID 18 | Print message 'Crash\!\!\!' |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 24, 54| swap item locations 'Bones(index:24)' and 'Decapitated skeleton(index:54)' |
### Action 73 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 124, 502, 80, 0, 0, 8157, 11400|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 3 ArgID 6| player in room 6 |
| Condition| ConditionID 1 ArgID 25| item 'Open door(index:25)' in room with player |
| Action| ActionID 54 ArgID 4| move room 4 |
| Action| ActionID 57 | clear darkness flag |
| Action| ActionID 76 | look |
### Action 74 - Input: GO ALC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 173, 582, 742, 0, 0, 0, 4984, 0|  |
| Verb| 1| GO |
| Noun| 23| ALC |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Condition| ConditionID 1 ArgID 37| item 'Entrance to an alcove(index:37)' in room with player |
| Action| ActionID 33 | Print message 'Mummy' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 75 - Input: YES ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3750, 0, 0, 0, 0, 0, 3750, 0|  |
| Verb| 25| YES |
| Noun| 0| ANY |
| Action| ActionID 25 | Print message 'Sorry, won't work\.' |
### Action 76 - SHOOT - Input: SHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 566, 0, 0, 0, 0, 300, 0|  |
| Verb| 24| SHO |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 28| item 'Pistol(index:28)' not carried |
| Action| ActionID 2 | Print message 'Bare\-handed?' |
### Action 77 - Input: SHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 19, 0, 0, 0, 0, 4200, 0|  |
| Verb| 24| SHO |
| Noun| 0| ANY |
| Condition| ConditionID 18 ArgID 0| current counter equals 0 |
| Action| ActionID 28 | Print message 'No bullets\.' |
### Action 78 - Input: SHO NOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3617, 220, 20, 0, 0, 0, 8758, 0|  |
| Verb| 24| SHO |
| Noun| 17| NOM |
| Action| ActionID 58 ArgID 11| set 11 flag |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 79 - Input: POU WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 907, 101, 622, 720, 620, 40, 10858, 10950|  |
| Verb| 6| POU |
| Noun| 7| WAT |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Condition| ConditionID 1 ArgID 31| item 'Burning tanna leaves(index:31)' in room with player |
| Action| ActionID 72 ArgID 36, 31| swap item locations 'Wet tanna leaves(index:36)' and 'Burning tanna leaves(index:31)' |
| Action| ActionID 58 ArgID 2| set 2 flag |
| Action| ActionID 73 | continue with next action |
### Action 80 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 48, 100, 80, 0, 0, 10873, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Action| ActionID 72 ArgID 5, 4| swap item locations 'Full canteen(index:5)' and 'Empty canteen(index:4)' |
| Action| ActionID 73 | continue with next action |
### Action 81 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 48, 582, 660, 580, 40, 10860, 10950|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 72 ArgID 33, 29| swap item locations 'Sleeping mummy(index:33)' and 'Fearsome mummy(index:29)' |
| Action| ActionID 60 ArgID 2| set 2 flag |
| Action| ActionID 73 | continue with next action |
### Action 82 - POU - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 48, 642, 640, 660, 40, 10860, 0|  |
| Probability| 0%|  |
| Condition| ConditionID 7 ArgID 2| bitflag 2 is set |
| Condition| ConditionID 1 ArgID 32| item 'Enraged mummy(index:32)' in room with player |
| Action| ActionID 72 ArgID 32, 33| swap item locations 'Enraged mummy(index:32)' and 'Sleeping mummy(index:33)' |
| Action| ActionID 60 ArgID 2| set 2 flag |
### Action 83 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 605, 0, 0, 0, 0, 600, 0|  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 4 ArgID 30| item '\* ANTIQUE TAPESTRY \*(index:30)' not in room with player |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 84 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 582, 0, 0, 0, 0, 4984, 0|  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 33 | Print message 'Mummy' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 85 - Input: GET MUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1522, 582, 0, 0, 0, 0, 4984, 5250|  |
| Verb| 10| GET |
| Noun| 22| MUM |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 33 | Print message 'Mummy' |
| Action| ActionID 34 | Print message 'won't let me' |
| Action| ActionID 35 | Print message 'You be weird\. Cut that out\.' |
### Action 86 - Input: GET LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1521, 622, 0, 0, 0, 0, 4500, 0|  |
| Verb| 10| GET |
| Noun| 21| LEA |
| Condition| ConditionID 1 ArgID 31| item 'Burning tanna leaves(index:31)' in room with player |
| Action| ActionID 30 | Print message 'Too hot\.' |
### Action 87 - Input: SHO MUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3622, 582, 580, 640, 20, 0, 5472, 8700|  |
| Verb| 24| SHO |
| Noun| 22| MUM |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 36 | Print message 'Doesn't bother him\.' |
| Action| ActionID 72 ArgID 29, 32| swap item locations 'Fearsome mummy(index:29)' and 'Enraged mummy(index:32)' |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 88 - Input: SHO MUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3622, 642, 20, 0, 0, 0, 5458, 0|  |
| Verb| 24| SHO |
| Noun| 22| MUM |
| Condition| ConditionID 1 ArgID 32| item 'Enraged mummy(index:32)' in room with player |
| Action| ActionID 36 | Print message 'Doesn't bother him\.' |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 89 - Input: BRE RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2008, 1801, 0, 0, 0, 0, 600, 0|  |
| Verb| 13| BRE |
| Noun| 58| RUB |
| Condition| ConditionID 0 ArgID 90| item ' \* RUBY \*(index:90)' carried |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 90 - Input: LOO SKU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4524, 963, 1014, 1000, 0, 0, 7988, 0|  |
| Verb| 30| LOO |
| Noun| 24| SKU |
| Condition| ConditionID 2 ArgID 48| item 'Skull(index:48)' carried or in room with player |
| Condition| ConditionID 13 ArgID 50| item '\* GOLD TEETH \*(index:50)' not in game |
| Action| ActionID 53 ArgID 50| drops item '* GOLD TEETH *(index:50)' into current room |
| Action| ActionID 38 | Print message 'Something falls out\.' |
### Action 91 - Input: LOO BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4537, 983, 1034, 1020, 394, 493, 188, 7950|  |
| Verb| 30| LOO |
| Noun| 37| BOX |
| Condition| ConditionID 2 ArgID 49| item 'Box(index:49)' carried or in room with player |
| Condition| ConditionID 13 ArgID 51| item 'Iron glove(index:51)' not in game |
| Condition| ConditionID 13 ArgID 19| item 'I'm wearing an iron glove(index:19)' not in game |
| Condition| ConditionID 12 ArgID 24| item 'Bones(index:24)' in game |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 38 | Print message 'Something falls out\.' |
| Action| ActionID 53 ArgID 51| drops item 'Iron glove(index:51)' into current room |
### Action 92 - Input: PUN NOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11867, 542, 0, 0, 0, 0, 5145, 3300|  |
| Verb| 79| PUN |
| Noun| 17| NOM |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Action| ActionID 34 | Print message 'won't let me' |
| Action| ActionID 45 | Print message 'Rats' |
| Action| ActionID 22 | Print message 'The nomad stuck out his tongue at me\.' |
### Action 93 - Input: SHO MUM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3622, 1082, 20, 0, 0, 0, 5458, 0|  |
| Verb| 24| SHO |
| Noun| 22| MUM |
| Condition| ConditionID 1 ArgID 54| item 'Decapitated skeleton(index:54)' in room with player |
| Action| ActionID 36 | Print message 'Doesn't bother him\.' |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 94 - Input: GET POL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1548, 202, 200, 220, 0, 0, 8302, 0|  |
| Verb| 10| GET |
| Noun| 48| POL |
| Condition| ConditionID 1 ArgID 10| item 'Wooden pole sticking from sand(index:10)' in room with player |
| Action| ActionID 55 ArgID 10| Item 'Wooden pole sticking from sand(index:10)' is removed from the game (put in room 0) |
| Action| ActionID 52 ArgID 11| get item 'Shovel(index:11)', check if can carry |
### Action 95 - Input: PUL BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5318, 1062, 0, 0, 0, 0, 7500, 0|  |
| Verb| 35| PUL |
| Noun| 68| BAR |
| Condition| ConditionID 1 ArgID 53| item 'Metal bar protruding from ceiling(index:53)' in room with player |
| Action| ActionID 50 | Print message 'I can't reach it\.' |
### Action 96 - Input: GO BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 218, 1062, 0, 0, 0, 0, 7500, 0|  |
| Verb| 1| GO |
| Noun| 68| BAR |
| Condition| ConditionID 1 ArgID 53| item 'Metal bar protruding from ceiling(index:53)' in room with player |
| Action| ActionID 50 | Print message 'I can't reach it\.' |
### Action 97 - Input: GO LAD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 186, 1162, 360, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 36| LAD |
| Condition| ConditionID 1 ArgID 58| item 'Ladder(index:58)' in room with player |
| Action| ActionID 54 ArgID 18| move room 18 |
| Action| ActionID 76 | look |
### Action 98 - Input: GO ARC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 264, 209, 0, 0, 0, 15600, 0|  |
| Verb| 1| GO |
| Noun| 43| ARC |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 8 ArgID 10| bitflag 10 is false |
| Action| ActionID 104 | Print message 'Oyster won't let me' |
### Action 99 - Input: GO ARC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 193, 264, 208, 1266, 280, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 43| ARC |
| Condition| ConditionID 3 ArgID 13| player in room 13 |
| Condition| ConditionID 7 ArgID 10| bitflag 10 is set |
| Condition| ConditionID 5 ArgID 63| item 'Giant Oyster(index:63)' not carried |
| Action| ActionID 54 ArgID 14| move room 14 |
| Action| ActionID 76 | look |
### Action 100 - . - Input: GET TAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1576, 1202, 1200, 1373, 0, 0, 19702, 0|  |
| Verb| 10| GET |
| Noun| 76| TAB |
| Condition| ConditionID 1 ArgID 60| item 'Table(index:60)' in room with player |
| Condition| ConditionID 12 ArgID 68| item '\* DIAMOND NECKLACE \*(index:68)' in game |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 52 ArgID 60| get item 'Table(index:60)', check if can carry |
### Action 101 - Input: GET STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1546, 22, 20, 0, 0, 0, 7931, 0|  |
| Verb| 10| GET |
| Noun| 46| STO |
| Condition| ConditionID 1 ArgID 1| item 'Stone(index:1)' in room with player |
| Action| ActionID 52 ArgID 1| get item 'Stone(index:1)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 102 - Input: SAW TAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6226, 1103, 1203, 1360, 1374, 0, 203, 0|  |
| Verb| 41| SAW |
| Noun| 76| TAB |
| Condition| ConditionID 2 ArgID 55| item 'Saw(index:55)' carried or in room with player |
| Condition| ConditionID 2 ArgID 60| item 'Table(index:60)' carried or in room with player |
| Condition| ConditionID 13 ArgID 68| item '\* DIAMOND NECKLACE \*(index:68)' not in game |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 68| drops item '* DIAMOND NECKLACE *(index:68)' into current room |
### Action 103 - Input: LIG FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4277, 161, 329, 160, 180, 0, 10876, 0|  |
| Verb| 28| LIG |
| Noun| 77| FLA |
| Condition| ConditionID 0 ArgID 8| item 'Unlit flashlite(index:8)' carried |
| Condition| ConditionID 8 ArgID 16| bitflag 16 is false |
| Action| ActionID 72 ArgID 8, 9| swap item locations 'Unlit flashlite(index:8)' and 'Lit flashlite(index:9)' |
| Action| ActionID 76 | look |
### Action 104 - SCORE - Input: SCO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2400, 0, 0, 0, 0, 0, 9750, 0|  |
| Verb| 16| SCO |
| Noun| 0| ANY |
| Action| ActionID 65 | score |
### Action 105 - Input: UNL FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2177, 181, 160, 180, 0, 0, 10876, 0|  |
| Verb| 14| UNL |
| Noun| 77| FLA |
| Condition| ConditionID 0 ArgID 9| item 'Lit flashlite(index:9)' carried |
| Action| ActionID 72 ArgID 8, 9| swap item locations 'Unlit flashlite(index:8)' and 'Lit flashlite(index:9)' |
| Action| ActionID 76 | look |
### Action 106 - Input: LOO ASH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4555, 324, 1494, 1480, 0, 0, 203, 0|  |
| Verb| 30| LOO |
| Noun| 55| ASH |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Condition| ConditionID 13 ArgID 74| item '\* GOLD NECKLACE \*(index:74)' not in game |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 74| drops item '* GOLD NECKLACE *(index:74)' into current room |
### Action 107 - Input: LOO BAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4532, 1474, 324, 874, 1460, 0, 7951, 0|  |
| Verb| 30| LOO |
| Noun| 32| BAS |
| Condition| ConditionID 13 ArgID 73| item 'Hissing cobra(index:73)' not in game |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Condition| ConditionID 13 ArgID 43| item 'Passageway behind fireplace(index:43)' not in game |
| Action| ActionID 53 ArgID 73| drops item 'Hissing cobra(index:73)' into current room |
| Action| ActionID 1 | Print message 'I see something\.' |
### Action 108 - Input: GET COB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1554, 1462, 0, 0, 0, 0, 16914, 9150|  |
| Verb| 10| GET |
| Noun| 54| COB |
| Condition| ConditionID 1 ArgID 73| item 'Hissing cobra(index:73)' in room with player |
| Action| ActionID 112 | Print message 'Cobra' |
| Action| ActionID 114 | Print message 'attacks\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 109 - Input: PLA FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4842, 324, 874, 1301, 860, 1460, 5603, 8323|  |
| Verb| 32| PLA |
| Noun| 42| FLU |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Condition| ConditionID 13 ArgID 43| item 'Passageway behind fireplace(index:43)' not in game |
| Condition| ConditionID 0 ArgID 65| item 'Flute(index:65)' carried |
| Action| ActionID 37 | Print message 'Cobra crawls out, presses a loose brick and then disappears intoa passage which appeared\.' |
| Action| ActionID 53 ArgID 43| drops item 'Passageway behind fireplace(index:43)' into current room |
| Action| ActionID 55 ArgID 73| Item 'Hissing cobra(index:73)' is removed from the game (put in room 0) |
| Action| ActionID 73 | continue with next action |
### Action 110 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1500, 340, 0, 0, 0, 9300, 0|  |
| Probability| 0%|  |
| Action| ActionID 62 ArgID 75, 17| item 'Passageway(index:75)' is moved to room 17 |
### Action 111 - Input: GET BAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 842, 874, 1460, 0, 0, 5753, 0|  |
| Verb| 10| GET |
| Noun| 32| BAS |
| Condition| ConditionID 1 ArgID 42| item 'Basket(index:42)' in room with player |
| Condition| ConditionID 13 ArgID 43| item 'Passageway behind fireplace(index:43)' not in game |
| Action| ActionID 38 | Print message 'Something falls out\.' |
| Action| ActionID 53 ArgID 73| drops item 'Hissing cobra(index:73)' into current room |
### Action 112 - Input: GO PAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 224, 324, 862, 340, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 74| PAS |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Condition| ConditionID 1 ArgID 43| item 'Passageway behind fireplace(index:43)' in room with player |
| Action| ActionID 54 ArgID 17| move room 17 |
| Action| ActionID 76 | look |
### Action 113 - Input: GO ASH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 205, 324, 1494, 0, 0, 0, 150, 0|  |
| Verb| 1| GO |
| Noun| 55| ASH |
| Condition| ConditionID 3 ArgID 16| player in room 16 |
| Condition| ConditionID 13 ArgID 74| item '\* GOLD NECKLACE \*(index:74)' not in game |
| Action| ActionID 1 | Print message 'I see something\.' |
### Action 114 - Input: GO PAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 224, 344, 1502, 320, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 74| PAS |
| Condition| ConditionID 3 ArgID 17| player in room 17 |
| Condition| ConditionID 1 ArgID 75| item 'Passageway(index:75)' in room with player |
| Action| ActionID 54 ArgID 16| move room 16 |
| Action| ActionID 76 | look |
### Action 115 - Input: PLA FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4842, 1301, 0, 0, 0, 0, 19500, 0|  |
| Verb| 32| PLA |
| Noun| 42| FLU |
| Condition| ConditionID 0 ArgID 65| item 'Flute(index:65)' carried |
| Action| ActionID 130 | Print message 'Ah, 'tis music to my ears\.' |
### Action 116 - Input: GET TAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1576, 1202, 1200, 1374, 0, 0, 7931, 1650|  |
| Verb| 10| GET |
| Noun| 76| TAB |
| Condition| ConditionID 1 ArgID 60| item 'Table(index:60)' in room with player |
| Condition| ConditionID 13 ArgID 68| item '\* DIAMOND NECKLACE \*(index:68)' not in game |
| Action| ActionID 52 ArgID 60| get item 'Table(index:60)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 11 | Print message 'I hear strange noises\!' |
### Action 117 - RUBBISH - Input: LOO RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4558, 1542, 1654, 1640, 0, 0, 203, 0|  |
| Verb| 30| LOO |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 77| item 'Pile of Rubbish(index:77)' in room with player |
| Condition| ConditionID 13 ArgID 82| item '\* JADE CARVING \*(index:82)' not in game |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 82| drops item '* JADE CARVING *(index:82)' into current room |
### Action 118 - Input: LOO RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4558, 1542, 1653, 0, 0, 0, 15961, 0|  |
| Verb| 30| LOO |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 77| item 'Pile of Rubbish(index:77)' in room with player |
| Condition| ConditionID 12 ArgID 82| item '\* JADE CARVING \*(index:82)' in game |
| Action| ActionID 106 | Print message 'I just caught dengue fever\. Very bad\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 119 - Input: GO POR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 209, 1562, 0, 0, 0, 0, 1950, 0|  |
| Verb| 1| GO |
| Noun| 59| POR |
| Condition| ConditionID 1 ArgID 78| item 'Closed portal(index:78)' in room with player |
| Action| ActionID 13 | Print message 'The right key could help \(maybe\)\.' |
### Action 120 - Input: GO POR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 209, 1582, 0, 0, 0, 0, 19861, 0|  |
| Verb| 1| GO |
| Noun| 59| POR |
| Condition| ConditionID 1 ArgID 79| item 'Open portal(index:79)' in room with player |
| Action| ActionID 132 | Print message 'Into the worm's mouth\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 121 - Input: UNL POR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2159, 1562, 1600, 1580, 1560, 0, 8022, 0|  |
| Verb| 14| UNL |
| Noun| 59| POR |
| Condition| ConditionID 1 ArgID 78| item 'Closed portal(index:78)' in room with player |
| Action| ActionID 53 ArgID 80| drops item 'Purple Worm(index:80)' into current room |
| Action| ActionID 72 ArgID 79, 78| swap item locations 'Open portal(index:79)' and 'Closed portal(index:78)' |
### Action 122 - WORM - Input: SHO WOR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3663, 1602, 20, 0, 0, 0, 5458, 0|  |
| Verb| 24| SHO |
| Noun| 63| WOR |
| Condition| ConditionID 1 ArgID 80| item 'Purple Worm(index:80)' in room with player |
| Action| ActionID 36 | Print message 'Doesn't bother him\.' |
| Action| ActionID 58 ArgID 1| set 1 flag |
### Action 123 - Input: WET ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9000, 0, 0, 0, 0, 0, 16350, 0|  |
| Verb| 60| WET |
| Noun| 0| ANY |
| Action| ActionID 109 | Print message 'Pour water?' |
### Action 124 - ROPE - Input: THR ROP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6029, 404, 901, 900, 1700, 0, 8303, 0|  |
| Verb| 40| THR |
| Noun| 29| ROP |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 0 ArgID 45| item 'Rope(index:45)' carried |
| Action| ActionID 55 ArgID 45| Item 'Rope(index:45)' is removed from the game (put in room 0) |
| Action| ActionID 53 ArgID 85| drops item 'Rope hanging from ceiling(index:85)' into current room |
### Action 125 - Input: GO ROP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 179, 404, 1702, 420, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 29| ROP |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 1 ArgID 85| item 'Rope hanging from ceiling(index:85)' in room with player |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 76 | look |
### Action 126 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 203, 404, 1702, 420, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 53| HOL |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 1 ArgID 85| item 'Rope hanging from ceiling(index:85)' in room with player |
| Action| ActionID 54 ArgID 21| move room 21 |
| Action| ActionID 76 | look |
### Action 127 - Input: GO HOL
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 203, 404, 1714, 0, 0, 0, 7500, 0|  |
| Verb| 1| GO |
| Noun| 53| HOL |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 13 ArgID 85| item 'Rope hanging from ceiling(index:85)' not in game |
| Action| ActionID 50 | Print message 'I can't reach it\.' |
### Action 128 - Input: GET LAD
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1536, 1162, 0, 0, 0, 0, 16500, 0|  |
| Verb| 10| GET |
| Noun| 36| LAD |
| Condition| ConditionID 1 ArgID 58| item 'Ladder(index:58)' in room with player |
| Action| ActionID 110 | Print message 'It's stuck\.' |
### Action 129 - Input: BUR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3900, 424, 1120, 0, 0, 0, 6055, 0|  |
| Verb| 26| BUR |
| Noun| 0| ANY |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 40 | Print message '\.' |
| Action| ActionID 55 ArgID 56| Item 'Fireplace(index:56)' is removed from the game (put in room 0) |
### Action 130 - Input: GO POO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 162, 404, 0, 0, 0, 0, 17461, 0|  |
| Verb| 1| GO |
| Noun| 12| POO |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 116 | Print message 'Liquid is acid\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 131 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 404, 101, 0, 0, 0, 900, 0|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 6 | Print message 'Canteen is full\.' |
### Action 132 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 404, 81, 80, 0, 0, 17517, 8250|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 0 ArgID 4| item 'Empty canteen(index:4)' carried |
| Action| ActionID 116 | Print message 'Liquid is acid\.' |
| Action| ActionID 117 | Print message 'Canteen dissolves\.' |
| Action| ActionID 55 ArgID 4| Item 'Empty canteen(index:4)' is removed from the game (put in room 0) |
### Action 133 - Input: GET WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1507, 404, 86, 0, 0, 0, 750, 0|  |
| Verb| 10| GET |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Condition| ConditionID 5 ArgID 4| item 'Empty canteen(index:4)' not carried |
| Action| ActionID 5 | Print message 'No container\.' |
### Action 134 - Input: GO CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 188, 1722, 1880, 1720, 0, 0, 2922, 1500|  |
| Verb| 1| GO |
| Noun| 38| CHA |
| Condition| ConditionID 1 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' in room with player |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 94, 86| swap item locations 'Standing iron statue(index:94)' and 'Iron statue of Pharoah seated on throne(index:86)' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
### Action 135 - Input: GO CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 188, 1882, 1880, 1900, 1840, 0, 1519, 10853|  |
| Verb| 1| GO |
| Noun| 38| CHA |
| Condition| ConditionID 1 ArgID 94| item 'Standing iron statue(index:94)' in room with player |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 94, 95| swap item locations 'Standing iron statue(index:94)' and 'Iron Statue, slowly advancing. . .(index:95)' |
| Action| ActionID 53 ArgID 92| drops item 'Spiral Staircase(index:92)' into current room |
### Action 136 - Input: PUL CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5288, 1722, 1880, 1720, 0, 0, 2922, 1500|  |
| Verb| 35| PUL |
| Noun| 38| CHA |
| Condition| ConditionID 1 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' in room with player |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 94, 86| swap item locations 'Standing iron statue(index:94)' and 'Iron statue of Pharoah seated on throne(index:86)' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
### Action 137 - Input: PUL CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5288, 1882, 1880, 1900, 1840, 0, 1519, 10853|  |
| Verb| 35| PUL |
| Noun| 38| CHA |
| Condition| ConditionID 1 ArgID 94| item 'Standing iron statue(index:94)' in room with player |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 72 ArgID 94, 95| swap item locations 'Standing iron statue(index:94)' and 'Iron Statue, slowly advancing. . .(index:95)' |
| Action| ActionID 53 ArgID 92| drops item 'Spiral Staircase(index:92)' into current room |
### Action 138 - Input: GO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 212, 1902, 0, 0, 0, 0, 17734, 0|  |
| Verb| 1| GO |
| Noun| 62| STA |
| Condition| ConditionID 1 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' in room with player |
| Action| ActionID 118 | Print message 'Iron Statue' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 139 - Input: GO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 212, 1842, 1914, 440, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 62| STA |
| Condition| ConditionID 1 ArgID 92| item 'Spiral Staircase(index:92)' in room with player |
| Condition| ConditionID 13 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' not in game |
| Action| ActionID 54 ArgID 22| move room 22 |
| Action| ActionID 76 | look |
### Action 140 - Input: UNL CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2166, 424, 1734, 1894, 1914, 1874, 10950, 0|  |
| Verb| 14| UNL |
| Noun| 66| CHE |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 13 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' not in game |
| Condition| ConditionID 13 ArgID 94| item 'Standing iron statue(index:94)' not in game |
| Condition| ConditionID 13 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' not in game |
| Condition| ConditionID 13 ArgID 93| item '\* PLATINUM CROWN \*(index:93)' not in game |
| Action| ActionID 73 | continue with next action |
### Action 141 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 1860, 0, 0, 0, 0, 203, 0|  |
| Probability| 0%|  |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 53 ArgID 93| drops item '* PLATINUM CROWN *(index:93)' into current room |
### Action 142 - Input: UNL CHE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2166, 424, 0, 0, 0, 0, 17734, 0|  |
| Verb| 14| UNL |
| Noun| 66| CHE |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 118 | Print message 'Iron Statue' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 143 - Input: THR RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6058, 1801, 404, 1800, 1900, 1880, 8305, 8323|  |
| Verb| 40| THR |
| Noun| 58| RUB |
| Condition| ConditionID 0 ArgID 90| item ' \* RUBY \*(index:90)' carried |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 55 ArgID 90| Item ' * RUBY *(index:90)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 95| Item 'Iron Statue, slowly advancing. . .(index:95)' is removed from the game (put in room 0) |
| Action| ActionID 55 ArgID 94| Item 'Standing iron statue(index:94)' is removed from the game (put in room 0) |
| Action| ActionID 73 | continue with next action |
### Action 144 - Probability: 0 %
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 0, 340, 0, 0, 0, 0, 8831, 18150|  |
| Probability| 0%|  |
| Action| ActionID 58 ArgID 17| set 17 flag |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 121 | Print message 'Ruby falls into pool of acid, burns up\.' |
### Action 145 - Input: REA MUR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1867, 424, 0, 0, 0, 0, 17850, 0|  |
| Verb| 12| REA |
| Noun| 67| MUR |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 119 | Print message 'Mural: Seek ye well the HEART of Iron\.' |
### Action 146 - Input: GET SIG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1509, 302, 0, 0, 0, 0, 16500, 0|  |
| Verb| 10| GET |
| Noun| 9| SIG |
| Condition| ConditionID 1 ArgID 15| item 'Sign(index:15)' in room with player |
| Action| ActionID 110 | Print message 'It's stuck\.' |
### Action 147 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6607, 404, 0, 0, 0, 0, 17461, 0|  |
| Verb| 44| DRI |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 20| player in room 20 |
| Action| ActionID 116 | Print message 'Liquid is acid\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 148 - Input: GET RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1558, 1802, 1882, 1800, 1900, 1880, 7872, 1500|  |
| Verb| 10| GET |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 90| item ' \* RUBY \*(index:90)' in room with player |
| Condition| ConditionID 1 ArgID 94| item 'Standing iron statue(index:94)' in room with player |
| Action| ActionID 52 ArgID 90| get item ' * RUBY *(index:90)', check if can carry |
| Action| ActionID 72 ArgID 95, 94| swap item locations 'Iron Statue, slowly advancing. . .(index:95)' and 'Standing iron statue(index:94)' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
### Action 149 - Input: GET RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1558, 1802, 1722, 1800, 1900, 1720, 7872, 1500|  |
| Verb| 10| GET |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 90| item ' \* RUBY \*(index:90)' in room with player |
| Condition| ConditionID 1 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' in room with player |
| Action| ActionID 52 ArgID 90| get item ' * RUBY *(index:90)', check if can carry |
| Action| ActionID 72 ArgID 95, 86| swap item locations 'Iron Statue, slowly advancing. . .(index:95)' and 'Iron statue of Pharoah seated on throne(index:86)' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
### Action 150 - Input: GO BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 218, 444, 1962, 460, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 68| BAR |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 1 ArgID 98| item 'Open window(index:98)' in room with player |
| Action| ActionID 54 ArgID 23| move room 23 |
| Action| ActionID 76 | look |
### Action 151 - Input: SAW BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6218, 444, 1101, 2000, 1960, 0, 10800, 0|  |
| Verb| 41| SAW |
| Noun| 68| BAR |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Action| ActionID 72 ArgID 100, 98| swap item locations 'Barred window(index:100)' and 'Open window(index:98)' |
### Action 152 - Input: UNL BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2168, 444, 1101, 2000, 1960, 0, 10800, 0|  |
| Verb| 14| UNL |
| Noun| 68| BAR |
| Condition| ConditionID 3 ArgID 22| player in room 22 |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Action| ActionID 72 ArgID 100, 98| swap item locations 'Barred window(index:100)' and 'Open window(index:98)' |
### Action 153 - Input: UNL COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2171, 1982, 381, 1980, 880, 241, 10800, 0|  |
| Verb| 14| UNL |
| Noun| 71| COF |
| Condition| ConditionID 1 ArgID 99| item 'Treasure coffer(index:99)' in room with player |
| Condition| ConditionID 0 ArgID 19| item 'I'm wearing an iron glove(index:19)' carried |
| Condition| ConditionID 0 ArgID 12| item 'Tiny key(index:12)' carried |
| Action| ActionID 72 ArgID 99, 44| swap item locations 'Treasure coffer(index:99)' and 'Open treasure coffer(index:44)' |
### Action 154 - Input: UNL COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2171, 1982, 386, 241, 0, 0, 1861, 0|  |
| Verb| 14| UNL |
| Noun| 71| COF |
| Condition| ConditionID 1 ArgID 99| item 'Treasure coffer(index:99)' in room with player |
| Condition| ConditionID 5 ArgID 19| item 'I'm wearing an iron glove(index:19)' not carried |
| Condition| ConditionID 0 ArgID 12| item 'Tiny key(index:12)' carried |
| Action| ActionID 12 | Print message 'ARRGH\! Poison needle in the lock\.' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 155 - Input: WEA GLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6334, 1021, 1020, 380, 0, 0, 10800, 0|  |
| Verb| 42| WEA |
| Noun| 34| GLO |
| Condition| ConditionID 0 ArgID 51| item 'Iron glove(index:51)' carried |
| Action| ActionID 72 ArgID 51, 19| swap item locations 'Iron glove(index:51)' and 'I'm wearing an iron glove(index:19)' |
### Action 156 - Input: REM GLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8734, 381, 1020, 380, 0, 0, 10800, 0|  |
| Verb| 58| REM |
| Noun| 34| GLO |
| Condition| ConditionID 0 ArgID 19| item 'I'm wearing an iron glove(index:19)' carried |
| Action| ActionID 72 ArgID 51, 19| swap item locations 'Iron glove(index:51)' and 'I'm wearing an iron glove(index:19)' |
### Action 157 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 782, 500, 0, 0, 0, 8231, 0|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 39| item 'Open door(index:39)' in room with player |
| Action| ActionID 54 ArgID 25| move room 25 |
| Action| ActionID 131 | Print message 'OK' |
### Action 158 - Input: REA STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1846, 23, 307, 0, 0, 0, 16050, 0|  |
| Verb| 12| REA |
| Noun| 46| STO |
| Condition| ConditionID 2 ArgID 1| item 'Stone(index:1)' carried or in room with player |
| Condition| ConditionID 6 ArgID 15| player not in room 15 |
| Action| ActionID 107 | Print message 'Confusing\. Part appears missing\.' |
### Action 159 - Input: GO PYR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 230, 0, 0, 0, 0, 0, 600, 0|  |
| Verb| 1| GO |
| Noun| 80| PYR |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 160 - Input: RUB ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5100, 0, 0, 0, 0, 0, 5250, 0|  |
| Verb| 34| RUB |
| Noun| 0| ANY |
| Action| ActionID 35 | Print message 'You be weird\. Cut that out\.' |
### Action 161 - Input: POU WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 907, 101, 100, 80, 0, 0, 19722, 0|  |
| Verb| 6| POU |
| Noun| 7| WAT |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 72 ArgID 5, 4| swap item locations 'Full canteen(index:5)' and 'Empty canteen(index:4)' |
### Action 162 - Input: DIG ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4050, 221, 0, 0, 0, 0, 18300, 0|  |
| Verb| 27| DIG |
| Noun| 0| ANY |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
### Action 163 - Input: SAV GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6825, 0, 0, 0, 0, 0, 10650, 0|  |
| Verb| 45| SAV |
| Noun| 75| GAM |
| Action| ActionID 71 | save game |
### Action 164 - Input: PUL CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5288, 424, 1734, 1914, 1894, 1840, 7951, 0|  |
| Verb| 35| PUL |
| Noun| 38| CHA |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 13 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' not in game |
| Condition| ConditionID 13 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' not in game |
| Condition| ConditionID 13 ArgID 94| item 'Standing iron statue(index:94)' not in game |
| Action| ActionID 53 ArgID 92| drops item 'Spiral Staircase(index:92)' into current room |
| Action| ActionID 1 | Print message 'I see something\.' |
### Action 165 - Input: GO CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 188, 424, 1734, 1914, 1894, 1840, 7951, 0|  |
| Verb| 1| GO |
| Noun| 38| CHA |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Condition| ConditionID 13 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' not in game |
| Condition| ConditionID 13 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' not in game |
| Condition| ConditionID 13 ArgID 94| item 'Standing iron statue(index:94)' not in game |
| Action| ActionID 53 ArgID 92| drops item 'Spiral Staircase(index:92)' into current room |
| Action| ActionID 1 | Print message 'I see something\.' |
### Action 166 - Input: LOO COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4571, 882, 1954, 1940, 0, 0, 7951, 0|  |
| Verb| 30| LOO |
| Noun| 71| COF |
| Condition| ConditionID 1 ArgID 44| item 'Open treasure coffer(index:44)' in room with player |
| Condition| ConditionID 13 ArgID 97| item '\* EMERALD BRACELET \*(index:97)' not in game |
| Action| ActionID 53 ArgID 97| drops item '* EMERALD BRACELET *(index:97)' into current room |
| Action| ActionID 1 | Print message 'I see something\.' |
### Action 167 - Input: BRE MIR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2014, 504, 0, 0, 0, 0, 20611, 0|  |
| Verb| 13| BRE |
| Noun| 64| MIR |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 137 | Print message '1000 years bad luck starts with a cave in\!' |
| Action| ActionID 61 | Death, clear dark flag, move to last room |
### Action 168 - Input: GO ALC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 173, 742, 585, 200, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 23| ALC |
| Condition| ConditionID 1 ArgID 37| item 'Entrance to an alcove(index:37)' in room with player |
| Condition| ConditionID 4 ArgID 29| item 'Fearsome mummy(index:29)' not in room with player |
| Action| ActionID 54 ArgID 10| move room 10 |
| Action| ActionID 76 | look |
### Action 169 - Input: POU WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 907, 101, 80, 100, 0, 0, 10810, 0|  |
| Verb| 6| POU |
| Noun| 7| WAT |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 72 ArgID 4, 5| swap item locations 'Empty canteen(index:4)' and 'Full canteen(index:5)' |
| Action| ActionID 10 | Print message 'The sound of machinery\.' |
### Action 170 - Input: HEL ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1350, 400, 0, 0, 0, 0, 8823, 0|  |
| Verb| 9| HEL |
| Noun| 0| ANY |
| Action| ActionID 58 ArgID 20| set 20 flag |
| Action| ActionID 123 | Print message 'A tiny voice says: `SEARCH AND YE SHALL FIND\!`' |
### Action 171 - Input: GET OYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1540, 1262, 0, 0, 0, 0, 18600, 0|  |
| Verb| 10| GET |
| Noun| 40| OYS |
| Condition| ConditionID 1 ArgID 63| item 'Giant Oyster(index:63)' in room with player |
| Action| ActionID 124 | Print message 'I can't lift it\. This is a big oyster' |
### Action 172 - Input: GET OYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1540, 1265, 0, 0, 0, 0, 18750, 0|  |
| Verb| 10| GET |
| Noun| 40| OYS |
| Condition| ConditionID 4 ArgID 63| item 'Giant Oyster(index:63)' not in room with player |
| Action| ActionID 125 | Print message 'I don't see it' |
### Action 173 - Input: THR RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6058, 1801, 1800, 0, 0, 0, 19703, 0|  |
| Verb| 40| THR |
| Noun| 58| RUB |
| Condition| ConditionID 0 ArgID 90| item ' \* RUBY \*(index:90)' carried |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 53 ArgID 90| drops item ' * RUBY *(index:90)' into current room |
### Action 174 - Input: FEE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11250, 814, 504, 800, 0, 0, 20753, 0|  |
| Verb| 75| FEE |
| Noun| 0| ANY |
| Condition| ConditionID 13 ArgID 40| item '\* GOLD COIN \*(index:40)' not in game |
| Condition| ConditionID 3 ArgID 25| player in room 25 |
| Action| ActionID 138 | Print message 'I feel a coin on the floor' |
| Action| ActionID 53 ArgID 40| drops item '* GOLD COIN *(index:40)' into current room |
### Action 175 - Input: GO STA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 212, 144, 160, 0, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 62| STA |
| Condition| ConditionID 3 ArgID 7| player in room 7 |
| Action| ActionID 54 ArgID 8| move room 8 |
| Action| ActionID 76 | look |
### Action 176 - Input: GO ENT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 229, 104, 0, 0, 0, 0, 600, 0|  |
| Verb| 1| GO |
| Noun| 79| ENT |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 177 - Input: GO DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 160, 104, 0, 0, 0, 0, 600, 0|  |
| Verb| 1| GO |
| Noun| 10| DOO |
| Condition| ConditionID 3 ArgID 5| player in room 5 |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 178 - Input: GET RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1558, 1802, 1800, 0, 0, 0, 7931, 0|  |
| Verb| 10| GET |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 90| item ' \* RUBY \*(index:90)' in room with player |
| Action| ActionID 52 ArgID 90| get item ' * RUBY *(index:90)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 179 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 585, 645, 754, 740, 600, 8024, 19650|  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 4 ArgID 29| item 'Fearsome mummy(index:29)' not in room with player |
| Condition| ConditionID 4 ArgID 32| item 'Enraged mummy(index:32)' not in room with player |
| Condition| ConditionID 13 ArgID 37| item 'Entrance to an alcove(index:37)' not in game |
| Action| ActionID 53 ArgID 37| drops item 'Entrance to an alcove(index:37)' into current room |
| Action| ActionID 74 ArgID 30| take item '* ANTIQUE TAPESTRY *(index:30)', no check done to see if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 180 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 642, 0, 0, 0, 0, 4984, 0|  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 1 ArgID 32| item 'Enraged mummy(index:32)' in room with player |
| Action| ActionID 33 | Print message 'Mummy' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 181 - Input: GO ENT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 229, 742, 582, 0, 0, 0, 4984, 0|  |
| Verb| 1| GO |
| Noun| 79| ENT |
| Condition| ConditionID 1 ArgID 37| item 'Entrance to an alcove(index:37)' in room with player |
| Condition| ConditionID 1 ArgID 29| item 'Fearsome mummy(index:29)' in room with player |
| Action| ActionID 33 | Print message 'Mummy' |
| Action| ActionID 34 | Print message 'won't let me' |
### Action 182 - Input: GO ENT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 229, 742, 585, 200, 0, 0, 8176, 0|  |
| Verb| 1| GO |
| Noun| 79| ENT |
| Condition| ConditionID 1 ArgID 37| item 'Entrance to an alcove(index:37)' in room with player |
| Condition| ConditionID 4 ArgID 29| item 'Fearsome mummy(index:29)' not in room with player |
| Action| ActionID 54 ArgID 10| move room 10 |
| Action| ActionID 76 | look |
### Action 183 - Input: LOO SIG
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4509, 302, 0, 0, 0, 0, 1350, 0|  |
| Verb| 30| LOO |
| Noun| 9| SIG |
| Condition| ConditionID 1 ArgID 15| item 'Sign(index:15)' in room with player |
| Action| ActionID 9 | Print message 'Sign: He who defiles the tombs of Egypt shall surely perish\!' |
### Action 184 - Input: LOO MUR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4567, 424, 0, 0, 0, 0, 17850, 0|  |
| Verb| 30| LOO |
| Noun| 67| MUR |
| Condition| ConditionID 3 ArgID 21| player in room 21 |
| Action| ActionID 119 | Print message 'Mural: Seek ye well the HEART of Iron\.' |
### Action 185 - Input: SHO RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3652, 1422, 344, 1420, 280, 20, 9415, 8716|  |
| Verb| 24| SHO |
| Noun| 52| RAT |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Condition| ConditionID 3 ArgID 17| player in room 17 |
| Action| ActionID 62 ArgID 71, 14| item 'Starving rats(index:71)' is moved to room 14 |
| Action| ActionID 115 | Print message 'Missed\.\.\.' |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 16 | Print message 'Noise scares them off' |
### Action 186 - Input: SHO RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3652, 1422, 1422, 1420, 340, 20, 9415, 8716|  |
| Verb| 24| SHO |
| Noun| 52| RAT |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Action| ActionID 62 ArgID 71, 17| item 'Starving rats(index:71)' is moved to room 17 |
| Action| ActionID 115 | Print message 'Missed\.\.\.' |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 16 | Print message 'Noise scares them off' |
### Action 187 - Input: SMO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7521, 622, 0, 0, 0, 0, 20400, 0|  |
| Verb| 50| SMO |
| Noun| 21| LEA |
| Condition| ConditionID 1 ArgID 31| item 'Burning tanna leaves(index:31)' in room with player |
| Action| ActionID 136 | Print message 'WOW, man, crazy\.\.\.' |
### Action 188 - Input: THR ROP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6029, 901, 900, 0, 0, 0, 8081, 0|  |
| Verb| 40| THR |
| Noun| 29| ROP |
| Condition| ConditionID 0 ArgID 45| item 'Rope(index:45)' carried |
| Action| ActionID 53 ArgID 45| drops item 'Rope(index:45)' into current room |
| Action| ActionID 131 | Print message 'OK' |
### Action 189 - Input: CLO SAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5714, 442, 440, 400, 0, 0, 10931, 0|  |
| Verb| 38| CLO |
| Noun| 14| SAR |
| Condition| ConditionID 1 ArgID 22| item 'Open sarcophagus(index:22)' in room with player |
| Action| ActionID 72 ArgID 22, 20| swap item locations 'Open sarcophagus(index:22)' and 'Closed sarcophagus(index:20)' |
| Action| ActionID 131 | Print message 'OK' |
### Action 190 - Input: LOO BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4537, 983, 494, 480, 0, 0, 188, 7950|  |
| Verb| 30| LOO |
| Noun| 37| BOX |
| Condition| ConditionID 2 ArgID 49| item 'Box(index:49)' carried or in room with player |
| Condition| ConditionID 13 ArgID 24| item 'Bones(index:24)' not in game |
| Action| ActionID 1 | Print message 'I see something\.' |
| Action| ActionID 38 | Print message 'Something falls out\.' |
| Action| ActionID 53 ArgID 24| drops item 'Bones(index:24)' into current room |
### Action 191 - Input: GET HEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1581, 0, 0, 0, 0, 0, 20250, 0|  |
| Verb| 10| GET |
| Noun| 81| HEA |
| Action| ActionID 135 | Print message 'Pharoah's heart is red like yours, yet evil has darkened it\!' |
### Action 192 - Input: LOA PIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7394, 561, 0, 0, 0, 0, 19950, 0|  |
| Verb| 49| LOA |
| Noun| 44| PIS |
| Condition| ConditionID 0 ArgID 28| item 'Pistol(index:28)' carried |
| Action| ActionID 133 | Print message 'TRY: `TAKE INVENTORY`' |
### Action 193 - Input: LOO COA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4572, 263, 0, 0, 0, 0, 6450, 0|  |
| Verb| 30| LOO |
| Noun| 72| COA |
| Condition| ConditionID 2 ArgID 13| item 'Lump of coal(index:13)' carried or in room with player |
| Action| ActionID 43 | Print message 'Its black, dirty & dusty' |
### Action 194 - Input: THR STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6046, 21, 20, 0, 0, 0, 7996, 0|  |
| Verb| 40| THR |
| Noun| 46| STO |
| Condition| ConditionID 0 ArgID 1| item 'Stone(index:1)' carried |
| Action| ActionID 53 ArgID 1| drops item 'Stone(index:1)' into current room |
| Action| ActionID 46 | Print message 'Strange \. \. \. Nothing happens\.' |
### Action 195 - Input: GET BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1568, 224, 0, 0, 0, 0, 7500, 0|  |
| Verb| 10| GET |
| Noun| 68| BAR |
| Condition| ConditionID 3 ArgID 11| player in room 11 |
| Action| ActionID 50 | Print message 'I can't reach it\.' |
### Action 196 - Input: PUN DOO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11860, 762, 760, 780, 381, 0, 10931, 2700|  |
| Verb| 79| PUN |
| Noun| 10| DOO |
| Condition| ConditionID 1 ArgID 38| item 'Bricked up doorway(index:38)' in room with player |
| Condition| ConditionID 0 ArgID 19| item 'I'm wearing an iron glove(index:19)' carried |
| Action| ActionID 72 ArgID 38, 39| swap item locations 'Bricked up doorway(index:38)' and 'Open door(index:39)' |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 18 | Print message 'Crash\!\!\!' |
### Action 197 - Input: THR ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6000, 0, 0, 0, 0, 0, 3085, 0|  |
| Verb| 40| THR |
| Noun| 0| ANY |
| Action| ActionID 20 | Print message 'I don't see any reason to throw a ' |
| Action| ActionID 85 | echo noun |
### Action 198 - Input: LOO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 4500, 0, 0, 0, 0, 0, 18376, 0|  |
| Verb| 30| LOO |
| Noun| 0| ANY |
| Action| ActionID 122 | Print message 'I see nothing special\.' |
| Action| ActionID 76 | look |
### Action 199 - Input: GET BAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1532, 842, 840, 0, 0, 0, 7931, 0|  |
| Verb| 10| GET |
| Noun| 32| BAS |
| Condition| ConditionID 1 ArgID 42| item 'Basket(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Basket(index:42)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 200 - Input: EAT JER
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 8895, 61, 60, 0, 0, 0, 19667, 8250|  |
| Verb| 59| EAT |
| Noun| 45| JER |
| Condition| ConditionID 0 ArgID 3| item 'Dried Camel Jerky(index:3)' carried |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 17 | Print message 'Thanks\.' |
| Action| ActionID 55 ArgID 3| Item 'Dried Camel Jerky(index:3)' is removed from the game (put in room 0) |
### Action 201 - Input: SHO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3600, 20, 0, 0, 0, 0, 19708, 17250|  |
| Verb| 24| SHO |
| Noun| 0| ANY |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 58 ArgID 1| set 1 flag |
| Action| ActionID 115 | Print message 'Missed\.\.\.' |
### Action 202 - Input: SHA ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 7950, 0, 0, 0, 0, 0, 6900, 0|  |
| Verb| 53| SHA |
| Noun| 0| ANY |
| Action| ActionID 46 | Print message 'Strange \. \. \. Nothing happens\.' |
### Action 203 - Input: ASK NOM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9167, 542, 0, 0, 0, 0, 3300, 0|  |
| Verb| 61| ASK |
| Noun| 17| NOM |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Action| ActionID 22 | Print message 'The nomad stuck out his tongue at me\.' |
### Action 204 - Input: UNL OYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2140, 1262, 0, 0, 0, 0, 15600, 0|  |
| Verb| 14| UNL |
| Noun| 40| OYS |
| Condition| ConditionID 1 ArgID 63| item 'Giant Oyster(index:63)' in room with player |
| Action| ActionID 104 | Print message 'Oyster won't let me' |
### Action 205 - Input: REA HIE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1827, 304, 32, 0, 0, 0, 16050, 0|  |
| Verb| 12| REA |
| Noun| 27| HIE |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 11 ArgID 1| item 'Stone(index:1)' not carried or in room with player |
| Action| ActionID 107 | Print message 'Confusing\. Part appears missing\.' |
### Action 206 - Input: REA HIE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1827, 304, 23, 0, 0, 0, 19752, 0|  |
| Verb| 12| REA |
| Noun| 27| HIE |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Condition| ConditionID 2 ArgID 1| item 'Stone(index:1)' carried or in room with player |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 102 | Print message 'It says: `LEAVE \*TREASURES\* HERE\!`' |
### Action 207 - Input: REA STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1846, 23, 304, 0, 0, 0, 19752, 0|  |
| Verb| 12| REA |
| Noun| 46| STO |
| Condition| ConditionID 2 ArgID 1| item 'Stone(index:1)' carried or in room with player |
| Condition| ConditionID 3 ArgID 15| player in room 15 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 102 | Print message 'It says: `LEAVE \*TREASURES\* HERE\!`' |
### Action 208 - Input: FEE RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11302, 1422, 63, 1420, 1380, 60, 19722, 8250|  |
| Verb| 75| FEE |
| Noun| 52| RAT |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Condition| ConditionID 2 ArgID 3| item 'Dried Camel Jerky(index:3)' carried or in room with player |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 72 ArgID 71, 69| swap item locations 'Starving rats(index:71)' and 'Satisfied rats(index:69)' |
| Action| ActionID 55 ArgID 3| Item 'Dried Camel Jerky(index:3)' is removed from the game (put in room 0) |
### Action 209 - Input: DRI WAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6607, 484, 0, 0, 0, 0, 19667, 0|  |
| Verb| 44| DRI |
| Noun| 7| WAT |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 17 | Print message 'Thanks\.' |
### Action 210 - Input: GO PAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 224, 184, 0, 0, 0, 0, 16200, 0|  |
| Verb| 1| GO |
| Noun| 74| PAS |
| Condition| ConditionID 3 ArgID 9| player in room 9 |
| Action| ActionID 108 | Print message 'I'm there\.' |
### Action 211 - Input: FEE OYS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11290, 1262, 61, 60, 200, 1280, 8308, 8053|  |
| Verb| 75| FEE |
| Noun| 40| OYS |
| Condition| ConditionID 1 ArgID 63| item 'Giant Oyster(index:63)' in room with player |
| Condition| ConditionID 0 ArgID 3| item 'Dried Camel Jerky(index:3)' carried |
| Action| ActionID 55 ArgID 3| Item 'Dried Camel Jerky(index:3)' is removed from the game (put in room 0) |
| Action| ActionID 58 ArgID 10| set 10 flag |
| Action| ActionID 53 ArgID 64| drops item '* BLACK PEARL *(index:64)' into current room |
| Action| ActionID 103 | Print message 'Oyster makes a slobbering noise' |
### Action 212 - Input: GET ASH
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1555, 822, 0, 0, 0, 0, 630, 0|  |
| Verb| 10| GET |
| Noun| 55| ASH |
| Condition| ConditionID 1 ArgID 41| item 'Ashes(index:41)' in room with player |
| Action| ActionID 4 | Print message 'I can't\.' |
| Action| ActionID 30 | Print message 'Too hot\.' |
### Action 213 - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1520, 585, 645, 753, 600, 0, 19724, 0|  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 4 ArgID 29| item 'Fearsome mummy(index:29)' not in room with player |
| Condition| ConditionID 4 ArgID 32| item 'Enraged mummy(index:32)' not in room with player |
| Condition| ConditionID 12 ArgID 37| item 'Entrance to an alcove(index:37)' in game |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 74 ArgID 30| take item '* ANTIQUE TAPESTRY *(index:30)', no check done to see if can carry |
### Action 214 - Input: SAW CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6188, 1101, 1522, 0, 0, 0, 6300, 0|  |
| Verb| 41| SAW |
| Noun| 38| CHA |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Condition| ConditionID 1 ArgID 76| item 'Dead explorer chained to wall(index:76)' in room with player |
| Action| ActionID 42 | Print message 'Chain too tough\.' |
### Action 215 - Input: SAW CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 6188, 1101, 1722, 0, 0, 0, 6300, 0|  |
| Verb| 41| SAW |
| Noun| 38| CHA |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Condition| ConditionID 1 ArgID 86| item 'Iron statue of Pharoah seated on throne(index:86)' in room with player |
| Action| ActionID 42 | Print message 'Chain too tough\.' |
### Action 216 - Input: UNC EXP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10557, 1522, 0, 0, 0, 0, 6300, 0|  |
| Verb| 70| UNC |
| Noun| 57| EXP |
| Condition| ConditionID 1 ArgID 76| item 'Dead explorer chained to wall(index:76)' in room with player |
| Action| ActionID 42 | Print message 'Chain too tough\.' |
### Action 217 - Input: ASK ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 9150, 0, 0, 0, 0, 0, 6900, 0|  |
| Verb| 61| ASK |
| Noun| 0| ANY |
| Action| ActionID 46 | Print message 'Strange \. \. \. Nothing happens\.' |
### Action 218 - Input: PUL CHA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5288, 1902, 0, 0, 0, 0, 19669, 19050|  |
| Verb| 35| PUL |
| Noun| 38| CHA |
| Condition| ConditionID 1 ArgID 95| item 'Iron Statue, slowly advancing\. \. \.(index:95)' in room with player |
| Action| ActionID 131 | Print message 'OK' |
| Action| ActionID 19 | Print message 'I hear a hollow laugh\. \. \.' |
| Action| ActionID 127 | Print message 'Nomad: `RUN YOU FOOL\!`' |
### Action 219 - Input: POU CAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 951, 0, 0, 0, 0, 0, 16350, 0|  |
| Verb| 6| POU |
| Noun| 51| CAN |
| Action| ActionID 109 | Print message 'Pour water?' |
### Action 220 - Input: CLO ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 5700, 0, 0, 0, 0, 0, 600, 0|  |
| Verb| 38| CLO |
| Noun| 0| ANY |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 221 - Input: GET LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1521, 722, 720, 0, 0, 0, 7931, 0|  |
| Verb| 10| GET |
| Noun| 21| LEA |
| Condition| ConditionID 1 ArgID 36| item 'Wet tanna leaves(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Wet tanna leaves(index:36)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 222 - Input: GET BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1568, 1342, 1340, 0, 0, 0, 7931, 0|  |
| Verb| 10| GET |
| Noun| 68| BAR |
| Condition| ConditionID 1 ArgID 67| item '\* PLATINUM BAR \*(index:67)' in room with player |
| Action| ActionID 52 ArgID 67| get item '* PLATINUM BAR *(index:67)', check if can carry |
| Action| ActionID 131 | Print message 'OK' |
### Action 223 - Input: UNL COF
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 2171, 1982, 246, 0, 0, 0, 7050, 0|  |
| Verb| 14| UNL |
| Noun| 71| COF |
| Condition| ConditionID 1 ArgID 99| item 'Treasure coffer(index:99)' in room with player |
| Condition| ConditionID 5 ArgID 12| item 'Tiny key(index:12)' not carried |
| Action| ActionID 47 | Print message 'Its locked\.' |
### Action 224 - Input: CLE COA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10872, 263, 260, 1800, 103, 0, 10931, 0|  |
| Verb| 72| CLE |
| Noun| 72| COA |
| Condition| ConditionID 2 ArgID 13| item 'Lump of coal(index:13)' carried or in room with player |
| Condition| ConditionID 2 ArgID 5| item 'Full canteen(index:5)' carried or in room with player |
| Action| ActionID 72 ArgID 13, 90| swap item locations 'Lump of coal(index:13)' and ' * RUBY *(index:90)' |
| Action| ActionID 131 | Print message 'OK' |
### Action 225 - Input: CLE COA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 10872, 263, 260, 1800, 484, 0, 10931, 0|  |
| Verb| 72| CLE |
| Noun| 72| COA |
| Condition| ConditionID 2 ArgID 13| item 'Lump of coal(index:13)' carried or in room with player |
| Condition| ConditionID 3 ArgID 24| player in room 24 |
| Action| ActionID 72 ArgID 13, 90| swap item locations 'Lump of coal(index:13)' and ' * RUBY *(index:90)' |
| Action| ActionID 131 | Print message 'OK' |
### Action 226 - Input: BRE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 1950, 0, 0, 0, 0, 0, 600, 0|  |
| Verb| 13| BRE |
| Noun| 0| ANY |
| Action| ActionID 4 | Print message 'I can't\.' |
### Action 227 - Input: PUN ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11850, 386, 0, 0, 0, 0, 300, 0|  |
| Verb| 79| PUN |
| Noun| 0| ANY |
| Condition| ConditionID 5 ArgID 19| item 'I'm wearing an iron glove(index:19)' not carried |
| Action| ActionID 2 | Print message 'Bare\-handed?' |
### Action 228 - Input: ATT ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 3300, 542, 0, 0, 0, 0, 300, 0|  |
| Verb| 22| ATT |
| Noun| 0| ANY |
| Condition| ConditionID 1 ArgID 27| item 'Small Nomad(index:27)' in room with player |
| Action| ActionID 2 | Print message 'Bare\-handed?' |
### Action 229 - . - Input: FEE ANY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| 11250, 0, 0, 0, 0, 0, 5250, 0|  |
| Verb| 75| FEE |
| Noun| 0| ANY |
| Action| ActionID 35 | Print message 'You be weird\. Cut that out\.' |
### Action 231 - Take for item Stone - Input: GET STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 46| STO |
| Condition| ConditionID 1 ArgID 1| item 'Stone(index:1)' in room with player |
| Action| ActionID 52 ArgID 1| get item 'Stone(index:1)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 232 - Drop for item Stone - Input: DRO STO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 46| STO |
| Condition| ConditionID 0 ArgID 1| item 'Stone(index:1)' carried |
| Action| ActionID 53 ArgID 1| drops item 'Stone(index:1)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 233 - Take for item Dried Camel Jerky - Input: GET JER
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 45| JER |
| Condition| ConditionID 1 ArgID 3| item 'Dried Camel Jerky(index:3)' in room with player |
| Action| ActionID 52 ArgID 3| get item 'Dried Camel Jerky(index:3)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 234 - Drop for item Dried Camel Jerky - Input: DRO JER
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 45| JER |
| Condition| ConditionID 0 ArgID 3| item 'Dried Camel Jerky(index:3)' carried |
| Action| ActionID 53 ArgID 3| drops item 'Dried Camel Jerky(index:3)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 235 - Take for item Empty canteen - Input: GET CAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 51| CAN |
| Condition| ConditionID 1 ArgID 4| item 'Empty canteen(index:4)' in room with player |
| Action| ActionID 52 ArgID 4| get item 'Empty canteen(index:4)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 236 - Drop for item Empty canteen - Input: DRO CAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 51| CAN |
| Condition| ConditionID 0 ArgID 4| item 'Empty canteen(index:4)' carried |
| Action| ActionID 53 ArgID 4| drops item 'Empty canteen(index:4)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 237 - Take for item Full canteen - Input: GET CAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 51| CAN |
| Condition| ConditionID 1 ArgID 5| item 'Full canteen(index:5)' in room with player |
| Action| ActionID 52 ArgID 5| get item 'Full canteen(index:5)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 238 - Drop for item Full canteen - Input: DRO CAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 51| CAN |
| Condition| ConditionID 0 ArgID 5| item 'Full canteen(index:5)' carried |
| Action| ActionID 53 ArgID 5| drops item 'Full canteen(index:5)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 239 - Take for item Unlit flashlite - Input: GET FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 77| FLA |
| Condition| ConditionID 1 ArgID 8| item 'Unlit flashlite(index:8)' in room with player |
| Action| ActionID 52 ArgID 8| get item 'Unlit flashlite(index:8)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 240 - Drop for item Unlit flashlite - Input: DRO FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 77| FLA |
| Condition| ConditionID 0 ArgID 8| item 'Unlit flashlite(index:8)' carried |
| Action| ActionID 53 ArgID 8| drops item 'Unlit flashlite(index:8)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 241 - Take for item Lit flashlite - Input: GET FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 77| FLA |
| Condition| ConditionID 1 ArgID 9| item 'Lit flashlite(index:9)' in room with player |
| Action| ActionID 52 ArgID 9| get item 'Lit flashlite(index:9)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 242 - Drop for item Lit flashlite - Input: DRO FLA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 77| FLA |
| Condition| ConditionID 0 ArgID 9| item 'Lit flashlite(index:9)' carried |
| Action| ActionID 53 ArgID 9| drops item 'Lit flashlite(index:9)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 243 - Take for item Shovel - Input: GET SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 49| SHO |
| Condition| ConditionID 1 ArgID 11| item 'Shovel(index:11)' in room with player |
| Action| ActionID 52 ArgID 11| get item 'Shovel(index:11)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 244 - Drop for item Shovel - Input: DRO SHO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 49| SHO |
| Condition| ConditionID 0 ArgID 11| item 'Shovel(index:11)' carried |
| Action| ActionID 53 ArgID 11| drops item 'Shovel(index:11)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 245 - Take for item Tiny key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 56| KEY |
| Condition| ConditionID 1 ArgID 12| item 'Tiny key(index:12)' in room with player |
| Action| ActionID 52 ArgID 12| get item 'Tiny key(index:12)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 246 - Drop for item Tiny key - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 56| KEY |
| Condition| ConditionID 0 ArgID 12| item 'Tiny key(index:12)' carried |
| Action| ActionID 53 ArgID 12| drops item 'Tiny key(index:12)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 247 - Take for item Lump of coal - Input: GET COA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 72| COA |
| Condition| ConditionID 1 ArgID 13| item 'Lump of coal(index:13)' in room with player |
| Action| ActionID 52 ArgID 13| get item 'Lump of coal(index:13)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 248 - Drop for item Lump of coal - Input: DRO COA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 72| COA |
| Condition| ConditionID 0 ArgID 13| item 'Lump of coal(index:13)' carried |
| Action| ActionID 53 ArgID 13| drops item 'Lump of coal(index:13)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 249 - Take for item Large key - Input: GET KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 56| KEY |
| Condition| ConditionID 1 ArgID 18| item 'Large key(index:18)' in room with player |
| Action| ActionID 52 ArgID 18| get item 'Large key(index:18)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 250 - Drop for item Large key - Input: DRO KEY
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 56| KEY |
| Condition| ConditionID 0 ArgID 18| item 'Large key(index:18)' carried |
| Action| ActionID 53 ArgID 18| drops item 'Large key(index:18)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 251 - Take for item Mouldy bandages - Input: GET BAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 15| BAN |
| Condition| ConditionID 1 ArgID 21| item 'Mouldy bandages(index:21)' in room with player |
| Action| ActionID 52 ArgID 21| get item 'Mouldy bandages(index:21)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 252 - Drop for item Mouldy bandages - Input: DRO BAN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 15| BAN |
| Condition| ConditionID 0 ArgID 21| item 'Mouldy bandages(index:21)' carried |
| Action| ActionID 53 ArgID 21| drops item 'Mouldy bandages(index:21)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 253 - Take for item Bones - Input: GET BON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 19| BON |
| Condition| ConditionID 1 ArgID 24| item 'Bones(index:24)' in room with player |
| Action| ActionID 52 ArgID 24| get item 'Bones(index:24)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 254 - Drop for item Bones - Input: DRO BON
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 19| BON |
| Condition| ConditionID 0 ArgID 24| item 'Bones(index:24)' carried |
| Action| ActionID 53 ArgID 24| drops item 'Bones(index:24)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 255 - Take for item Pistol - Input: GET PIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 44| PIS |
| Condition| ConditionID 1 ArgID 28| item 'Pistol(index:28)' in room with player |
| Action| ActionID 52 ArgID 28| get item 'Pistol(index:28)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 256 - Drop for item Pistol - Input: DRO PIS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 44| PIS |
| Condition| ConditionID 0 ArgID 28| item 'Pistol(index:28)' carried |
| Action| ActionID 53 ArgID 28| drops item 'Pistol(index:28)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 257 - Take for item * ANTIQUE TAPESTRY * - Input: GET TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 20| TAP |
| Condition| ConditionID 1 ArgID 30| item '\* ANTIQUE TAPESTRY \*(index:30)' in room with player |
| Action| ActionID 52 ArgID 30| get item '* ANTIQUE TAPESTRY *(index:30)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 258 - Drop for item * ANTIQUE TAPESTRY * - Input: DRO TAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 20| TAP |
| Condition| ConditionID 0 ArgID 30| item '\* ANTIQUE TAPESTRY \*(index:30)' carried |
| Action| ActionID 53 ArgID 30| drops item '* ANTIQUE TAPESTRY *(index:30)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 259 - Take for item * GOLD SCARAB * - Input: GET SCA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 82| SCA |
| Condition| ConditionID 1 ArgID 34| item '\* GOLD SCARAB \*(index:34)' in room with player |
| Action| ActionID 52 ArgID 34| get item '* GOLD SCARAB *(index:34)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 260 - Drop for item * GOLD SCARAB * - Input: DRO SCA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 82| SCA |
| Condition| ConditionID 0 ArgID 34| item '\* GOLD SCARAB \*(index:34)' carried |
| Action| ActionID 53 ArgID 34| drops item '* GOLD SCARAB *(index:34)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 261 - Take for item Wet tanna leaves - Input: GET LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 21| LEA |
| Condition| ConditionID 1 ArgID 36| item 'Wet tanna leaves(index:36)' in room with player |
| Action| ActionID 52 ArgID 36| get item 'Wet tanna leaves(index:36)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 262 - Drop for item Wet tanna leaves - Input: DRO LEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 21| LEA |
| Condition| ConditionID 0 ArgID 36| item 'Wet tanna leaves(index:36)' carried |
| Action| ActionID 53 ArgID 36| drops item 'Wet tanna leaves(index:36)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 263 - Take for item * GOLD COIN * - Input: GET COI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 73| COI |
| Condition| ConditionID 1 ArgID 40| item '\* GOLD COIN \*(index:40)' in room with player |
| Action| ActionID 52 ArgID 40| get item '* GOLD COIN *(index:40)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 264 - Drop for item * GOLD COIN * - Input: DRO COI
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 73| COI |
| Condition| ConditionID 0 ArgID 40| item '\* GOLD COIN \*(index:40)' carried |
| Action| ActionID 53 ArgID 40| drops item '* GOLD COIN *(index:40)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 265 - Take for item Basket - Input: GET BAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 32| BAS |
| Condition| ConditionID 1 ArgID 42| item 'Basket(index:42)' in room with player |
| Action| ActionID 52 ArgID 42| get item 'Basket(index:42)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 266 - Drop for item Basket - Input: DRO BAS
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 32| BAS |
| Condition| ConditionID 0 ArgID 42| item 'Basket(index:42)' carried |
| Action| ActionID 53 ArgID 42| drops item 'Basket(index:42)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 267 - Take for item Rope - Input: GET ROP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 29| ROP |
| Condition| ConditionID 1 ArgID 45| item 'Rope(index:45)' in room with player |
| Action| ActionID 52 ArgID 45| get item 'Rope(index:45)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 268 - Drop for item Rope - Input: DRO ROP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 29| ROP |
| Condition| ConditionID 0 ArgID 45| item 'Rope(index:45)' carried |
| Action| ActionID 53 ArgID 45| drops item 'Rope(index:45)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 269 - Take for item Chopping block - Input: GET BLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 31| BLO |
| Condition| ConditionID 1 ArgID 47| item 'Chopping block(index:47)' in room with player |
| Action| ActionID 52 ArgID 47| get item 'Chopping block(index:47)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 270 - Drop for item Chopping block - Input: DRO BLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 31| BLO |
| Condition| ConditionID 0 ArgID 47| item 'Chopping block(index:47)' carried |
| Action| ActionID 53 ArgID 47| drops item 'Chopping block(index:47)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 271 - Take for item Skull - Input: GET SKU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 24| SKU |
| Condition| ConditionID 1 ArgID 48| item 'Skull(index:48)' in room with player |
| Action| ActionID 52 ArgID 48| get item 'Skull(index:48)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 272 - Drop for item Skull - Input: DRO SKU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 24| SKU |
| Condition| ConditionID 0 ArgID 48| item 'Skull(index:48)' carried |
| Action| ActionID 53 ArgID 48| drops item 'Skull(index:48)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 273 - Take for item Box - Input: GET BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 37| BOX |
| Condition| ConditionID 1 ArgID 49| item 'Box(index:49)' in room with player |
| Action| ActionID 52 ArgID 49| get item 'Box(index:49)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 274 - Drop for item Box - Input: DRO BOX
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 37| BOX |
| Condition| ConditionID 0 ArgID 49| item 'Box(index:49)' carried |
| Action| ActionID 53 ArgID 49| drops item 'Box(index:49)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 275 - Take for item * GOLD TEETH * - Input: GET TEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 33| TEE |
| Condition| ConditionID 1 ArgID 50| item '\* GOLD TEETH \*(index:50)' in room with player |
| Action| ActionID 52 ArgID 50| get item '* GOLD TEETH *(index:50)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 276 - Drop for item * GOLD TEETH * - Input: DRO TEE
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 33| TEE |
| Condition| ConditionID 0 ArgID 50| item '\* GOLD TEETH \*(index:50)' carried |
| Action| ActionID 53 ArgID 50| drops item '* GOLD TEETH *(index:50)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 277 - Take for item Iron glove - Input: GET GLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 34| GLO |
| Condition| ConditionID 1 ArgID 51| item 'Iron glove(index:51)' in room with player |
| Action| ActionID 52 ArgID 51| get item 'Iron glove(index:51)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 278 - Drop for item Iron glove - Input: DRO GLO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 34| GLO |
| Condition| ConditionID 0 ArgID 51| item 'Iron glove(index:51)' carried |
| Action| ActionID 53 ArgID 51| drops item 'Iron glove(index:51)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 279 - Take for item Saw - Input: GET SAW
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 35| SAW |
| Condition| ConditionID 1 ArgID 55| item 'Saw(index:55)' in room with player |
| Action| ActionID 52 ArgID 55| get item 'Saw(index:55)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 280 - Drop for item Saw - Input: DRO SAW
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 35| SAW |
| Condition| ConditionID 0 ArgID 55| item 'Saw(index:55)' carried |
| Action| ActionID 53 ArgID 55| drops item 'Saw(index:55)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 281 - Take for item Table - Input: GET TAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 76| TAB |
| Condition| ConditionID 1 ArgID 60| item 'Table(index:60)' in room with player |
| Action| ActionID 52 ArgID 60| get item 'Table(index:60)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 282 - Drop for item Table - Input: DRO TAB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 76| TAB |
| Condition| ConditionID 0 ArgID 60| item 'Table(index:60)' carried |
| Action| ActionID 53 ArgID 60| drops item 'Table(index:60)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 283 - Take for item * BLACK PEARL * - Input: GET PEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 41| PEA |
| Condition| ConditionID 1 ArgID 64| item '\* BLACK PEARL \*(index:64)' in room with player |
| Action| ActionID 52 ArgID 64| get item '* BLACK PEARL *(index:64)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 284 - Drop for item * BLACK PEARL * - Input: DRO PEA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 41| PEA |
| Condition| ConditionID 0 ArgID 64| item '\* BLACK PEARL \*(index:64)' carried |
| Action| ActionID 53 ArgID 64| drops item '* BLACK PEARL *(index:64)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 285 - Take for item Flute - Input: GET FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 42| FLU |
| Condition| ConditionID 1 ArgID 65| item 'Flute(index:65)' in room with player |
| Action| ActionID 52 ArgID 65| get item 'Flute(index:65)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 286 - Drop for item Flute - Input: DRO FLU
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 42| FLU |
| Condition| ConditionID 0 ArgID 65| item 'Flute(index:65)' carried |
| Action| ActionID 53 ArgID 65| drops item 'Flute(index:65)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 287 - Take for item * PLATINUM BAR * - Input: GET BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 68| BAR |
| Condition| ConditionID 1 ArgID 67| item '\* PLATINUM BAR \*(index:67)' in room with player |
| Action| ActionID 52 ArgID 67| get item '* PLATINUM BAR *(index:67)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 288 - Drop for item * PLATINUM BAR * - Input: DRO BAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 68| BAR |
| Condition| ConditionID 0 ArgID 67| item '\* PLATINUM BAR \*(index:67)' carried |
| Action| ActionID 53 ArgID 67| drops item '* PLATINUM BAR *(index:67)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 289 - Take for item * DIAMOND NECKLACE * - Input: GET NEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 50| NEC |
| Condition| ConditionID 1 ArgID 68| item '\* DIAMOND NECKLACE \*(index:68)' in room with player |
| Action| ActionID 52 ArgID 68| get item '* DIAMOND NECKLACE *(index:68)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 290 - Drop for item * DIAMOND NECKLACE * - Input: DRO NEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 50| NEC |
| Condition| ConditionID 0 ArgID 68| item '\* DIAMOND NECKLACE \*(index:68)' carried |
| Action| ActionID 53 ArgID 68| drops item '* DIAMOND NECKLACE *(index:68)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 291 - Take for item Satisfied rats - Input: GET RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 52| RAT |
| Condition| ConditionID 1 ArgID 69| item 'Satisfied rats(index:69)' in room with player |
| Action| ActionID 52 ArgID 69| get item 'Satisfied rats(index:69)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 292 - Drop for item Satisfied rats - Input: DRO RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 52| RAT |
| Condition| ConditionID 0 ArgID 69| item 'Satisfied rats(index:69)' carried |
| Action| ActionID 53 ArgID 69| drops item 'Satisfied rats(index:69)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 293 - Take for item Starving rats - Input: GET RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 52| RAT |
| Condition| ConditionID 1 ArgID 71| item 'Starving rats(index:71)' in room with player |
| Action| ActionID 52 ArgID 71| get item 'Starving rats(index:71)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 294 - Drop for item Starving rats - Input: DRO RAT
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 52| RAT |
| Condition| ConditionID 0 ArgID 71| item 'Starving rats(index:71)' carried |
| Action| ActionID 53 ArgID 71| drops item 'Starving rats(index:71)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 295 - Take for item * GOLD NECKLACE * - Input: GET NEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 50| NEC |
| Condition| ConditionID 1 ArgID 74| item '\* GOLD NECKLACE \*(index:74)' in room with player |
| Action| ActionID 52 ArgID 74| get item '* GOLD NECKLACE *(index:74)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 296 - Drop for item * GOLD NECKLACE * - Input: DRO NEC
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 50| NEC |
| Condition| ConditionID 0 ArgID 74| item '\* GOLD NECKLACE \*(index:74)' carried |
| Action| ActionID 53 ArgID 74| drops item '* GOLD NECKLACE *(index:74)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 297 - Take for item * GOLD PIN * - Input: GET PIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 60| PIN |
| Condition| ConditionID 1 ArgID 81| item '\* GOLD PIN \*(index:81)' in room with player |
| Action| ActionID 52 ArgID 81| get item '* GOLD PIN *(index:81)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 298 - Drop for item * GOLD PIN * - Input: DRO PIN
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 60| PIN |
| Condition| ConditionID 0 ArgID 81| item '\* GOLD PIN \*(index:81)' carried |
| Action| ActionID 53 ArgID 81| drops item '* GOLD PIN *(index:81)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 299 - Take for item * JADE CARVING * - Input: GET CAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 61| CAR |
| Condition| ConditionID 1 ArgID 82| item '\* JADE CARVING \*(index:82)' in room with player |
| Action| ActionID 52 ArgID 82| get item '* JADE CARVING *(index:82)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 300 - Drop for item * JADE CARVING * - Input: DRO CAR
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 61| CAR |
| Condition| ConditionID 0 ArgID 82| item '\* JADE CARVING \*(index:82)' carried |
| Action| ActionID 53 ArgID 82| drops item '* JADE CARVING *(index:82)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 301 - Take for item * SAPPHIRE * - Input: GET SAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 65| SAP |
| Condition| ConditionID 1 ArgID 83| item '\* SAPPHIRE \*(index:83)' in room with player |
| Action| ActionID 52 ArgID 83| get item '* SAPPHIRE *(index:83)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 302 - Drop for item * SAPPHIRE * - Input: DRO SAP
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 65| SAP |
| Condition| ConditionID 0 ArgID 83| item '\* SAPPHIRE \*(index:83)' carried |
| Action| ActionID 53 ArgID 83| drops item '* SAPPHIRE *(index:83)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 303 - Take for item  * RUBY * - Input: GET RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 58| RUB |
| Condition| ConditionID 1 ArgID 90| item ' \* RUBY \*(index:90)' in room with player |
| Action| ActionID 52 ArgID 90| get item ' * RUBY *(index:90)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 304 - Drop for item  * RUBY * - Input: DRO RUB
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 58| RUB |
| Condition| ConditionID 0 ArgID 90| item ' \* RUBY \*(index:90)' carried |
| Action| ActionID 53 ArgID 90| drops item ' * RUBY *(index:90)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 305 - Take for item * PLATINUM CROWN * - Input: GET CRO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 25| CRO |
| Condition| ConditionID 1 ArgID 93| item '\* PLATINUM CROWN \*(index:93)' in room with player |
| Action| ActionID 52 ArgID 93| get item '* PLATINUM CROWN *(index:93)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 306 - Drop for item * PLATINUM CROWN * - Input: DRO CRO
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 25| CRO |
| Condition| ConditionID 0 ArgID 93| item '\* PLATINUM CROWN \*(index:93)' carried |
| Action| ActionID 53 ArgID 93| drops item '* PLATINUM CROWN *(index:93)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 307 - Take for item * EMERALD BRACELET * - Input: GET BRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 10| GET |
| Noun| 18| BRA |
| Condition| ConditionID 1 ArgID 97| item '\* EMERALD BRACELET \*(index:97)' in room with player |
| Action| ActionID 52 ArgID 97| get item '* EMERALD BRACELET *(index:97)', check if can carry |
| Action| ActionID 64 ArgID 0| look |
### Action 308 - Drop for item * EMERALD BRACELET * - Input: DRO BRA
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 18| DRO |
| Noun| 18| BRA |
| Condition| ConditionID 0 ArgID 97| item '\* EMERALD BRACELET \*(index:97)' carried |
| Action| ActionID 53 ArgID 97| drops item '* EMERALD BRACELET *(index:97)' into current room |
| Action| ActionID 64 ArgID 0| look |
### Action 309 - Manually added load game action - Input: LOA GAM
| Property| Value| Comment |
| --------| -----| ------- |
| Original values| |  |
| Verb| 49| LOA |
| Noun| 75| GAM |
| Action| ActionID 89 ArgID 0| Load Game |
## Words
### Verbs
| Word| Index| Aliases |
| ----| -----| ------- |
| AUT| 0|  |
| GO| 1| ENT, WAL, RUN, CLI |
| POU| 6| SPI, EMP |
| HEL| 9|  |
| GET| 10| TAK |
| REA| 12|  |
| BRE| 13|  |
| UNL| 14| OPE |
| SCO| 16|  |
| QUI| 17|  |
| DRO| 18| PUT, LEA |
| PET| 21|  |
| ATT| 22| KIL |
| SHO| 24|  |
| YES| 25|  |
| BUR| 26|  |
| DIG| 27|  |
| LIG| 28| FLA |
| LOO| 30| SEA |
| PLA| 32|  |
| BAL| 33|  |
| RUB| 34|  |
| PUL| 35| GRA |
| PLA| 37|  |
| CLO| 38| SHU |
| THR| 40|  |
| SAW| 41|  |
| WEA| 42|  |
| GLO| 43|  |
| DRI| 44|  |
| SAV| 45|  |
| INV| 46|  |
| DRA| 47|  |
| \.| 48|  |
| LOA| 49|  |
| SMO| 50|  |
| SWI| 51|  |
| JUM| 52|  |
| SHA| 53| ., SME, PUS, WAV |
| REM| 58|  |
| EAT| 59|  |
| WET| 60|  |
| ASK| 61| TAL, YEL, SAY, SCR, KIC, TIC |
| \.| 68|  |
| HUG| 69|  |
| UNC| 70|  |
| | 71|  |
| CLE| 72| WAS |
| | 74|  |
| FEE| 75| TOU, GRO |
| | 78|  |
| PUN| 79| HIT |
| | 81|  |
| | 82|  |
| | 83|  |
| | 84|  |
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
| WAT| 7| LIQ |
| SIG| 9|  |
| DOO| 10| BRI |
| POO| 12|  |
| SKE| 13|  |
| SAR| 14|  |
| BAN| 15|  |
| INV| 16|  |
| NOM| 17|  |
| BRA| 18|  |
| BON| 19|  |
| TAP| 20|  |
| LEA| 21|  |
| MUM| 22|  |
| ALC| 23|  |
| SKU| 24|  |
| CRO| 25|  |
| FLO| 26|  |
| HIE| 27|  |
| THR| 28|  |
| ROP| 29|  |
| PLA| 30|  |
| BLO| 31|  |
| BAS| 32|  |
| TEE| 33|  |
| GLO| 34|  |
| SAW| 35|  |
| LAD| 36|  |
| BOX| 37|  |
| CHA| 38|  |
| ARO| 39|  |
| OYS| 40|  |
| PEA| 41|  |
| FLU| 42|  |
| ARC| 43|  |
| PIS| 44|  |
| JER| 45|  |
| STO| 46| MAR |
| POL| 48|  |
| SHO| 49|  |
| NEC| 50|  |
| CAN| 51|  |
| RAT| 52|  |
| HOL| 53|  |
| COB| 54|  |
| ASH| 55|  |
| KEY| 56|  |
| EXP| 57|  |
| RUB| 58|  |
| POR| 59|  |
| PIN| 60|  |
| CAR| 61|  |
| STA| 62|  |
| WOR| 63|  |
| MIR| 64|  |
| SAP| 65|  |
| CHE| 66|  |
| MUR| 67|  |
| BAR| 68| WIN |
| \.| 70|  |
| COF| 71|  |
| COA| 72|  |
| COI| 73|  |
| PAS| 74|  |
| GAM| 75|  |
| TAB| 76|  |
| FLA| 77|  |
| STA| 78|  |
| ENT| 79|  |
| PYR| 80|  |
| HEA| 81|  |
| SCA| 82|  |
| FIR| 83|  |
| ALT| 84|  |
## Rooms
| Index| Description| Exits (RoomIDs) |
| -----| -----------| --------------- |
| 0| |  |
| 1| desert| South: 4, West: 2 |
| 2| desert| South: 3, East: 1 |
| 3| desert| North: 2, East: 4 |
| 4| desert next to a pyramid| North: 1, West: 3 |
| 5| hole| Up: 4 |
| 6| rocky entrance\-way| North: 12, South: 16 |
| 7| sarcophagus| West: 6, Down: 8 |
| 8| burial room| North: 9, South: 11, Up: 7 |
| 9| long, narrow passageway| South: 8 |
| 10| hidden alcove| West: 8 |
| 11| tall room| North: 8 |
| 12| dining hall| South: 6, East: 13 |
| 13| hallway| West: 12 |
| 14| round altar room| North: 13, South: 17, East: 15 |
| 15| hieroglyphics room| West: 14 |
| 16| sitting room| North: 6 |
| 17| sloping crawlway| North: 14 |
| 18| Revolving cavern| North: 19, South: 20, Down: 11 |
| 19| prison cell| South: 20, West: 18 |
| 20| \*I'm on a narrow ledge| South: 19, West: 18 |
| 21| throne room| Down: 20 |
| 22| treasure room| Down: 21 |
| 23| \*I'm on top of a pyramid| West: 22 |
| 24| Pool of water| East: 3 |
| 25| \.| North: 9, South: 9, East: 26, West: 9, Up: 9, Down: 9 |
| 26| dressing room| West: 25 |
| 27| lot of TROUBLE\!|  |
## Messages
| Index| Text |
| -----| ---- |
| 0|  |
| 1| I see something\. |
| 2| Bare\-handed? |
| 3| \. |
| 4| I can't\. |
| 5| No container\. |
| 6| Canteen is full\. |
| 7| Welcome to Adventure: 8 `PYRAMID OF DOOM` |
| 8| By Alvin Files & Scott Adams Dedicated to Ray Harshaw\! |
| 9| Sign: He who defiles the tombs of Egypt shall surely perish\! |
| 10| The sound of machinery\. |
| 11| I hear strange noises\! |
| 12| ARRGH\! Poison needle in the lock\. |
| 13| The right key could help \(maybe\)\. |
| 14| Large stone falls on me\! |
| 15| Something won't fit\. |
| 16| Noise scares them off |
| 17| Thanks\. |
| 18| Crash\!\!\! |
| 19| I hear a hollow laugh\. \. \. |
| 20| I don't see any reason to throw a  |
| 21| A small desert nomad appears\.\.\. |
| 22| The nomad stuck out his tongue at me\. |
| 23| What\! The nomad jumped me while my back was turned\! |
| 24| Nomad vanishes in a puff of yellow smoke\. |
| 25| Sorry, won't work\. |
| 26| Pistol has |
| 27| bullets |
| 28| No bullets\. |
| 29| Got him\!\! |
| 30| Too hot\. |
| 31| Mummy moves toward me\. |
| 32| Mummy has me by the throat\! |
| 33| Mummy |
| 34| won't let me |
| 35| You be weird\. Cut that out\. |
| 36| Doesn't bother him\. |
| 37| Cobra crawls out, presses a loose brick and then disappears intoa passage which appeared\. |
| 38| Something falls out\. |
| 39| \. |
| 40| \. |
| 41| Purple worm devours me\. |
| 42| Chain too tough\. |
| 43| Its black, dirty & dusty |
| 44| That feels good\. |
| 45| Rats |
| 46| Strange \. \. \. Nothing happens\. |
| 47| Its locked\. |
| 48| Skeleton places skull on his shoulders, grasps |
| 49| metal bar, pulls down ladder |
| 50| I can't reach it\. |
| 51| I'm not an arsonist\. |
| 52| It says: `LEAVE \*TREASURES\* HERE\!` |
| 53| Oyster makes a slobbering noise |
| 54| Oyster won't let me |
| 55| It attacks\! |
| 56| I just caught dengue fever\. Very bad\. |
| 57| Confusing\. Part appears missing\. |
| 58| I'm there\. |
| 59| Pour water? |
| 60| It's stuck\. |
| 61| \. |
| 62| Cobra |
| 63| Strange markings are present\. |
| 64| attacks\! |
| 65| Missed\.\.\. |
| 66| Liquid is acid\. |
| 67| Canteen dissolves\. |
| 68| Iron Statue |
| 69| Mural: Seek ye well the HEART of Iron\. |
| 70| Iron Statue tears me apart\! |
| 71| Ruby falls into pool of acid, burns up\. |
| 72| I see nothing special\. |
| 73| A tiny voice says: `SEARCH AND YE SHALL FIND\!` |
| 74| I can't lift it\. This is a big oyster |
| 75| I don't see it |
| 76| Nomad: `Look up decapitated\!` |
| 77| Nomad: `RUN YOU FOOL\!` |
| 78| Nomad: `Oyster thirsty?` |
| 79| Glove falls off my sweaty hand |
| 80| Ah, 'tis music to my ears\. |
| 81| OK |
| 82| Into the worm's mouth\! |
| 83| TRY: `TAKE INVENTORY` |
| 84| Mirrors EVERYWHERE\! Light blinds me, so I shut it OFF\! |
| 85| Pharoah's heart is red like yours, yet evil has darkened it\! |
| 86| WOW, man, crazy\.\.\. |
| 87| 1000 years bad luck starts with a cave in\! |
| 88| I feel a coin on the floor |
## Items
| Index| Description| GetDrop| RoomID |
| -----| -----------| -------| ------ |
| 0| | | 0 |
| 1| Stone| STO| 4 |
| 2| Door with large keyhole| | 0 |
| 3| Dried Camel Jerky| JER| 15 |
| 4| Empty canteen| CAN| 255 |
| 5| Full canteen| CAN| 0 |
| 6| Hole| | 0 |
| 7| Tiny locked door| | 5 |
| 8| Unlit flashlite| FLA| 255 |
| 9| Lit flashlite| FLA| 0 |
| 10| Wooden pole sticking from sand| | 0 |
| 11| Shovel| SHO| -1 |
| 12| Tiny key| KEY| 0 |
| 13| Lump of coal| COA| 0 |
| 14| Pool of liquid| | 3 |
| 15| Sign| | 4 |
| 16| Door with large keyhole| | 0 |
| 17| Open door| | 0 |
| 18| Large key| KEY| -1 |
| 19| I'm wearing an iron glove| | 0 |
| 20| Closed sarcophagus| | 6 |
| 21| Mouldy bandages| BAN| 6 |
| 22| Open sarcophagus| | 0 |
| 23| Stairs| | 7 |
| 24| Bones| BON| 0 |
| 25| Open door| | 6 |
| 26| Tiny open door| | 0 |
| 27| Small Nomad| | 0 |
| 28| Pistol| PIS| 6 |
| 29| Fearsome mummy| | 8 |
| 30| \* ANTIQUE TAPESTRY \*| TAP| 8 |
| 31| Burning tanna leaves| | 8 |
| 32| Enraged mummy| | 0 |
| 33| Sleeping mummy| | 0 |
| 34| \* GOLD SCARAB \*| SCA| 26 |
| 35| \.| | 0 |
| 36| Wet tanna leaves| LEA| 0 |
| 37| Entrance to an alcove| | 0 |
| 38| Bricked up doorway| | 9 |
| 39| Open door| | 0 |
| 40| \* GOLD COIN \*| COI| 0 |
| 41| Ashes| | 16 |
| 42| Basket| BAS| 16 |
| 43| Passageway behind fireplace| | 0 |
| 44| Open treasure coffer| | 0 |
| 45| Rope| ROP| 9 |
| 46|  | | 0 |
| 47| Chopping block| BLO| 10 |
| 48| Skull| SKU| 10 |
| 49| Box| BOX| 10 |
| 50| \* GOLD TEETH \*| TEE| 0 |
| 51| Iron glove| GLO| 0 |
| 52| Archway| | 13 |
| 53| Metal bar protruding from ceiling| | 11 |
| 54| Decapitated skeleton| | 11 |
| 55| Saw| SAW| 11 |
| 56| Fireplace| | 16 |
| 57|  | | 0 |
| 58| Ladder| | 0 |
| 59| Glowing skeleton| | 0 |
| 60| Table| TAB| 12 |
| 61|   | | 0 |
| 62|  | | 0 |
| 63| Giant Oyster| | 13 |
| 64| \* BLACK PEARL \*| PEA| 0 |
| 65| Flute| FLU| 13 |
| 66| Blood\-stained altar| | 14 |
| 67| \* PLATINUM BAR \*| BAR| 23 |
| 68| \* DIAMOND NECKLACE \*| NEC| 0 |
| 69| Satisfied rats| RAT| 0 |
| 70|  | | 0 |
| 71| Starving rats| RAT| 17 |
| 72|  | | 0 |
| 73| Hissing cobra| | 0 |
| 74| \* GOLD NECKLACE \*| NEC| 0 |
| 75| Passageway| | 0 |
| 76| Dead explorer chained to wall| | 19 |
| 77| Pile of Rubbish| | 19 |
| 78| Closed portal| | 19 |
| 79| Open portal| | 0 |
| 80| Purple Worm| | 0 |
| 81| \* GOLD PIN \*| PIN| 0 |
| 82| \* JADE CARVING \*| CAR| 0 |
| 83| \* SAPPHIRE \*| SAP| 20 |
| 84| Hole in the ceiling| | 20 |
| 85| Rope hanging from ceiling| | 0 |
| 86| Iron statue of Pharoah seated on throne| | 21 |
| 87| Chain hanging from ceiling| | 21 |
| 88| Chest| | 21 |
| 89| Wall Mural| | 21 |
| 90|  \* RUBY \*| RUB| 0 |
| 91| Pool of liquid \(far below ledge\)| | 20 |
| 92| Spiral Staircase| | 0 |
| 93| \* PLATINUM CROWN \*| CRO| 0 |
| 94| Standing iron statue| | 0 |
| 95| Iron Statue, slowly advancing\. \. \.| | 0 |
| 96| Pile of Melted iron| | 0 |
| 97| \* EMERALD BRACELET \*| BRA| 0 |
| 98| Open window| | 0 |
| 99| Treasure coffer| | 22 |
| 100| Barred window| | 22 |