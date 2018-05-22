# Subterranea
A simple dungeon-crawler game for a computer science class

Dean Whiteside, Trevor McKay

## Game Description
Subterranea is a game in which you controlan individual delving through various underground dungeons. Inside the dungeon are a variety of rooms, items, and enemies. The player will start with a basic weapon and no armor. The player will explore throughprocedurally generated rooms that will spawn enemies ranging from snakes to goblins. Each enemy has a chance to drop armor or weapons. Weapons and armor can also be found lying around the dungeon. The dungeon will be represented by an ever expanding ArrayList of rooms. Rooms will be randomly generated as the player ventures father.It is unreasonable to expect a game to go long enoughto fill the ArrayList to a size in which performance issues are found, so no cap will be placed on the number of rooms unless this is found to be a problem. Each room is also and ArrayList of unique tiles with their own items, enemies, and properties. The game is turned based. Moving and attacking each count as one turn. After each player turn, all other entities in the dungeon also take one turn.

## Game Parameters
•The player will start in a randomly generated room with no enemies

•Only the room occupied by the player is rendered, however all nearby rooms are included in the simulation

•The players currently equippedgear, number of rooms discovered, and health will be displayed in the HUD.Game Rules

•An input of either movement or an attack will trigger the simulation of the next turn.

•Each turn allows the player and all enemies to perform one action.

•The player cannot hold more than one weapon or piece of armor at once.

•The players attackand defensewill scale with thequality of their items. Attack will be used when calculatingdamage dealt and defense will be used when calculating damage received.

•Enemies will not spawn until the player leaves the starting room.

•After 50 rooms are discovered and cleared, the final room that spawns will be the outside world. Entering it will trigger victory.

•When the player’s health reaches zero, the game is over.



## How players will interact

•The player will view the room they are currently occupying.

•They may use the arrow keys to move left, right, up, or down.

•They may also choose to attackif an enemy is adjacent to them.

•They may move to a tile occupied by a weapon or armor set to equip it.


## How data will be loaded

•Tile and character images will be stored as PNGs.

•A list of rooms will be contained in the main class as an ArrayList.

•Each instance of room will have its own ArrayList of tiles.

•Each tile will contain its parameters as local variables.

•Each entity (player or enemy) will be a unique class.

•Most data will be procedurally generated (maybe from a seed to allow games to be replayed).

