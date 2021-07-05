# My_RPG

This project is one of the freest project of your first year. Create your own RPG.\
Your main challenge for this game will be to create a complete product using everything that you and your\
team know.

We had the best grade of the promotion, a guarantee of quality :trophy:

## Description :sunrise_over_mountains:

Your game must follow the following rules:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• The player needs to have characteristics which you can find in the status menu.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• The player can fight enemies, statistics will impact the fights results.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• There must be NPC in your game.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• You need to implement at least one quest.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• The player must have an inventory which can contain a limited set of items.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• The player can earn experience by winning fights and accomplishing specific actions.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• With enough experience, the player can level up, upgrading its statistics.

To realize our project, we were only allowed to use some functions,\
most of them being forbidden such as: printf

<p align="center">
    <br/>
  <img src="./img/function.png" />
  <br/>
  <br/>
</p>

We started with the creation of a game engine, \
that is to say that we created functions allowing to add buttons, particle generators, animated texts... \
as simply as possible to save time later.\
You just have to call the function and the new object will be stored after the linked list of its type

<p align="center">
    <br/>
  <img src="./img/linked_list.png" />
  <br/>
  <br/>
</p>

Another important part, is the creation of a JSON parser and writer.\
We were obviously not allowed to use what already exists, so we remade a [JSON parser](https://github.com/Davphla/JSON-Parser)\
which you will see will be useful later on.

The parser is integrated in the project sources or available alone on this repository


[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=Davphla&repo=JSON-Parser&theme=gruvbox&hide_border=false)](https://github.com/Davphla/JSON-Parser)

  <br/>


Then, after preparing our game engine, we made a scene system that fades at each scene change,\
then we focused on the menu, a smooth interface, intuitive, buttons that have pixel accurate hitboxes.\
This is what we wanted and what we did.

<p align="center">
    <br/>
  <img src="./img/menu.png" />
  <br/>
  <br/>
</p>

It was also important to create a menu setting.\
We decided to program sliders for the sound,\
buttons for frames per second, and for full screen.

<p align="center">
    <br/>
  <img src="./img/settings.png" />
  <br/>
  <br/>
</p>

After that we have the different saves, the game can manage up to 3 different saves,\
if you create a new game you will have the choice between 4 different skins, \
which does not change anything to the gameplay.\
The saves are saved in .json format

<p align="center">
    <br/>
  <img src="./img/save.png" />
  <br/>
  <br/>
</p>

Speaking of the json format, here is an example of a map file.

<p align="center">
    <br/>
  <img src="./img/json_file.png" />
  <br/>
  <br/>
</p>

And speaking of maps, our maps are on five different layers to recreate a 3D effect,\
including a collision layer to manage the hitbox.\
The maps were entirely created by ourselves using [Tiled](https://www.mapeditor.org/) software, then exported to json format

<p align="center">
    <br/>
  <img src="./img/layers.png" />
  <br/>
  <br/>
</p>

We also have event management integrated directly into the map files.

<p align="center">
    <br/>
  <img src="./img/event.png" />
  <br/>
  <br/>
</p>

It is also possible to talk to NPCs, which move according to patterns.\
They stop when they detect you near them, you can talk to them, then animated texts are displayed,\
the facial expressions change according to the dialogues.

<p align="center">
    <br/>
  <img src="./img/npc.png" />
  <br/>
  <br/>
</p>

Moreover, talking to the NPC allows you to unlock quests.\
Dialogues, events, accessible zones evolve according to the quests and the player's progress.

<p align="center">
    <br/>
  <img src="./img/Quest.png" />
  <br/>
  <br/>
</p>

Then, in some areas it is possible to be attacked by monsters, the fight takes place in two phases.\
a first phase of attack where you have to press the space key at the right moment,\
the bar moves thanks to a sinusoidal function.

<p align="center">
    <br/>
  <img src="./img/attack.png" />
  <br/>
  <br/>
</p>

Then the defense part is a "Hell bullet", you are the blue ball and you have to dodge the red balls \
that are generated by 4 particle generators on the edges that are moving to avoid blind spots.\
Moreover the statistics of the monsters (level, attack) define the number, the speed, the damage of the red balls.

<p align="center">
    <br/>
  <img src="./img/defense.png" />
  <br/>
  <br/>
</p>

Fighting monsters gives you experience and items, some events also give you items. \
All of this is directly manageable from an inventory that handles drag & drop or double click to equip/use an item. \
It is also possible to throw an item out of the inventory by drag & drop to delete it permanently.

<p align="center">
    <br/>
  <img src="./img/inventory.png" />
  <br/>
  <br/>
</p>

By the way, in terms of experience, each time you pass a level you unlock a star that allows you to improve your skill tree.\
Each upgrade unlocks another one, several paths are possible, will you choose attack, defense or speed in priority? :sunglasses:

<p align="center">
    <br/>
  <img src="./img/skilltree.png" />
  <br/>
  <br/>
</p>

To finish this description, here is the in-game menu,\
with the possibility to save, to go back to the menu, to quit the game,\
to open a minimalist in-game settings menu, or just to resume the game.

<p align="center">
    <br/>
  <img src="./img/in_game_menu.png" />
  <br/>
  <br/>
</p>

Now that you know everything, it's time to explain how to play the game.

## Installation :mag_right:

:warning: This project requires CSFML 2.5.0 to run.

```
 git clone git clone https://github.com/Mikatech/my_rpg.git
 cd my_rpg
 make
```

## Start project :checkered_flag:

```
./my_rpg
```

## Results :trophy:

|                          Label                        |      Note       |
|:----------------------------------------------------------:|:------------------:|
|           Total | 200 / 200 |

## Maintainers :sunglasses:

 - [Mikaël Vallenet](https://github.com/Mikatech)
 - [David Gozlan](https://github.com/Davphla)
 - [Nolann Sabre](https://github.com/Nolann71)
 - [Maxime Premont](https://github.com/MaximePremont)
