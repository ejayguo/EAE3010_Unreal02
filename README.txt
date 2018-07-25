Yijie Guo Unreal Assignment 02
Please choose and open the project in the 'YijieGuo_Unreal02 4.19" folder.

[GamePlay Design]
[1] The goal of this game is to collect the collectable items in the scene. 

[2] There is always a collectable item located at one of the five item spawning locations randomly. 
The five locations are top-left, top-right, bottom-left, bottom-right and the center.

[3] Each time the player collects an item, he will gain one point and the scene will generate the next item randomly.

[4] There are also several AI enemies. If the player gets caught by these enemies, he will lose 1 point for each contacting.
Enemies will only chase the player, if they see the player, otherwise, they will move randomly in the scene.
Every time when the player get caught, he will have 5 seconds being invincible.

[5] If the player gets +2 points, then the player wins the game. If the player get -5 points, then the player loses the game.


[Blueprints Descriptions]
My customized blueprints are located at
..\EAE3010_Unreal02\YijieGuo_Unreal02 4.19\Content\TopDownBP\Blueprints\MyBlueprints

AIEnemy BP:
Control the AI agents.
AI agents move randomly in the scene.
If AI agents see the player, they will chase him.

CollectableItem BP:
The Item, which the player should collect to gain points.
After the player collect the item, the item actor will be destroyed and play an explosion sound.

CustomHUD BP:
The UI used to display the score and show the player if he wins or loses

FlashingLight BP:
Randomly flashing light sources in the scene.

GameManager BP:
Monitor the player score and the game status and then destribute the events to the UI to update the score and the game status.
Also, updates the invincible time duration when player gets caught by the enemy.


ItemFactory BP:
Once the current collectable item is collected by the player, 
the item factory will generate the next collectable item and place it at one of the five spawning location randomly.