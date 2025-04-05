# Adventureland.md
## Actions
### Action 0 - FISH ESCAPE - Probability: 75
 *Conditions*
 ```
 item '*GOLDEN FISH* - I:8' carried
 item '*GOLDEN NET* - I:19' not carried
 ```
 *Actions*
 ```
 Print message 'Fish have escaped back to the lake.'
 item '*GOLDEN FISH* - I:8' is moved to room 10
 ```
### Action 1 - DIE BITES - Probability: 10
 *Conditions*
 ```
 item 'Infected chigger bites - I:21' carried
 player not in room 33
 ```
 *Actions*
 ```
 Print message 'My bites have rotted my whole body!'
 Death, clear dark flag, move to last room
 ```
### Action 2 - BITE INFECT - Probability: 10
 *Conditions*
 ```
 item 'Chigger bites - I:20' carried
 item 'Evil smelling mud - I:7' not carried
 ```
 *Actions*
 ```
 Print message '
My chigger bites are now INFECTED!
'
 take item 'Infected chigger bites - I:21', no check done to see if can carry
 Item 'Chigger bites - I:20' is removed from the game (put in room 0)
 ```
### Action 3 - BEES DIE - Probability: 8
 *Conditions*
 ```
 item 'Bees in a bottle - I:26' carried or in room with player
 bitflag 17 is false
 ```
 *Actions*
 ```
 Print message 'The bees all suffocated and disappeared'
 swap item locations 'Bees in a bottle - I:26' and 'Empty bottle - I:13'
 ```
### Action 4 - HIT MIRROR - Probability: 100
 *Conditions*
 ```
 bitflag 5 is set
 ```
 *Actions*
 ```
 Item '*MAGIC MIRROR* - I:38' is removed from the game (put in room 0)
 item 'Broken glass - I:41' is moved to room 21
 set 5 flag
 look
 ```
### Action 5 - IN HADES - Probability: 100
 *Conditions*
 ```
 player in room 24
 ```
 *Actions*
 ```
 Print message 'You lost *ALL* treasures.'
 game over
 ```
### Action 6 - MUD OFF - Probability: 5
 *Conditions*
 ```
 item 'Evil smelling mud - I:7' carried
 item 'Water in bottle - I:12' not carried
 ```
 *Actions*
 ```
 Print message 'The mud dried up and fell off.'
 item 'Evil smelling mud - I:7' is moved to room 1
 ```
### Action 7 - BIT CHIG - Probability: 8
 *Conditions*
 ```
 item 'Chigger bites - I:20' not carried
 item 'Infected chigger bites - I:21' not carried
 item 'Chiggers - I:42' in room with player
 item 'Evil smelling mud - I:7' not carried
 ```
 *Actions*
 ```
 take item 'Chigger bites - I:20', no check done to see if can carry
 Print message '
I'm bitten by chiggers.
'
 ```
### Action 8 - BEE STING - Probability: 8
 *Conditions*
 ```
 item 'Large african bees - I:24' in room with player
 item 'Evil smelling mud - I:7' not carried or in room with player
 ```
 *Actions*
 ```
 Print message 'Bees sting me'
 Death, clear dark flag, move to last room
 ```
### Action 9 - LITE - Probability: 100
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
### Action 10 - FISH DIE - Probability: 50
 *Conditions*
 ```
 item '*GOLDEN FISH* - I:8' carried
 item 'Water in bottle - I:12' not carried
 ```
 *Actions*
 ```
 Print message 'Too dry, the fish died.'
 Item '*GOLDEN FISH* - I:8' is removed from the game (put in room 0)
 get item 'Dead fish - I:55', check if can carry
 ```
### Action 11 - MOVE OX - Probability: 100
 *Conditions*
 ```
 bitflag 7 is set
 ```
 *Actions*
 ```
 set 7 flag
 item '*Small statue of a BLUE OX* - I:47' is moved to room 25
 output inventory
 ```
### Action 12 - GET CHIG - Probability: 30
 *Conditions*
 ```
 item 'Chiggers - I:42' carried
 item 'Infected chigger bites - I:21' not carried
 item 'Chigger bites - I:20' not carried
 item 'Evil smelling mud - I:7' not carried
 ```
 *Actions*
 ```
 take item 'Chigger bites - I:20', no check done to see if can carry
 Print message '
I'm bitten by chiggers.
'
 ```
### Action 13 - MUD DRAGON - Probability: 50
 *Conditions*
 ```
 item 'Large sleeping dragon - I:27' in room with player
 item 'Evil smelling mud - I:7' carried or in room with player
 ```
 *Actions*
 ```
 clear screen
 Print message 'Dragon smells something. Awakens & attacks me!'
 Death, clear dark flag, move to last room
 ```
### Action 14 - BLAST WALL - Probability: 100
 *Conditions*
 ```
 bitflag 12 is set
 item 'Bricked up window - I:32' in room with player
 ```
 *Actions*
 ```
 drops item 'Loose fire bricks - I:36' into current room
 Item 'Bricked up window - I:32' is removed from the game (put in room 0)
 drops item 'Bricked up window with a hole in it - I:35' into current room
 ```
### Action 15 - BLAS DRAGON - Probability: 100
 *Conditions*
 ```
 bitflag 12 is set
 item 'Large sleeping dragon - I:27' in room with player
 ```
 *Actions*
 ```
 drops item 'Smoking hole. pieces of dragon and gore. - I:52' into current room
 Item 'Large sleeping dragon - I:27' is removed from the game (put in room 0)
 ```
### Action 16 - 1ST MIRROR CLUE - Probability: 100
 *Conditions*
 ```
 bitflag 1 is set
 bitflag 2 is false
 ```
 *Actions*
 ```
 Print message '` DRAGON STING ` and fades. I don't get it, I hope you do.'
 set 1 flag
 set 2 flag
 ```
### Action 17 - BEAR MAD - Probability: 100
 *Conditions*
 ```
 bitflag 14 is set
 ```
 *Actions*
 ```
 take item 'Empty bottle - I:13', no check done to see if can carry
 set 14 flag
 Death, clear dark flag, move to last room
 ```
### Action 18 - RESET BLAST - Probability: 100
 *Conditions*
 ```
 bitflag 12 is set
 ```
 *Actions*
 ```
 look
 set 12 flag
 ```
### Action 19 - INTRO - Probability: 100
 *Conditions*
 ```
 bitflag 13 is false
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 set 13 flag
 Print message '
Welcome to Adventure number: 1 `ADVENTURELAND`.
In this Adventure you're to find *TREASURES* & store them away.

To see how well you're doing say: `SCORE`'
 Print message 'Remember you can always say `HELP`'
 ```
### Action 20 - 2ND MIRROR CLUE - Probability: 100
 *Conditions*
 ```
 bitflag 1 is set
 bitflag 2 is set
 ```
 *Actions*
 ```
 Print message '`Don't waste honey, get mad instead! Dam lava!?`'
 set 1 flag
 set 2 flag
 ```
### Action 21 - DEAD LAMP - Probability: 100
 *Conditions*
 ```
 bitflag 16 is set
 ```
 *Actions*
 ```
 set 16 flag
 swap item locations 'Empty lamp - I:60' and 'Lit brass lamp - I:9'
 look
 ```
### Action 22 - MUDDY RUG - Probability: 100
 *Conditions*
 ```
 player in room 26
 item '*Thick PERSIAN RUG* - I:29' carried or in room with player
 ```
 *Actions*
 ```
 swap item locations '*Thick PERSIAN RUG* - I:29' and 'Muddy worthless old rug - I:61'
 ```
### Action 23 - Input: LOO LAV
 *Conditions*
 ```
 item 'Stream of lava - I:34' in room with player
 ```
 *Actions*
 ```
 Print message 'There's something there all right! Maybe I should go there?'
 ```
### Action 24 - Input: LOO TRE
 *Conditions*
 ```
 item '-HOLLOW- stump and remains of a felled tree - I:4' in room with player
 ```
 *Actions*
 ```
 Print message 'There's something there all right! Maybe I should go there?'
 ```
### Action 25 - Input: GET MUD
 *Conditions*
 ```
 item 'Evil smelling mud - I:7' in room with player
 item 'Infected chigger bites - I:21' carried
 ```
 *Actions*
 ```
 Item 'Infected chigger bites - I:21' is removed from the game (put in room 0)
 get item 'Evil smelling mud - I:7', check if can carry
 Print message 'OK'
 Print message 'BOY that really hit the spot!'
 ```
### Action 26 - Input: GET HON
 *Conditions*
 ```
 item '*ROYAL HONEY* - I:23' in room with player
 item 'Evil smelling mud - I:7' not carried
 item 'Large african bees - I:24' in room with player
 ```
 *Actions*
 ```
 Print message 'Bees sting me'
 Death, clear dark flag, move to last room
 ```
### Action 27 - Input: GET MUD
 *Conditions*
 ```
 item 'Evil smelling mud - I:7' in room with player
 item 'Chigger bites - I:20' carried
 ```
 *Actions*
 ```
 Item 'Chigger bites - I:20' is removed from the game (put in room 0)
 get item 'Evil smelling mud - I:7', check if can carry
 Print message 'OK'
 Print message 'BOY that really hit the spot!'
 ```
### Action 28 - Input: DRO HON
 *Conditions*
 ```
 item '*ROYAL HONEY* - I:23' carried
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Item '*ROYAL HONEY* - I:23' is removed from the game (put in room 0)
 Print message 'Bear eats the honey and falls asleep.'
 drops item 'Sleeping bear - I:39' into current room
 Item 'Very thin black bear - I:25' is removed from the game (put in room 0)
 ```
### Action 29 - Input: DRO HON
 *Conditions*
 ```
 item '*ROYAL HONEY* - I:23' carried
 ```
 *Actions*
 ```
 drops item '*ROYAL HONEY* - I:23' into current room
 ```
### Action 30 - Input: GET BEE
 *Conditions*
 ```
 item 'Large african bees - I:24' in room with player
 item 'Evil smelling mud - I:7' not carried
 ```
 *Actions*
 ```
 Print message 'Bees sting me'
 Death, clear dark flag, move to last room
 ```
### Action 31 - Input: GET BEE
 *Conditions*
 ```
 item 'Large african bees - I:24' in room with player
 item 'Evil smelling mud - I:7' carried
 item 'Empty bottle - I:13' not carried
 ```
 *Actions*
 ```
 Print message 'First I need an empty container.'
 ```
### Action 32 - Input: GET BEE
 *Conditions*
 ```
 item 'Large african bees - I:24' in room with player
 item 'Evil smelling mud - I:7' carried
 item 'Empty bottle - I:13' carried
 ```
 *Actions*
 ```
 swap item locations 'Empty bottle - I:13' and 'Bees in a bottle - I:26'
 Print message 'OK'
 ```
### Action 33 - Input: GET INV
 *Actions*
 ```
 output inventory
 ```
### Action 34 - Input: CRO LAV
 *Conditions*
 ```
 player in room 18
 ```
 *Actions*
 ```
 Print message 'No, its too hot.'
 ```
### Action 35 - Input: INV ANY
 *Actions*
 ```
 output inventory
 ```
### Action 36 - Input: SAY AWA
 *Conditions*
 ```
 item '*Thick PERSIAN RUG* - I:29' carried
 player in room 17
 ```
 *Actions*
 ```
 move room 23
 Print message 'Something I'm holding vibrates and...'
 clear darkness flag
 look
 ```
### Action 37 - Input: LIG ANY
 *Conditions*
 ```
 item 'Flint & steel - I:28' not carried
 ```
 *Actions*
 ```
 Print message 'nothing to light it with'
 ```
### Action 38 - Input: LIG GAS
 *Conditions*
 ```
 item 'Distended gas bladder - I:31' carried
 item 'Flint & steel - I:28' carried
 ```
 *Actions*
 ```
 Print message 'Gas bladder blew up'
 Print message 'in my hands!'
 Death, clear dark flag, move to last room
 Item 'Distended gas bladder - I:31' is removed from the game (put in room 0)
 ```
### Action 39 - Input: MAK HOL
 *Conditions*
 ```
 item 'Bees in a bottle - I:26' carried or in room with player
 ```
 *Actions*
 ```
 set 17 flag
 Print message 'OK'
 ```
### Action 40 - Input: LIG GAS
 *Conditions*
 ```
 item 'Distended gas bladder - I:31' in room with player
 item 'Flint & steel - I:28' carried
 ```
 *Actions*
 ```
 clear screen
 Item 'Distended gas bladder - I:31' is removed from the game (put in room 0)
 set 12 flag
 Print message 'Gas bladder blew up'
 ```
### Action 41 - Input: GO LED
 *Conditions*
 ```
 player in room 20
 item 'Bricked up window with a hole in it - I:35' in room with player
 ```
 *Actions*
 ```
 move room 19
 clear screen
 look
 ```
### Action 42 - Input: GET GAS
 *Conditions*
 ```
 player in room 1
 item 'Empty wine bladder - I:40' not carried
 ```
 *Actions*
 ```
 Print message 'First I need an empty container.'
 ```
### Action 43 - Input: GET GAS
 *Conditions*
 ```
 player in room 1
 item 'Empty wine bladder - I:40' carried
 ```
 *Actions*
 ```
 swap item locations 'Empty wine bladder - I:40' and 'Distended gas bladder - I:31'
 Print message 'OK'
 ```
### Action 44 - Input: DRO GAS
 *Conditions*
 ```
 item 'Distended gas bladder - I:31' carried
 ```
 *Actions*
 ```
 swap item locations 'Distended gas bladder - I:31' and 'Empty wine bladder - I:40'
 Print message 'OK'
 Print message 'Gas dissipates. (I think you blew it)'
 ```
### Action 45 - Input: LIG GAS
 *Conditions*
 ```
 item 'Swamp gas - I:18' in room with player
 item 'Flint & steel - I:28' carried
 ```
 *Actions*
 ```
 Print message 'gas needs to be contained before it will burn'
 ```
### Action 46 - Input: FIN SWA
 *Actions*
 ```
 Print message 'I don't know where it is'
 ```
### Action 47 - Input: GO THR
 *Conditions*
 ```
 player in room 19
 ```
 *Actions*
 ```
 Print message 'How?'
 ```
### Action 48 - Input: GET MIR
 *Conditions*
 ```
 item '*MAGIC MIRROR* - I:38' in room with player
 item 'Very thin black bear - I:25' not in room with player
 ```
 *Actions*
 ```
 get item '*MAGIC MIRROR* - I:38', check if can carry
 Print message 'OK'
 ```
### Action 49 - Input: DRO MIR
 *Conditions*
 ```
 item '*MAGIC MIRROR* - I:38' carried
 item '*Thick PERSIAN RUG* - I:29' in room with player
 ```
 *Actions*
 ```
 drops item '*MAGIC MIRROR* - I:38' into current room
 Print message 'Mirror lands softly on rug, lights up and says:'
 set 1 flag
 ```
### Action 50 - Input: DRI FRU
 *Conditions*
 ```
 item '*JEWELED FRUIT* - I:46' carried
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 Item '*JEWELED FRUIT* - I:46' is removed from the game (put in room 0)
 ```
### Action 51 - Input: GET WAT
 *Conditions*
 ```
 item 'Water - I:6' in room with player
 item 'Empty bottle - I:13' carried
 ```
 *Actions*
 ```
 Item 'Empty bottle - I:13' is removed from the game (put in room 0)
 get item 'Water in bottle - I:12', check if can carry
 Print message 'OK'
 ```
### Action 52 - Input: JUM ANY
 *Conditions*
 ```
 player in room 19
 item 'Loose fire bricks - I:36' not carried
 ```
 *Actions*
 ```
 move room 21
 look
 ```
### Action 53 - Input: JUM ANY
 *Conditions*
 ```
 player in room 21
 ```
 *Actions*
 ```
 move room 19
 look
 ```
### Action 54 - Input: GO THR
 *Conditions*
 ```
 player in room 21
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Print message 'Bear won't let me'
 ```
### Action 55 - Input: GO THR
 *Conditions*
 ```
 player in room 21
 item 'Very thin black bear - I:25' not in room with player
 ```
 *Actions*
 ```
 move room 22
 clear screen
 look
 ```
### Action 56 - BUILD DAM - Input: MAK LAV
 *Conditions*
 ```
 item 'Loose fire bricks - I:36' carried or in room with player
 item 'Stream of lava - I:34' in room with player
 ```
 *Actions*
 ```
 swap item locations 'Glowing *FIRESTONE* - I:0' and 'Stream of lava - I:34'
 drops item 'Lava stream with brick dam - I:45' into current room
 look
 ```
### Action 57 - Input: GO LAV
 *Conditions*
 ```
 player in room 18
 ```
 *Actions*
 ```
 Print message 'No, its too hot.'
 ```
### Action 58 - Input: DRO BEE
 *Conditions*
 ```
 item 'Bees in a bottle - I:26' carried
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Print message 'Bees madden bear, bear then attacks me!'
 Item 'Bees in a bottle - I:26' is removed from the game (put in room 0)
 drops item 'Large african bees - I:24' into current room
 set 14 flag
 ```
### Action 59 - Input: GET WAT
 *Conditions*
 ```
 item 'Water - I:6' in room with player
 item 'Empty bottle - I:13' not carried
 ```
 *Actions*
 ```
 Print message 'First I need an empty container.'
 ```
### Action 60 - Input: REA WEB
 *Conditions*
 ```
 item 'Spider web with writing on it - I:3' in room with player
 ```
 *Actions*
 ```
 Print message 'Chop 'er down!'
 ```
### Action 61 - Input: GO TRE
 *Conditions*
 ```
 item 'Cypress tree - I:5' in room with player
 ```
 *Actions*
 ```
 move room 2
 clear screen
 look
 ```
### Action 62 - Input: DRO WAT
 *Conditions*
 ```
 item 'Water in bottle - I:12' carried
 player not in room 18
 ```
 *Actions*
 ```
 swap item locations 'Water in bottle - I:12' and 'Empty bottle - I:13'
 Print message 'OK'
 Print message 'It soaks into the ground'
 ```
### Action 63 - Input: FIL LAM
 *Conditions*
 ```
 item 'Patches of `OILY` slime - I:22' carried or in room with player
 item 'Empty lamp - I:60' carried
 ```
 *Actions*
 ```
 Item 'Patches of `OILY` slime - I:22' is removed from the game (put in room 0)
 Item 'Empty lamp - I:60' is removed from the game (put in room 0)
 Print message 'Lamp is now full & lit'
 refill lamp
 ```
### Action 64 - Input: CHO TRE
 *Conditions*
 ```
 item 'Cypress tree - I:5' in room with player
 item 'Ring of skeleton keys - I:14' not carried or in room with player
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' carried
 ```
 *Actions*
 ```
 Item 'Cypress tree - I:5' is removed from the game (put in room 0)
 drops item '-HOLLOW- stump and remains of a felled tree - I:4' into current room
 Print message 'TIMBER. Something fell from the tree top & vanished in the swamp'
 ```
### Action 65 - Input: OPE DOO
 *Conditions*
 ```
 player in room 5
 item 'Locked door - I:16' in room with player
 item 'Ring of skeleton keys - I:14' not carried
 ```
 *Actions*
 ```
 Print message 'I can't its locked'
 ```
### Action 66 - Input: UNL DOO
 *Conditions*
 ```
 player in room 5
 item 'Locked door - I:16' in room with player
 item 'Ring of skeleton keys - I:14' not carried
 ```
 *Actions*
 ```
 Print message 'I can't its locked'
 ```
### Action 67 - Input: THR AXE
 *Conditions*
 ```
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' carried
 ```
 *Actions*
 ```
 Print message 'In 2 words tell me at what...like: AT TREE'
 set 3 flag
 drops item 'Rusty axe (Magic word `BUNYON` on it) - I:11' into current room
 ```
### Action 68 - Input: OPE DOO
 *Conditions*
 ```
 item 'Locked door - I:16' in room with player
 item 'Ring of skeleton keys - I:14' carried
 ```
 *Actions*
 ```
 Item 'Locked door - I:16' is removed from the game (put in room 0)
 drops item 'Open door with a hallway beyond - I:17' into current room
 look
 ```
### Action 69 - Input: CRO ANY
 *Actions*
 ```
 Print message 'How?'
 ```
### Action 70 - Input: JUM ANY
 *Conditions*
 ```
 player in room 19
 item 'Loose fire bricks - I:36' carried
 ```
 *Actions*
 ```
 Print message 'Somethings too heavy. I fall.'
 Death, clear dark flag, move to last room
 ```
### Action 71 - Input: DAM LAV
 *Conditions*
 ```
 item 'Loose fire bricks - I:36' carried or in room with player
 item 'Stream of lava - I:34' in room with player
 ```
 *Actions*
 ```
 swap item locations 'Glowing *FIRESTONE* - I:0' and 'Stream of lava - I:34'
 drops item 'Lava stream with brick dam - I:45' into current room
 look
 ```
### Action 72 - Input: GET BRI
 *Conditions*
 ```
 item 'Loose fire bricks - I:36' in room with player
 ```
 *Actions*
 ```
 get item 'Loose fire bricks - I:36', check if can carry
 Print message 'OK'
 Print message 'Its heavy!'
 ```
### Action 73 - Input: STO ANY
 *Actions*
 ```
 Print message 'To stop game say QUIT'
 ```
### Action 74 - Input: QUI ANY
 *Actions*
 ```
 score
 game over
 ```
### Action 75 - Input: GET MIR
 *Conditions*
 ```
 item '*MAGIC MIRROR* - I:38' in room with player
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Print message 'Bear won't let me'
 ```
### Action 76 - Input: DRO MIR
 *Conditions*
 ```
 item '*MAGIC MIRROR* - I:38' carried
 item '*Thick PERSIAN RUG* - I:29' not in room with player
 ```
 *Actions*
 ```
 Print message 'Mirror hits floor and shatters into a MILLION pieces'
 drops item 'Broken glass - I:41' into current room
 Item '*MAGIC MIRROR* - I:38' is removed from the game (put in room 0)
 ```
### Action 77 - Input: AT BEA
 *Conditions*
 ```
 bitflag 3 is set
 item '*MAGIC MIRROR* - I:38' not in room with player
 ```
 *Actions*
 ```
 Print message 'OK, I threw it.'
 Print message 'A voice BOOOOMS out:'
 Print message 'please leave it alone'
 set 3 flag
 ```
### Action 78 - Input: AT DRA
 *Conditions*
 ```
 bitflag 3 is set
 item 'Large sleeping dragon - I:27' in room with player
 ```
 *Actions*
 ```
 Print message 'OK, I threw it.'
 Print message 'It doesn't seem to bother him at all!'
 set 3 flag
 ```
### Action 79 - Input: SCO ANY
 *Actions*
 ```
 score
 ```
### Action 80 - Input: HEL ANY
 *Conditions*
 ```
 item 'Chigger bites - I:20' carried
 ```
 *Actions*
 ```
 clear screen
 Print message 'A voice BOOOOMS out:'
 Print message 'Medicine is good for bites.'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 81 - Input: HEL ANY
 *Conditions*
 ```
 item 'Infected chigger bites - I:21' carried
 ```
 *Actions*
 ```
 clear screen
 Print message 'A voice BOOOOMS out:'
 Print message 'Medicine is good for bites.'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 82 - Input: GO LED
 *Conditions*
 ```
 player in room 18
 ```
 *Actions*
 ```
 Print message 'Not here.'
 ```
### Action 83 - Input: GET LAV
 *Conditions*
 ```
 item 'Stream of lava - I:34' in room with player
 ```
 *Actions*
 ```
 Print message 'No, its too hot.'
 ```
### Action 84 - Input: SCR ANY
 *Conditions*
 ```
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Print message 'Bear is so startled that he FELL off the ledge!'
 item 'Slightly woozy bear - I:43' is moved to room 18
 Item 'Very thin black bear - I:25' is removed from the game (put in room 0)
 ```
### Action 85 - Input: DRO BEE
 *Conditions*
 ```
 item 'Bees in a bottle - I:26' carried
 item 'Large sleeping dragon - I:27' in room with player
 ```
 *Actions*
 ```
 drops item 'Large african bees - I:24' into current room
 drops item '*DRAGON EGGS* (very rare) - I:44' into current room
 Item 'Large sleeping dragon - I:27' is removed from the game (put in room 0)
 Print message 'The bees attack the dragon which gets so annoyed it gets up
and flys away...'
 ```
### Action 86 - Input: AT WIN
 *Conditions*
 ```
 bitflag 3 is set
 ```
 *Actions*
 ```
 set 3 flag
 Print message 'Nothing happens'
 Print message 'A voice BOOOOMS out:'
 Print message 'Remember you can always say `HELP`'
 ```
### Action 87 - Input: OPE DOO
 *Conditions*
 ```
 item 'Open door with a hallway beyond - I:17' in room with player
 ```
 *Actions*
 ```
 look
 ```
### Action 88 - Input: GO HOL
 *Conditions*
 ```
 item 'Bricked up window with a hole in it - I:35' in room with player
 ```
 *Actions*
 ```
 clear screen
 move room 19
 look
 ```
### Action 89 - Input: AT BEA
 *Conditions*
 ```
 bitflag 3 is set
 item '*MAGIC MIRROR* - I:38' in room with player
 ```
 *Actions*
 ```
 Item '*MAGIC MIRROR* - I:38' is removed from the game (put in room 0)
 set 5 flag
 Print message 'OH NO... Bear dodges... CRASH!'
 set 4 flag
 ```
### Action 90 - Input: FIN AXE
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'I don't know where it is'
 ```
### Action 91 - Input: WAK ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 Print message 'Maybe if I threw something?...'
 ```
### Action 92 - Input: GO TRE
 *Conditions*
 ```
 item '-HOLLOW- stump and remains of a felled tree - I:4' in room with player
 ```
 *Actions*
 ```
 move room 3
 clear screen
 look
 ```
### Action 93 - Input: CHO TRE
 *Conditions*
 ```
 item 'Cypress tree - I:5' in room with player
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' carried
 item 'Ring of skeleton keys - I:14' carried
 ```
 *Actions*
 ```
 Item 'Cypress tree - I:5' is removed from the game (put in room 0)
 drops item '-HOLLOW- stump and remains of a felled tree - I:4' into current room
 Print message 'TIMBER!'
 ```
### Action 94 - Input: ATT BEA
 *Conditions*
 ```
 item 'Very thin black bear - I:25' in room with player
 ```
 *Actions*
 ```
 Print message 'Bear won't let me'
 Print message 'Maybe if I threw something?...'
 ```
### Action 95 - Input: ATT DRA
 *Conditions*
 ```
 item 'Large sleeping dragon - I:27' in room with player
 ```
 *Actions*
 ```
 Print message 'It doesn't seem to bother him at all!'
 Print message 'Maybe if I threw something?...'
 ```
### Action 96 - Input: DRI WAT
 *Conditions*
 ```
 item 'Water in bottle - I:12' carried
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 Item 'Water in bottle - I:12' is removed from the game (put in room 0)
 get item 'Empty bottle - I:13', check if can carry
 ```
### Action 97 - Input: DRI WAT
 *Conditions*
 ```
 item 'Water - I:6' in room with player
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 ```
### Action 98 - Input: DRI HON
 *Conditions*
 ```
 item '*ROYAL HONEY* - I:23' carried or in room with player
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 Item '*ROYAL HONEY* - I:23' is removed from the game (put in room 0)
 ```
### Action 99 - Input: AT DOO
 *Conditions*
 ```
 item 'Locked door - I:16' in room with player
 bitflag 3 is set
 ```
 *Actions*
 ```
 Item 'Locked door - I:16' is removed from the game (put in room 0)
 drops item 'Open door with a hallway beyond - I:17' into current room
 Print message 'Lock shatters'
 set 3 flag
 ```
### Action 100 - Input: SWI ANY
 *Conditions*
 ```
 player in room 26
 something carried
 ```
 *Actions*
 ```
 Print message 'Somethings too heavy. I fall.'
 ```
### Action 101 - Input: SWI ANY
 *Conditions*
 ```
 player in room 26
 nothing carried
 ```
 *Actions*
 ```
 move room 10
 clear screen
 look
 ```
### Action 102 - Input: CHO ANY
 *Conditions*
 ```
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' not carried
 ```
 *Actions*
 ```
 Print message 'I'm not carrying ax, take inventory!'
 ```
### Action 103 - Input: SAY BUN
 *Conditions*
 ```
 item '*Small statue of a BLUE OX* - I:47' carried or in room with player
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' carried
 ```
 *Actions*
 ```
 echo noun
 Print message 'Something I'm holding vibrates and...'
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' is moved to room 25
 set 7 flag
 ```
### Action 104 - Input: SAY BUN
 *Conditions*
 ```
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' carried
 player not in room 26
 ```
 *Actions*
 ```
 echo noun
 Print message 'Something I'm holding vibrates and...'
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' is moved to room 25
 output inventory
 ```
### Action 105 - Input: RUB LAM
 *Conditions*
 ```
 item 'Lit brass lamp - I:9' carried or in room with player
 ```
 *Actions*
 ```
 Print message 'No, its too hot.'
 ```
### Action 106 - Input: GET MUD
 *Conditions*
 ```
 item 'Evil smelling mud - I:7' in room with player
 ```
 *Actions*
 ```
 get item 'Evil smelling mud - I:7', check if can carry
 Print message 'OK'
 ```
### Action 107 - Input: RUB LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 bitflag 8 is false
 ```
 *Actions*
 ```
 Print message 'A glowing Genie appears, drops somehting, then vanishes.'
 drops item '*DIAMOND RING* - I:48' into current room
 set 8 flag
 ```
### Action 108 - Input: RUB LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 bitflag 11 is set
 ```
 *Actions*
 ```
 Print message 'Nothing happens'
 ```
### Action 109 - Input: RUB LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 bitflag 10 is set
 ```
 *Actions*
 ```
 Print message 'A glowing Genie appears, says `Boy you're selfish`, takes
something and then makes `ME` vanish!'
 set 11 flag
 Death, clear dark flag, move to last room
 Item '*DIAMOND RING* - I:48' is removed from the game (put in room 0)
 ```
### Action 110 - Input: RUB LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 bitflag 9 is set
 ```
 *Actions*
 ```
 Print message 'A glowing Genie appears, says `Boy you're selfish`, takes
something and then makes `ME` vanish!'
 set 10 flag
 Death, clear dark flag, move to last room
 Item '*DIAMOND BRACELET* - I:49' is removed from the game (put in room 0)
 ```
### Action 111 - Input: RUB LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 bitflag 8 is set
 ```
 *Actions*
 ```
 Print message 'A glowing Genie appears, drops somehting, then vanishes.'
 drops item '*DIAMOND BRACELET* - I:49' into current room
 set 9 flag
 ```
### Action 112 - Input: SCR ANY
 *Conditions*
 ```
 item 'Chigger bites - I:20' carried
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 Print message '
My chigger bites are now INFECTED!
'
 swap item locations 'Chigger bites - I:20' and 'Infected chigger bites - I:21'
 ```
### Action 113 - Input: SCR ANY
 *Conditions*
 ```
 item 'Infected chigger bites - I:21' carried
 ```
 *Actions*
 ```
 Print message 'BOY that really hit the spot!'
 Print message 'My bites have rotted my whole body!'
 Death, clear dark flag, move to last room
 ```
### Action 114 - Input: SWI ANY
 *Conditions*
 ```
 player not in room 26
 ```
 *Actions*
 ```
 Print message 'Not here.'
 ```
### Action 115 - Input: WAV ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 ```
### Action 116 - Input: SAY BUN
 *Conditions*
 ```
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' in room with player
 ```
 *Actions*
 ```
 Print message 'OK'
 echo noun
 Print message 'The ax vibrated!'
 ```
### Action 117 - Input: LIG LAM
 *Conditions*
 ```
 item 'Lit brass lamp - I:9' carried or in room with player
 ```
 *Actions*
 ```
 Print message 'Lamp burns with a cold flameless blue glow.'
 ```
### Action 118 - Input: FIN TRE
 *Actions*
 ```
 Print message 'Try the swamp'
 ```
### Action 119 - Input: DRO BEE
 *Conditions*
 ```
 item 'Bees in a bottle - I:26' carried
 ```
 *Actions*
 ```
 drops item 'Large african bees - I:24' into current room
 swap item locations 'Bees in a bottle - I:26' and 'Empty bottle - I:13'
 Print message 'OK'
 ```
### Action 120 - Input: FIN KEY
 *Actions*
 ```
 Print message 'Try the swamp'
 ```
### Action 121 - Input: FIN MUD
 *Actions*
 ```
 Print message 'Try the swamp'
 ```
### Action 122 - Input: AT SHO
 *Conditions*
 ```
 bitflag 3 is set
 player in room 26
 ```
 *Actions*
 ```
 set 3 flag
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' is moved to room 10
 Print message 'OK'
 ```
### Action 123 - Input: GO TRE
 *Conditions*
 ```
 player in room 11
 ```
 *Actions*
 ```
 move room 28
 clear screen
 look
 ```
### Action 124 - Input: HEL ANY
 *Conditions*
 ```
 player in room 26
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 Print message 'You may need to say magic words here'
 ```
### Action 125 - Input: HEL ANY
 *Conditions*
 ```
 player in room 11
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 126 - Input: HEL ANY
 *Conditions*
 ```
 player in room 19
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 127 - Input: HEL ANY
 *Conditions*
 ```
 player in room 23
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'There are only 3 ways to wake the Dragon!'
 ```
### Action 128 - Input: HEL ANY
 *Conditions*
 ```
 player in room 13
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'You may need to say magic words here'
 ```
### Action 129 - Input: HEL ANY
 *Conditions*
 ```
 player in room 17
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'You may need to say magic words here'
 ```
### Action 130 - Input: HEL ANY
 *Conditions*
 ```
 player in room 15
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'You may need to say magic words here'
 ```
### Action 131 - Input: HEL ANY
 *Conditions*
 ```
 player in room 21
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 132 - Input: HEL ANY
 *Conditions*
 ```
 player in room 8
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Read the sign in the meadow!'
 ```
### Action 133 - Input: UNL DOO
 *Conditions*
 ```
 item 'Ring of skeleton keys - I:14' carried
 item 'Locked door - I:16' in room with player
 ```
 *Actions*
 ```
 drops item 'Open door with a hallway beyond - I:17' into current room
 Item 'Locked door - I:16' is removed from the game (put in room 0)
 ```
### Action 134 - Input: GO HAL
 *Conditions*
 ```
 item 'Open door with a hallway beyond - I:17' in room with player
 ```
 *Actions*
 ```
 move room 6
 set darkness flag
 clear screen
 look
 ```
### Action 135 - Input: LIG LAM
 *Conditions*
 ```
 item 'Old fashioned brass lamp - I:10' carried or in room with player
 ```
 *Actions*
 ```
 swap item locations 'Old fashioned brass lamp - I:10' and 'Lit brass lamp - I:9'
 Print message 'Lamp burns with a cold flameless blue glow.'
 look
 ```
### Action 136 - Input: UNL LAM
 *Conditions*
 ```
 item 'Lit brass lamp - I:9' carried or in room with player
 ```
 *Actions*
 ```
 swap item locations 'Lit brass lamp - I:9' and 'Old fashioned brass lamp - I:10'
 Print message 'OK'
 Print message 'Lamp is off'
 look
 ```
### Action 137 - Input: GET WEB
 *Conditions*
 ```
 item 'Spider web with writing on it - I:3' in room with player
 ```
 *Actions*
 ```
 Print message 'I'm bit by a spider'
 Death, clear dark flag, move to last room
 ```
### Action 138 - Input: GO HOL
 *Conditions*
 ```
 item 'Smoking hole. pieces of dragon and gore. - I:52' in room with player
 ```
 *Actions*
 ```
 move room 24
 clear screen
 look
 ```
### Action 139 - Input: GET SIG
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'please leave it alone'
 ```
### Action 140 - Input: LIG ANY
 *Conditions*
 ```
 item 'Flint & steel - I:28' carried
 item 'Swamp gas - I:18' not in room with player
 ```
 *Actions*
 ```
 Print message 'That won't ignite'
 ```
### Action 141 - Input: SCR ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 ```
### Action 142 - Input: SAY AWA
 *Conditions*
 ```
 item '*Thick PERSIAN RUG* - I:29' carried
 player not in room 17
 player not in room 33
 player not in room 26
 ```
 *Actions*
 ```
 move room 17
 Print message 'Something I'm holding vibrates and...'
 set darkness flag
 look
 ```
### Action 143 - Input: HEL ANY
 *Conditions*
 ```
 player in room 1
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Try --> `LOOK, JUMP, SWIM, CLIMB, FIND, TAKE, SCORE, DROP`
and any other verbs you can think of...'
 ```
### Action 144 - Input: THR AXE
 *Conditions*
 ```
 item 'Rusty axe (Magic word `BUNYON` on it) - I:11' not carried
 ```
 *Actions*
 ```
 Print message 'I'm not carrying ax, take inventory!'
 ```
### Action 145 - Input: HEL ANY
 *Conditions*
 ```
 player in room 20
 ```
 *Actions*
 ```
 Print message 'A voice BOOOOMS out:'
 Print message 'Blow it up!'
 Print message 'Try the swamp'
 ```
### Action 146 - Input: SAY BUN
 *Actions*
 ```
 Print message 'OK'
 echo noun
 Print message 'Nothing happens'
 ```
### Action 147 - Input: GO HOL
 *Conditions*
 ```
 player in room 4
 ```
 *Actions*
 ```
 move room 5
 clear screen
 look
 ```
### Action 148 - Input: GET HON
 *Conditions*
 ```
 item '*ROYAL HONEY* - I:23' in room with player
 ```
 *Actions*
 ```
 get item '*ROYAL HONEY* - I:23', check if can carry
 Print message 'OK'
 ```
### Action 149 - Input: HEL ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 Print message 'You might try examining things...'
 ```
### Action 150 - Input: CHO ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 Print message 'Maybe if I threw something?...'
 ```
### Action 151 - Input: THR ANY
 *Actions*
 ```
 Print message 'Sorry, I can only throw the ax.'
 ```
### Action 152 - Input: AT ANY
 *Conditions*
 ```
 bitflag 3 is set
 ```
 *Actions*
 ```
 set 3 flag
 Print message 'OK, I threw it.'
 Print message 'Nothing happens'
 ```
### Action 153 - Input: SAV GAM
 *Actions*
 ```
 Print message 'OK'
 save game
 ```
### Action 154 - Input: RUB ANY
 *Actions*
 ```
 Print message 'Nothing happens'
 ```
### Action 155 - Input: SAY ANY
 *Actions*
 ```
 Print message 'OK'
 echo noun
 Print message 'Nothing happens'
 ```
### Action 156 - Input: DRI ANY
 *Actions*
 ```
 Print message 'Huh? I don't think so!'
 ```
### Action 157 - Input: DRO WAT
 *Conditions*
 ```
 item 'Water in bottle - I:12' carried
 player in room 18
 ```
 *Actions*
 ```
 Print message 'Sizzle...'
 continue with next action
 swap item locations 'Water in bottle - I:12' and 'Empty bottle - I:13'
 ```
### Action 158 - Probability: 0
 *Conditions*
 ```
 item 'Glowing *FIRESTONE* - I:0' in room with player
 ```
 *Actions*
 ```
 swap item locations '*FIRESTONE* (cold now) - I:56' and 'Glowing *FIRESTONE* - I:0'
 ```
### Action 159 - Input: GET FIR
 *Conditions*
 ```
 item 'Glowing *FIRESTONE* - I:0' in room with player
 ```
 *Actions*
 ```
 Print message 'No, its too hot.'
 ```
### Action 160 - Input: GET FIR
 *Conditions*
 ```
 item '*FIRESTONE* (cold now) - I:56' in room with player
 ```
 *Actions*
 ```
 Print message 'OK'
 get item '*FIRESTONE* (cold now) - I:56', check if can carry
 ```
### Action 161 - Input: FIN ANY
 *Actions*
 ```
 Print message 'I don't know where it is'
 ```
### Action 162 - Input: REA ADV
 *Conditions*
 ```
 item 'Large outdoor Advertisement - I:62' carried or in room with player
 ```
 *Actions*
 ```
 clear screen
 Print message '
Check with your favorite computer dealer for the next Adventure
program: PIRATE ADVENTURE. If they don't carry `ADVENTURE` have
them call: 1-305-862-6917 today!
'
 ```
### Action 163 - Input: LOO HOL
 *Actions*
 ```
 Print message 'There's something there all right! Maybe I should go there?'
 ```
### Action 164 - Input: JUM ANY
 *Actions*
 ```
 Print message 'Not here.'
 ```
### Action 165 - Input: ATT SPI
 *Actions*
 ```
 Print message 'I don't know where it is'
 ```
### Action 166 - Input: ATT ANY
 *Actions*
 ```
 Print message 'How?'
 ```
### Action 167 - Input: LOO ANY
 *Actions*
 ```
 Print message 'OK'
 Print message 'I see nothing special'
 look
 ```
### Action 168 - Input: AT ANY
 *Actions*
 ```
 Print message 'What?'
 ```
### Action 169 - Input: GO HOL
 *Conditions*
 ```
 player in room 29
 ```
 *Actions*
 ```
 move room 30
 look
 ```