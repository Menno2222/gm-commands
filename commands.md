# Debug Commands
## Regular Debug Commands
### Same thing as (F9) but without the Screenshot window.
``d_cameramode``
### Some wire boxes on in-game objects.
``d_boundbox``
### Something with .NET Protocol?
``d_rtdebug``
### Show Dynamic NPC's ID in the order they were spawned.
``d_npcid``
### Seems to be useless or not working.
``d_runspeed`` 
### Move to X, Y cords. Use ``d_showpos`` to help you.
``d_goto x, y`` 
### Move to the specified game coordinates
``d_go x, y``
### Fly but only works when you have a high movement speed for flying without speed adjustments use ``d_c2scmd 10803 66``
``d_fly`` 
### [Client to Server Console Commands](#Client-to-Server-Console-Commands)
``d_c2scmd`` 
### Sight of your camera.
``d_viewradius`` 
### Return to character selection screen.
``d_relogin`` 
### Seems to be useless or not working. Perhaps to use a skill?
``d_skill`` 
### Show/Hide Water 0-2
``d_render_water`` 
### Show/Hide Grasses 
``d_render_grass`` 
### Show/Hide Trees
``d_render_forest`` 
### Show/Hide Shadow
``d_render_shadow`` 
### Show/Hide Outline
``d_render_outline`` 
### Do not prevent the window from updating when it loses focus.
``d_rendernofocus``
### Seems to be useless or not working.
``d_turnaround`` 
### Show the distance between your character and the cursor.
``d_testdist`` 
### Seems to be useless or not working.
``d_gfx``
### Show/Hide the cords for every NPC, MOB, PLAYER (and you).
``d_showpos`` 
### Seems to be useless or not working.
``d_trnlayer`` 
### Show/Hide 3D game information.
``d_a3dstat`` 
### Show/Hide computer and game resources.
``d_gamestat`` 
### Change the render of the trees. 0-4
``d_treelod`` 
### Show/Hide FPS in the right upper corner of the screen.
``d_fps`` 
### Seems to be useless or not working.
``d_playerradius`` 
### Show/Hide character's ID instead of their name. You can also get a character's ID by ``CTRL + Right Click`` their name in chat.
``d_showid`` 
### Seems to be useless or not working.
``d_skipframe`` 
### Seems to be useless or not working.
``d_modelupdate`` 
### Write dump, close the game and show the Report Bug window.
``d_minidump`` 
### Change ingame time (client side only). Format: 10,00 (mean 10AM).
``d_settimeofday`` 
### Show the server date and time.
``d_getservertime`` 
### Seems to be useless or not working. Quests are known as Tasks may be related to completing a quest
``d_task`` 
### Changer render of mipmap/pixel. 0-10 high-low quality
``d_mipmapbias`` 
### Seems to be useless or not working.
``d_trncull`` 
### Maybe for make some changes on GS(gamed)? GS controls the servers rates(exp/drop/gold/spirit/etc) and who knows what else.
``d_gscmd`` 
### Delete command?
``d_delcmd`` 
### Changes window title?
``d_title`` 
### Seems to be useless or not working.
``d_namepos`` 
### Display all purchased EB?
``d_money``
### Open a url in the browser
``d_ie <url>``
### Show character creation time
``d_createtime``

### ID Search
#### Search for a partial name of an item / mob / npc and get its ID in return
``d_query`` 
#### Type an npc id and get back its coordinates (if its already in the autopath database)
``d_querynpc`` 
#### Search for a partial name of an NPC Service and get its ID in return
``d_queryservice`` 
#### Type in a partial model path and it spits out the items that use it
``d_querymodel`` 

## Client to Server Console Commands
### Gain 9500 gold
``d_c2scmd 1988``
### Gain 100 EB
``d_c2scmd 2014``
### Expand inventory slots by amount
``d_c2scmd 2016 <amount>``
### Create item with 1 minute timer(no idea how to change timer amount needs to be looked into)
``d_c2scmd 2001 <ID>``
### Spawns item by quantity on the ground
``d_c2scmd 10800 <ID> <QUANTITY>``
### Spawns a mob/npc (NPCs that are spawned are not interactable)
``d_c2scmd 10802 <MonsterID> <Num>``