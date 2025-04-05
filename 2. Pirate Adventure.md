# Pirate Adventure
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
### Action 0 - CROCODILES - Probability: 80
*Conditions*
```
item 'Fish(index:21)' in room with player
item 'Mean and hungry looking crocodiles(index:17)' in room with player
```
*Actions*
```
Print message 'Crocs eat fish and leave'
Item 'Fish(index:21' is removed from the game (put in room 0)
Item 'Mean and hungry looking crocodiles(index:17' is removed from the game (put in room 0)
```
### Action 1 - SNAKES - Probability: 80
*Conditions*
```
item 'Deadly mamba snakes(index:23)' in room with player
item 'Parrot(index:24)' in room with player
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Pieces of eight`'
Print message 'Parrot attacks snakes and drives them off'
Item 'Deadly mamba snakes(index:23' is removed from the game (put in room 0)
```
### Action 2 - RUG FLAG 11 GOT KEYS - Probability: 100
*Conditions*
```
item 'Rug(index:26)' carried
item 'Ring of keys(index:27)' not carried or in room with player
bitflag 11 is false
```
*Actions*
```
Print message 'There's a strange sound'
drops item 'Ring of keys(index:27' into current room
set 11 flag
```
### Action 3 - PARROT PIECES 8 - Probability: 3
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Pieces of eight`'
```
### Action 4 - LITE - Probability: 100
*Conditions*
```
player in room 14
bitflag 15 is set
```
*Actions*
```
clear darkness flag
look
```
### Action 5 - FLAG 1. BUILD BOAT. NEED SAIL/LUMBER/BEACH - Probability: 100
*Conditions*
```
bitflag 1 is set
item 'Pile of precut lumber(index:33)' carried or in room with player
item 'Pile of sails(index:20)' carried or in room with player
```
*Actions*
```
set 2 flag
```
### Action 6 - FLAG 2.READY TO BUILD BOAT - Probability: 100
*Conditions*
```
bitflag 2 is set
```
*Actions*
```
set 1 flag
Item 'Pile of precut lumber(index:33' is removed from the game (put in room 0)
swap item locations 'Pirate ship(index:37)' and 'Small ship's keel and mast(index:11)'
Print message 'CONGRATULATIONS \!\!\! But your Adventure is not over yet\.\.\. '
```
### Action 7 - NOT READY TO BUILD - Probability: 100
*Conditions*
```
bitflag 1 is set
```
*Actions*
```
Print message 'No, something is missing\!'
set 1 flag
```
### Action 8 - UNLOCK DOOR. FLAG 0 - Probability: 100
*Conditions*
```
bitflag 0 is set
```
*Actions*
```
swap item locations 'Locked door(index:35)' and 'Open door with pit beyond(index:36)'
Set bit 0 false
```
### Action 9 - BUILDINg BOAT - Probability: 100
*Conditions*
```
bitflag 2 is set
```
*Actions*
```
set 2 flag
Item 'Nails(index:32' is removed from the game (put in room 0)
Item 'Pile of sails(index:20' is removed from the game (put in room 0)
Item 'Rusty anchor(index:15' is removed from the game (put in room 0)
```
### Action 10 - END GAME - Probability: 19
*Conditions*
```
player in room 26
```
*Actions*
```
score
Print message 'Since nothing is happening'
game over
```
### Action 11 - SLIPPED NO SHOES - Probability: 40
*Conditions*
```
player in room 5
item 'Safety sneakers(index:44)' not carried
```
*Actions*
```
Print message 'I slipped and fell\.\.\.'
Death, clear dark flag, move to last room
```
### Action 12 - PIRATE RUM FLAG 0 - Probability: 80
*Conditions*
```
item 'Wicked looking pirate(index:12)' in room with player
item 'Bottle of rum(index:25)' in room with player
```
*Actions*
```
item 'Sleeping pirate(index:41)' is moved to room 4
Print message 'Pirate grabs rum and scuttles off chortling'
Set bit 0 true
Item 'Wicked looking pirate(index:12' is removed from the game (put in room 0)
```
### Action 13 - PIRATE RUM ATTIC FLAG 0 - Probability: 100
*Conditions*
```
bitflag 0 is set
```
*Actions*
```
Set bit 0 false
item 'Empty bottle(index:7)' is moved to room 4
Item 'Bottle of rum(index:25' is removed from the game (put in room 0)
```
### Action 14 - FISH ESCAPE - Probability: 25
*Conditions*
```
item 'Fish(index:21)' carried
item 'Bottle of salt water(index:42)' not carried
```
*Actions*
```
Print message 'Too dry, fish vanish\.'
item 'Fish(index:21)' is moved to room 10
```
### Action 15 - FLAG 6 INTRO - Probability: 100
*Conditions*
```
bitflag 6 is false
```
*Actions*
```
Print message '\* Welcome to Adventure number 2: `pirate adventure` by Alexis & Scott Adams, dedicated: Ted Heeren & Paul Sharland Remember you can always ask for `help`\. '
set 6 flag
```
### Action 16 - PIRATE RUM AGAIN - Probability: 50
*Conditions*
```
item 'Wicked looking pirate(index:12)' in room with player
item 'Bottles of rum(index:49)' in room with player
```
*Actions*
```
item 'Sleeping pirate(index:41)' is moved to room 22
Print message 'Pirate grabs rum and scuttles off chortling'
Item 'Wicked looking pirate(index:12' is removed from the game (put in room 0)
```
### Action 17 - PARROT BAG - Probability: 35
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
bitflag 3 is false
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Check the bag matey`'
```
### Action 18 - PARROT CHEST - Probability: 7
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
bitflag 12 is false
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Check the chest matey`'
```
### Action 19 - TIDE IN DROWN - Probability: 50
*Conditions*
```
player in room 24
item 'The tide is coming in(index:53)' in game
item 'Water wings(index:54)' not carried
```
*Actions*
```
Print message 'The tide is coming in'
Print message 'I'm underwater, I guess I don't swim well\. Blub Blub\.\.\.'
Death, clear dark flag, move to last room
```
### Action 20 - DROWN OCEAN - Probability: 50
*Conditions*
```
player in room 10
item 'Water wings(index:54)' not carried
```
*Actions*
```
Print message 'I'm underwater, I guess I don't swim well\. Blub Blub\.\.\.'
Death, clear dark flag, move to last room
```
### Action 21 - TIDE WITH ANCHOR - Probability: 10
*Conditions*
```
bitflag 10 is false
```
*Actions*
```
swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)'
swap item locations 'Rusty anchor(index:15)' and 'Flotsam and jetsam(index:55)'
Set bit 0 true
```
### Action 22 - TIDE NO ANCHOR NOT T.I. - Probability: 10
*Conditions*
```
bitflag 10 is set
bitflag 4 is false
```
*Actions*
```
swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)'
Set bit 0 true
```
### Action 23 - PARROT TIDE - Probability: 100
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
bitflag 0 is set
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Tides be a changing matey`'
Set bit 0 false
```
### Action 24 - RESET FLAG 0 - Probability: 100
*Conditions*
```
bitflag 0 is set
```
*Actions*
```
Set bit 0 false
```
### Action 25 - LITE - Probability: 100
*Conditions*
```
player in room 5
bitflag 15 is set
```
*Actions*
```
clear darkness flag
look
```
### Action 26 - MONGOOSE - Probability: 80
*Conditions*
```
item 'Deadly mamba snakes(index:23)' in room with player
item 'Mongoose(index:14)' in room with player
```
*Actions*
```
Print message 'I was wrong, I guess its not a mongoose cause the snakes bit it\!'
swap item locations 'Mongoose(index:14)' and 'Dead squirrel(index:58)'
```
### Action 27 - BIRD & CROCS - Probability: 80
*Conditions*
```
item 'Mean and hungry looking crocodiles(index:17)' in room with player
item 'Parrot(index:24)' in room with player
```
*Actions*
```
Print message 'Parrot attacks crocs but is beaten off'
Print message 'Bird flys off looking very unhappy'
item 'Parrot(index:24)' is moved to room 13
```
### Action 28 - BIRD FOLLOWS CRACKERS - Probability: 30
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
item 'Sack of crackers(index:60)' not carried or in room with player
item 'Wicked looking pirate(index:12)' not carried or in room with player
```
*Actions*
```
Print message 'Bird flys off looking very unhappy'
put item 1 'Parrot(index:24)' with item2 'Sack of crackers(index:60)'
```
### Action 29 - PARROT EAT CRACKS - Probability: 20
*Conditions*
```
item 'Parrot(index:24)' carried or in room with player
item 'Sack of crackers(index:60)' carried or in room with player
```
*Actions*
```
Print message 'Parrot ate a cracker\.'
```
### Action 30 - PARROT BOOK - Probability: 25
*Conditions*
```
item 'Note(index:61)' not in game
item 'Parrot(index:24)' carried or in room with player
item 'Large blood soaked book(index:3)' carried or in room with player
```
*Actions*
```
Print message 'The Parrot crys:'
Print message '`Check the book, matey\!`'
```
### Action 31 - BURNT LAMP - Probability: 100
*Conditions*
```
bitflag 16 is set
```
*Actions*
```
swap item locations 'Burnt out torch(index:63)' and 'Lit torch(index:9)'
set 16 flag
look
```
### Action 32 - Input: SAY YOH
*Conditions*
```
player not in room 5
item 'Large blood soaked book(index:3)' carried
```
*Actions*
```
clear screen
Print message 'Everything spins around and suddenly I'm elsewhere\.\.\.'
move room 5
look
```
### Action 33 - NO SAIL WITH BOOK - Input: SET SAI
*Conditions*
```
player in room 20
item 'Wicked looking pirate(index:12)' in room with player
item 'Large blood soaked book(index:3)' carried or in room with player
item 'Map(index:45)' carried or in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Pirate says: `First Yee be getting that ACCURSED thing off me ship\!` '
```
### Action 34 - Input: LIG TOR
*Conditions*
```
item 'Unlit torch(index:8)' carried or in room with player
item 'Matches(index:10)' carried or in room with player
```
*Actions*
```
swap item locations 'Unlit torch(index:8)' and 'Lit torch(index:9)'
clear screen
Print message 'Torch is lit'
look
```
### Action 35 - Input: UNL TOR
*Conditions*
```
item 'Lit torch(index:9)' carried or in room with player
```
*Actions*
```
swap item locations 'Lit torch(index:9)' and 'Unlit torch(index:8)'
Print message 'OK'
look
```
### Action 36 - Input: HEL ANY
*Conditions*
```
player in room 5
```
*Actions*
```
Print message 'I may need to say a MAGIC word here\!'
```
### Action 37 - Input: GET DUB
*Conditions*
```
item '\*DUBLEONS\*(index:22)' in room with player
item 'Deadly mamba snakes(index:23)' not in room with player
```
*Actions*
```
get item '*DUBLEONS*(index:22', check if can carry
Print message 'OK'
```
### Action 38 - Input: GET DUB
*Conditions*
```
item '\*DUBLEONS\*(index:22)' in room with player
item 'Deadly mamba snakes(index:23)' in room with player
```
*Actions*
```
Print message 'That's not very smart'
Print message 'I'm snake bit'
Death, clear dark flag, move to last room
```
### Action 39 - Input: GO SHA
*Conditions*
```
item 'Grass shack(index:16)' in room with player
```
*Actions*
```
move room 9
clear screen
look
```
### Action 40 - Input: GET CHE
*Conditions*
```
item 'Treasure chest(index:13)' in room with player
item 'Wicked looking pirate(index:12)' in room with player
```
*Actions*
```
Print message 'Pirate won't let me'
```
### Action 41 - . - Input: GET CHE
*Conditions*
```
item 'Treasure chest(index:13)' in room with player
item 'Wicked looking pirate(index:12)' not in room with player
```
*Actions*
```
get item 'Treasure chest(index:13', check if can carry
Print message 'OK'
```
### Action 42 - Input: OPE CHE
*Conditions*
```
item 'Treasure chest(index:13)' in room with player
item 'Wicked looking pirate(index:12)' in room with player
```
*Actions*
```
Print message 'Pirate won't let me'
```
### Action 43 - Input: OPE CHE
*Conditions*
```
item 'Treasure chest(index:13)' in room with player
item 'Wicked looking pirate(index:12)' not in room with player
```
*Actions*
```
Print message 'Its locked'
```
### Action 44 - Input: UNL CHE
*Conditions*
```
item 'Treasure chest(index:13)' in room with player
item 'Wicked looking pirate(index:12)' not in room with player
item 'Ring of keys(index:27)' carried
```
*Actions*
```
Print message 'Its open'
Item 'Treasure chest(index:13' is removed from the game (put in room 0)
drops item 'Open treasure chest(index:28' into current room
```
### Action 45 - Input: OPE CHE
*Conditions*
```
item 'Treasure chest(index:13)' carried
```
*Actions*
```
Print message 'Not while I'm carrying it'
```
### Action 46 - Input: LOO CHE
*Conditions*
```
item 'Open treasure chest(index:28)' carried
```
*Actions*
```
Print message 'Not while I'm carrying it'
```
### Action 47 - Input: LOO CHE
*Conditions*
```
item 'Treasure chest(index:13)' carried or in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its locked'
```
### Action 48 - FLAG 12 CHEST EMPTY - Input: LOO CHE
*Conditions*
```
item 'Open treasure chest(index:28)' in room with player
bitflag 5 is false
bitflag 12 is false
```
*Actions*
```
Print message 'There are a set of plans in it'
drops item 'Set of plans(index:29' into current room
set 5 flag
```
### Action 49 - CHEST MAP - Input: LOO CHE
*Conditions*
```
bitflag 12 is false
item 'Open treasure chest(index:28)' in room with player
bitflag 5 is set
```
*Actions*
```
Print message 'There's a map in it'
drops item 'Map(index:45' into current room
set 12 flag
```
### Action 50 - EMPTY - Input: LOO CHE
*Conditions*
```
bitflag 12 is set
item 'Open treasure chest(index:28)' in room with player
```
*Actions*
```
Print message 'Its empty'
```
### Action 51 - Input: LOO BAG
*Conditions*
```
item 'Pirate's duffel bag(index:5)' carried or in room with player
bitflag 3 is false
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'open it?'
```
### Action 52 - Input: LOO BAG
*Conditions*
```
item 'Pirate's duffel bag(index:5)' carried or in room with player
bitflag 3 is set
```
*Actions*
```
Print message 'Its empty'
```
### Action 53 - Input: OPE DOO
*Conditions*
```
item 'Mean and hungry looking crocodiles(index:17)' in room with player
```
*Actions*
```
Print message 'Crocs stop me'
```
### Action 54 - Input: OPE DOO
*Conditions*
```
item 'Locked door(index:18)' in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its locked'
```
### Action 55 - Input: OPE DOO
*Conditions*
```
item 'Open door with hall beyond(index:19)' in room with player
```
*Actions*
```
Print message 'Its open'
```
### Action 56 - Input: GO HAL
*Conditions*
```
item 'Open door with hall beyond(index:19)' in room with player
```
*Actions*
```
move room 16
clear screen
look
```
### Action 57 - Input: UNL DOO
*Conditions*
```
item 'Mean and hungry looking crocodiles(index:17)' in room with player
item 'Locked door(index:18)' in room with player
```
*Actions*
```
Print message 'Crocs stop me'
```
### Action 58 - Input: UNL DOO
*Conditions*
```
item 'Mean and hungry looking crocodiles(index:17)' not in room with player
item 'Locked door(index:18)' in room with player
item 'Ring of keys(index:27)' carried
```
*Actions*
```
Item 'Locked door(index:18' is removed from the game (put in room 0)
drops item 'Open door with hall beyond(index:19' into current room
Set bit 0 true
Print message 'OK'
```
### Action 59 - Input: DRI BOT
*Conditions*
```
item 'Bottle of rum(index:25)' carried or in room with player
```
*Actions*
```
Print message 'Yummy'
Print message 'There's a strange sound'
Print message '\.\.\.I think its me, Hee Hee\.'
```
### Action 60 - Input: INV ANY
*Actions*
```
output inventory
```
### Action 61 - Input: GET INV
*Actions*
```
output inventory
```
### Action 62 - Input: LOO BOX
*Conditions*
```
item 'Wooden box(index:57)' carried or in room with player
item '\*RARE STAMPS\*(index:50)' not carried or in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'open it?'
```
### Action 63 - Input: SAY AWA
*Actions*
```
Print message 'Wrong game you silly goose\!'
Print message 'Nothing happens'
```
### Action 64 - Input: REA BOO
*Conditions*
```
item 'Large blood soaked book(index:3)' not carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'I don't have it'
```
### Action 65 - Input: SCO ANY
*Actions*
```
score
```
### Action 66 - Input: SAV GAM
*Actions*
```
save game
```
### Action 67 - . - Input: BUI BOA
*Conditions*
```
item 'Set of plans(index:29)' not carried or in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'I've no plans\!'
```
### Action 68 - Input: GO CAV
*Conditions*
```
player in room 14
```
*Actions*
```
move room 7
set darkness flag
clear screen
look
```
### Action 69 - Input: LOO LAG
*Conditions*
```
item 'The tide is out(index:52)' not in game
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
Print message 'The tide is coming in'
```
### Action 70 - TIDE OUT - Input: LOO LAG
*Conditions*
```
item 'The tide is out(index:52)' in game
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
Print message 'The tide is out'
```
### Action 71 - Input: LOO SHA
*Conditions*
```
item 'Grass shack(index:16)' in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
```
### Action 72 - Input: LOO CRA
*Conditions*
```
item 'Rock wall with narrow crack in it(index:38)' in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
```
### Action 73 - CARRYING SHOVEL - Input: GO CRA
*Conditions*
```
item 'Narrow crack in the rock(index:39)' in room with player
item 'Shovel(index:46)' carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Something won't fit'
```
### Action 74 - CARRYING CHEST - Input: GO CRA
*Conditions*
```
item 'Rock wall with narrow crack in it(index:38)' in room with player
item 'Treasure chest(index:13)' carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Something won't fit'
```
### Action 75 - Input: QUI ANY
*Actions*
```
game over
```
### Action 76 - Input: GET RUG
*Conditions*
```
item 'Rug(index:30)' in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its nailed to the floor\!'
```
### Action 77 - Input: GET NAI
*Conditions*
```
item 'Claw hammer(index:31)' carried
item 'Rug(index:30)' in room with player
```
*Actions*
```
get item 'Nails(index:32', check if can carry
drops item 'Rug(index:26' into current room
Item 'Rug(index:30' is removed from the game (put in room 0)
Print message 'OK'
```
### Action 78 - CARRYING LUMBER - Input: GO CRA
*Conditions*
```
item 'Narrow crack in the rock(index:39)' in room with player
item 'Pile of precut lumber(index:33)' carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Something won't fit'
```
### Action 79 - Input: BUI BOA
*Conditions*
```
item 'Claw hammer(index:31)' carried or in room with player
item 'Set of plans(index:29)' carried or in room with player
item 'Rusty anchor(index:15)' carried or in room with player
item 'Nails(index:32)' carried or in room with player
```
*Actions*
```
set 1 flag
```
### Action 80 - Input: BUI BOA
*Actions*
```
Print message 'No, something is missing\!'
```
### Action 81 - Input: GO PIT
*Conditions*
```
item 'Open door with pit beyond(index:36)' in room with player
```
*Actions*
```
clear screen
move room 11
look
```
### Action 82 - CARRYING BOOK - Input: GO CRA
*Conditions*
```
item 'Rock wall with narrow crack in it(index:38)' in room with player
item 'Large blood soaked book(index:3)' carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Something won't fit'
```
### Action 83 - Input: SAY YOH
*Conditions*
```
player in room 5
item 'Large blood soaked book(index:3)' carried
```
*Actions*
```
clear screen
Print message 'Everything spins around and suddenly I'm elsewhere\.\.\.'
move room 6
look
```
### Action 84 - Input: GET RUG
*Conditions*
```
item 'Rug(index:26)' carried or in room with player
```
*Actions*
```
get item 'Rug(index:26', check if can carry
Print message 'OK'
```
### Action 85 - DARK - Input: GO CRA
*Conditions*
```
item 'Rock wall with narrow crack in it(index:38)' in room with player
```
*Actions*
```
move room 17
Print message 'It was a tight squeeze\!'
set darkness flag
look
```
### Action 86 - LITE - Input: GO CRA
*Conditions*
```
item 'Narrow crack in the rock(index:39)' in room with player
```
*Actions*
```
move room 18
clear darkness flag
clear screen
look
```
### Action 87 - WAIT FOR FOR TIDE - Input: SET SAI
*Conditions*
```
player in room 20
item 'Wicked looking pirate(index:12)' in room with player
item 'The tide is out(index:52)' in game
bitflag 4 is false
```
*Actions*
```
Print message 'Pirate says: `Aye me Buckeroo, we be waiting for the tide to come in\!`'
```
### Action 88 - Probability: 0
### Action 89 - FLAG 3 EMPTY BAG - Input: OPE BAG
*Conditions*
```
item 'Pirate's duffel bag(index:5)' carried or in room with player
bitflag 3 is false
```
*Actions*
```
Print message 'Something falls out'
drops item 'Matches(index:10' into current room
set 3 flag
```
### Action 90 - Input: OPE BAG
*Conditions*
```
bitflag 3 is set
```
*Actions*
```
Print message 'Nothing happens'
Print message 'Its empty'
```
### Action 91 - Input: GET WAT
*Conditions*
```
item 'Empty bottle(index:7)' not carried
```
*Actions*
```
Print message 'I've no container'
```
### Action 92 - Input: GET WAT
*Conditions*
```
item 'Salt water(index:40)' in room with player
item 'Empty bottle(index:7)' carried
```
*Actions*
```
Item 'Empty bottle(index:7' is removed from the game (put in room 0)
get item 'Bottle of salt water(index:42', check if can carry
Print message 'OK'
```
### Action 93 - Input: DRO WAT
*Conditions*
```
item 'Bottle of salt water(index:42)' carried
```
*Actions*
```
Item 'Bottle of salt water(index:42' is removed from the game (put in room 0)
get item 'Empty bottle(index:7', check if can carry
Print message 'It soaks into the ground'
```
### Action 94 - Input: DRI WAT
*Conditions*
```
item 'Salt water(index:40)' in room with player
```
*Actions*
```
Print message 'That's not very smart'
Death, clear dark flag, move to last room
```
### Action 95 - Input: DRI WAT
*Conditions*
```
item 'Bottle of salt water(index:42)' carried
```
*Actions*
```
Print message 'That's not very smart'
Death, clear dark flag, move to last room
Item 'Bottle of salt water(index:42' is removed from the game (put in room 0)
get item 'Empty bottle(index:7', check if can carry
```
### Action 96 - Input: WAK PIR
*Conditions*
```
item 'Sleeping pirate(index:41)' in room with player
```
*Actions*
```
Print message 'Pirate awakens and says `Aye matey we be casting off soon` He then VANISHES\!'
Item 'Sleeping pirate(index:41' is removed from the game (put in room 0)
item 'Wicked looking pirate(index:12)' is moved to room 20
```
### Action 97 - Input: OPE BOT
*Conditions*
```
item 'Bottle of rum(index:25)' carried or in room with player
```
*Actions*
```
Print message 'Its open'
```
### Action 98 - Input: EMP BOT
*Conditions*
```
item 'Bottle of rum(index:25)' carried or in room with player
```
*Actions*
```
Print message 'What a waste\.\.\.'
Print message 'It soaks into the ground'
swap item locations 'Bottle of rum(index:25)' and 'Empty bottle(index:7)'
```
### Action 99 - Input: GO BOA
*Conditions*
```
item 'Pirate ship(index:37)' in room with player
```
*Actions*
```
move room 20
clear screen
look
```
### Action 100 - FLAG 4 WE AT TREASUE ISLE - Input: GO SHO
*Conditions*
```
player in room 20
bitflag 4 is set
item 'Wicked looking pirate(index:12)' in room with player
```
*Actions*
```
move room 21
clear screen
drops item 'Wicked looking pirate(index:12' into current room
Print message 'Pirate follows me ashore as if expecting something'
```
### Action 101 - Input: GO SHO
*Conditions*
```
player in room 20
bitflag 4 is false
```
*Actions*
```
move room 6
clear screen
look
```
### Action 102 - . - Input: SET SAI
*Conditions*
```
player in room 20
item 'Wicked looking pirate(index:12)' not in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'I've no crew'
```
### Action 103 - Input: SET SAI
*Conditions*
```
player in room 20
item 'Map(index:45)' not carried or in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Pirate says: `Aye matey we be needing a map first`\.'
```
### Action 104 - GO TREASURE ISLE - Input: SET SAI
*Conditions*
```
player in room 20
bitflag 4 is false
```
*Actions*
```
clear screen
Print message 'After a day at sea we set anchor off of a sandy beach\. All Ashore who's going Ashore\.\.\.'
set 4 flag
item 'Pirate ship(index:37)' is moved to room 21
```
### Action 105 - RETURN FROM TR ISLE - Input: SET SAI
*Conditions*
```
player in room 20
bitflag 4 is set
```
*Actions*
```
clear screen
Print message 'After a day at sea we set anchor off of a sandy beach\. All Ashore who's going Ashore\.\.\.'
set 4 flag
item 'Pirate ship(index:37)' is moved to room 6
```
### Action 106 - Input: CAS OFF
*Actions*
```
Print message 'Try: `WEIGH ANCHOR`'
```
### Action 107 - Input: REA MAP
*Conditions*
```
item 'Map(index:45)' carried or in room with player
```
*Actions*
```
Print message 'Its a map to Treasure Island\. At the bottom it says: `30 paces then dig\!`'
```
### Action 108 - Input: SAI ANY
*Actions*
```
Print message 'Try: `WEIGH ANCHOR`'
```
### Action 109 - Input: GET BOO
*Conditions*
```
item 'Large blood soaked book(index:3)' in room with player
```
*Actions*
```
get item 'Large blood soaked book(index:3', check if can carry
Print message 'OK'
```
### Action 110 - Input: OPE BOO
*Conditions*
```
item 'Large blood soaked book(index:3)' carried or in room with player
item 'Small advertising flyer(index:62)' not in game
```
*Actions*
```
drops item 'Small advertising flyer(index:62' into current room
Print message 'OK'
Print message 'Something falls out'
```
### Action 111 - AT T.I. - Input: GO SHO
*Conditions*
```
player in room 20
bitflag 4 is set
```
*Actions*
```
move room 21
clear screen
look
```
### Action 112 - Input: GO PAT
*Conditions*
```
player in room 14
```
*Actions*
```
move room 18
clear screen
look
```
### Action 113 - Input: GET PAR
*Conditions*
```
item 'Parrot(index:24)' in room with player
item 'Wicked looking pirate(index:12)' in room with player
```
*Actions*
```
Print message 'Pirate won't let me'
```
### Action 114 - Input: GET PAR
*Conditions*
```
item 'Parrot(index:24)' in room with player
```
*Actions*
```
get item 'Parrot(index:24', check if can carry
Print message 'The Parrot crys:'
Print message '`Pieces of eight`'
```
### Action 115 - Input: GO SHE
*Conditions*
```
item 'Tool shed(index:34)' in room with player
```
*Actions*
```
move room 15
clear screen
look
```
### Action 116 - FLAG 7. THIS IS IT - Input: GO 30
*Conditions*
```
player in room 23
```
*Actions*
```
set 7 flag
Print message 'OK I walked off 30 paces\.'
```
### Action 117 - PACE 30 BUT WRONG PLACE - Input: GO 30
*Actions*
```
set 7 flag
Print message 'OK I walked off 30 paces\.'
```
### Action 118 - BONES - Input: DIG ANY
*Conditions*
```
player in room 22
item 'Shovel(index:46)' carried
item 'Mouldy old bones(index:47)' not in game
```
*Actions*
```
clear screen
Print message 'I found something\!'
drops item 'Mouldy old bones(index:47' into current room
look
```
### Action 119 - EAT CRACKERRS - Input: DRI CRA
*Conditions*
```
item 'Sack of crackers(index:60)' carried or in room with player
```
*Actions*
```
Print message 'Yummy'
```
### Action 120 - BEACH TREASURE RUM - Input: DIG ANY
*Conditions*
```
player in room 21
item 'Bottles of rum(index:49)' not in game
item 'Shovel(index:46)' carried
```
*Actions*
```
clear screen
drops item 'Bottles of rum(index:49' into current room
Print message 'I found something\!'
look
```
### Action 121 - Input: JUM ANY
*Conditions*
```
player in room 5
```
*Actions*
```
clear screen
Print message 'That's not very smart'
Death, clear dark flag, move to last room
```
### Action 122 - GOT IT - Input: DIG ANY
*Conditions*
```
player in room 23
bitflag 7 is set
item 'Shovel(index:46)' carried
item 'Wooden box(index:57)' not in game
```
*Actions*
```
clear screen
drops item 'Wooden box(index:57' into current room
Print message 'I found something\!'
look
```
### Action 123 - Input: GET NAI
*Conditions*
```
item 'Nails(index:32)' carried or in room with player
```
*Actions*
```
get item 'Nails(index:32', check if can carry
Print message 'OK'
```
### Action 124 - Input: GO WIN
*Conditions*
```
player in room 5
```
*Actions*
```
move room 2
clear screen
look
```
### Action 125 - Input: HEL ANY
*Conditions*
```
player in room 2
```
*Actions*
```
Print message 'Reading expands the mind'
Print message 'I may need to say a MAGIC word here\!'
```
### Action 126 - Input: REA PLA
*Conditions*
```
item 'Set of plans(index:29)' carried or in room with player
```
*Actions*
```
Print message 'They're plans to build the Jolly Roger \(a Pirate ship\!\) You'll need: hammer, nails, lumber, anchor, sails, and a keel\.'
```
### Action 127 - Input: UNL DOO
*Conditions*
```
item 'Locked door(index:35)' in room with player
item 'Ring of keys(index:27)' carried
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its locked'
Print message 'from the other side\!'
```
### Action 128 - Input: OPE DOO
*Conditions*
```
item 'Locked door(index:35)' in room with player
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its locked'
```
### Action 129 - Input: OPE DOO
*Conditions*
```
item 'Open door with pit beyond(index:36)' in room with player
```
*Actions*
```
Print message 'Its open'
```
### Action 130 - Input: GO LAG
*Conditions*
```
item 'Lagoon(index:51)' in room with player
```
*Actions*
```
move room 24
clear screen
look
```
### Action 131 - Input: GO STA
*Conditions*
```
item 'Flight of stairs(index:0)' in room with player
player in room 1
```
*Actions*
```
move room 2
clear screen
look
```
### Action 132 - Input: GET BOO
*Conditions*
```
player in room 2
item 'Bookcase with secret passage beyond(index:4)' not in room with player
```
*Actions*
```
get item 'Large blood soaked book(index:3', check if can carry
Print message 'There's a strange sound'
swap item locations 'Books in a bookcase(index:2)' and 'Bookcase with secret passage beyond(index:4)'
```
### Action 133 - Input: GET ANC
*Conditions*
```
item 'Rusty anchor(index:15)' in room with player
bitflag 10 is set
```
*Actions*
```
get item 'Rusty anchor(index:15', check if can carry
Print message 'OK'
```
### Action 134 - Input: GET ANC
*Conditions*
```
item 'Rusty anchor(index:15)' in room with player
bitflag 10 is false
```
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its stuck in the sand'
```
### Action 135 - Input: GET ANC
*Conditions*
```
item 'Rusty anchor(index:15)' not in room with player
```
*Actions*
```
clear screen
Print message 'Sorry I can't'
Print message 'I don't see it here'
look
```
### Action 136 - DROP SALT WATER - Input: EMP BOT
*Conditions*
```
item 'Bottle of salt water(index:42)' carried or in room with player
```
*Actions*
```
swap item locations 'Bottle of salt water(index:42)' and 'Empty bottle(index:7)'
Print message 'OK'
```
### Action 137 - Input: GO MON
*Conditions*
```
item 'Monastary(index:56)' in room with player
```
*Actions*
```
move room 25
clear screen
look
```
### Action 138 - Input: SAI BOA
*Actions*
```
Print message 'Try: `WEIGH ANCHOR`'
```
### Action 139 - . - Input: HEL ANY
*Conditions*
```
player in room 14
```
*Actions*
```
Print message 'There's multiple exits here\!'
```
### Action 140 - Input: WEI ANC
*Actions*
```
Print message 'About 20 pounds\. Try: `SET SAIL`'
```
### Action 141 - FREE ANCHOR FLAG 10 - Input: DIG ANY
*Conditions*
```
item 'Shovel(index:46)' carried
bitflag 10 is false
item 'Rusty anchor(index:15)' in room with player
```
*Actions*
```
set 10 flag
Print message 'OK'
```
### Action 142 - Input: BUR ANY
*Actions*
```
Print message 'Sorry I can't'
```
### Action 143 - Input: OPE BOX
*Conditions*
```
item 'Claw hammer(index:31)' carried
item 'Wooden box(index:57)' carried or in room with player
```
*Actions*
```
Print message 'Something falls out'
drops item '*RARE STAMPS*(index:50' into current room
```
### Action 144 - Input: KIL PIR
*Actions*
```
Print message 'Pirate won't let me'
```
### Action 145 - Input: HEL ANY
*Conditions*
```
item 'Mean and hungry looking crocodiles(index:17)' in room with player
```
*Actions*
```
Print message 'Got anything to eat matey?'
```
### Action 146 - Input: SAY ANY
*Actions*
```
Print message 'OK'
echo noun
Print message 'Nothing happens'
```
### Action 147 - Input: HEL ANY
*Conditions*
```
player in room 6
```
*Actions*
```
Print message 'There's multiple exits here\!'
```
### Action 148 - Input: WAI ANY
*Conditions*
```
bitflag 10 is set
```
*Actions*
```
swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)'
Print message '`Tides be a changing matey`'
```
### Action 149 - Input: HEL ANY
*Conditions*
```
player in room 9
item 'Wicked looking pirate(index:12)' in room with player
```
*Actions*
```
Print message 'Yoho ho and a \.\.\.'
```
### Action 150 - Input: DIG ANY
*Conditions*
```
item 'Shovel(index:46)' carried
```
*Actions*
```
Print message 'I didn't find anything'
set 7 flag
```
### Action 151 - Input: HEL ANY
*Conditions*
```
player in room 1
```
*Actions*
```
Print message 'Climb stairs\.\.\.'
```
### Action 152 - Input: GO PAS
*Conditions*
```
item 'Bookcase with secret passage beyond(index:4)' in room with player
```
*Actions*
```
move room 3
clear screen
look
```
### Action 153 - Input: REA BOO
*Conditions*
```
item 'Large blood soaked book(index:3)' carried or in room with player
```
*Actions*
```
Print message 'The book is in bad condtion but I can make out the title: `Treasure Island`\. There's a word written in blood in the flyleaf: `YOHO` and a message:  `Long John Silver left 2 treasures on Treasure Island`'
```
### Action 154 - Input: DRI ANY
*Actions*
```
Print message 'Sorry I can't'
```
### Action 155 - . - Input: HEL ANY
*Actions*
```
Print message 'Nothing happens'
```
### Action 156 - Input: GO WIN
*Conditions*
```
item 'Open window(index:1)' in room with player
```
*Actions*
```
move room 5
clear screen
look
```
### Action 157 - Input: FIN ANY
*Actions*
```
Print message 'Sorry I can't'
Print message 'I don't know where to look\!'
```
### Action 158 - Input: LIS ANY
*Actions*
```
Print message 'I hear nothing now'
```
### Action 159 - Input: GET CHE
*Conditions*
```
item 'Open treasure chest(index:28)' carried or in room with player
```
*Actions*
```
get item 'Open treasure chest(index:28', check if can carry
Print message 'OK'
```
### Action 160 - Input: OPE BOO
*Conditions*
```
item 'Small advertising flyer(index:62)' in game
item 'Large blood soaked book(index:3)' carried or in room with player
item 'Note(index:61)' not in game
```
*Actions*
```
Print message 'OK'
drops item 'Note(index:61' into current room
Print message 'Something falls out'
```
### Action 161 - Input: LOO BOO
*Conditions*
```
item 'Large blood soaked book(index:3)' carried or in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'read it?'
Print message 'open it?'
```
### Action 162 - Input: REA NOT
*Conditions*
```
item 'Note(index:61)' carried or in room with player
```
*Actions*
```
Print message 'Note here says: `I be liking parrots, they be smart matey\!`'
```
### Action 163 - Input: LOO MAP
*Conditions*
```
item 'Map(index:45)' carried or in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'read it?'
```
### Action 164 - Input: REA FLY
*Conditions*
```
item 'Small advertising flyer(index:62)' carried or in room with player
```
*Actions*
```
clear screen
Print message 'Ask for Adventure number 3: `MISSION IMPOSSIBLE` at your favorite computer dealer\. If they DON'T carry `ADVENTURE` have them call: 1\-305\-862\-6917  TODAY\! `ADVENTURE` also supports lower case\! '
```
### Action 165 - Input: OPE BOO
*Conditions*
```
item 'Note(index:61)' in game
item 'Large blood soaked book(index:3)' carried or in room with player
```
*Actions*
```
Print message 'Nothing happens'
Print message 'Its empty'
```
### Action 166 - Input: LOO FLY
*Conditions*
```
item 'Small advertising flyer(index:62)' carried or in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'read it?'
```
### Action 167 - Input: FLY ANY
*Actions*
```
Print message 'Sorry I can't'
```
### Action 168 - Input: BRE ANY
*Actions*
```
Print message 'Sorry I can't'
Print message 'I'm not feeling destructive\!'
```
### Action 169 - Input: LOO WIN
*Conditions*
```
item 'Open window(index:1)' in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
```
### Action 170 - Input: LOO BOA
*Conditions*
```
item 'Pirate ship(index:37)' in room with player
```
*Actions*
```
Print message 'There's something there all right\. Maybe I should'
Print message 'go there?'
```
### Action 171 - Input: FEE DES
*Actions*
```
Print message 'All right, POOF the GAME is destroyed\!'
game over
```
### Action 172 - Input: KIL ANY
*Actions*
```
Print message 'Sorry I can't'
Print message 'I'm not feeling destructive\!'
```
### Action 173 - Input: GET SNA
*Conditions*
```
item 'Deadly mamba snakes(index:23)' in room with player
```
*Actions*
```
Print message 'That's not very smart'
Print message 'I'm snake bit'
Death, clear dark flag, move to last room
```
### Action 174 - Input: CLO WIN
*Actions*
```
Print message 'Sorry I can't'
Print message 'Its stuck'
```
### Action 175 - Input: JUM ANY
*Actions*
```
Print message 'OK'
Print message 'Nothing happens'
```
### Action 176 - Input: WAI ANY
*Conditions*
```
bitflag 10 is false
```
*Actions*
```
swap item locations 'The tide is out(index:52)' and 'The tide is coming in(index:53)'
swap item locations 'Rusty anchor(index:15)' and 'Flotsam and jetsam(index:55)'
Print message 'OK'
```
### Action 177 - Input: LOO ANY
*Actions*
```
look
Print message 'OK'
Print message 'I see nothing special'
```
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
| 2| alcove| 1 |
| 3| secret passageway| 4, 2 |
| 4| musty attic| 3 |
| 5| \*I'M outside an open window on the ledge of a very tall building|  |
| 6| sandy beach on a tropical isle| 8 |
| 7| maze of caves| 12, 13, 14, 11 |
| 8| meadow| 14, 6 |
| 9| grass shack| 8 |
| 10| \*I'm in the ocean| 10, 24, 10, 10 |
| 11| pit| 7 |
| 12| maze of caves| 7, 14, 13 |
| 13| maze of caves| 7, 14, 12, 19 |
| 14| \*I'm at the foot of a cave ridden hill, a pathway leads on up to the top| 8 |
| 15| tool shed| 17 |
| 16| long hallway| 17 |
| 17| large cavern| 16 |
| 18| \*I'm on top of a hill\. Below is Pirates Island\. Across the sea way off in the distance I see Treasure Island| 14 |
| 19| maze of caves| 14, 14, 13 |
| 20| \*I'm aboard Pirate ship anchored off shore|  |
| 21| \*I'm on the beach at \*Treasure\* Island| 22 |
| 22| spooky old graveyard filled with piles of empty and broken rum bottles| 21, 23 |
| 23| large barren field| 22 |
| 24| shallow lagoon\. to the north is the ocean| 10, 6, 6, 6 |
| 25| sacked and deserted monastary| 23 |
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
| 15| Rusty anchor| ANC| 0 |
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
| 52| The tide is out| | 0 |
| 53| The tide is coming in| | 24 |
| 54| Water wings| WIN| 15 |
| 55| Flotsam and jetsam| | 24 |
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