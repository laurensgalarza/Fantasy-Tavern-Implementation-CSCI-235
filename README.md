# Fantasy Tavern Simulation – Software Anaylsis and Design 2 Term Project
Built a C++ fantasy tavern simulation with RPG-style characters, combat, and inventories. This repo has no code to uphold Hunter College's Plagiarism Policy.

## Characters
- Created a Character `base class` and extended it into `subclasses` like Mage, Barbarian, and Ranger.
- Each character type has some unique attributes and overridden behavior alongside their shared features, with some depending on race type.
#### Example Character Information:
```
MARROW is a Level 2 UNDEAD RANGER. 
Vitality: 13
Armor: 6
They are not an enemy.
Animal Companion: FALSE
Arrows: 10
WATER: 6
POISON: 18
Affinities: POISON        
```
## Tavern
- Used `ArrayBag` to implement a Tavern class where characters can enter and exits, eat tainted stew, and can combat.
- Tracked and reported on character race composition, average level, and enemy percentage.
#### Example Report:
```
Tavern 1 report
Humans: 2 | Elves: 2 | Dwarves: 3 | Lizards: 0 | Undead: 0
The average level is: 6
42.86% are enemies.
```
## Combat
- Built a combat `queue` where players could select actions (heal, strike, throw tomato, buff armor) in a turn-based format after choosing a main character in the tavern.
- Defined custom `enums` for actions, race, and buffs in the Character class.
#### Example Combat Prompt:
```
YOUR TURN
(ENEMY)NAAN: LEVEL 2 HUMAN.
VITALITY: 4
ARMOR: 3

Choose an action(1-4):
1: BUFF_Heal            2: BUFF_MendMetal               3: ATT_Strike           4: ATT_ThrowTomato

3
(You) SKULL used Strike!
```
## Inventory
- Implemented a `Binary Search Tree (BST)` for finding and storing items in an inventory.
#### Example Inventory:
```
SWORD (WEAPON)
Level: 70
Value: 500

NOODLES (CONSUMABLE)
Level: 1
Value: 120
Quantity: 15
```

## Future Additions
- Connecting inventory to combat mechanics (e.g., choose between potions when healing, what weapon to strike with, etc.
- Evolve the project with visuals and interactivite gameplay.

