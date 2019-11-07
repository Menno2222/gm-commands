# Debug Commands
## Regular Debug Commands
### Same thing as (F9) but without the Screenshot window.
``d_cameramode``
### Some wire boxes on in-game objects.
``d_boundbox``
### Something with .NET Protocol?
``d_rtdebug``

"d_npcid" Show Dynamic NPC's ID in the order they were spawned.

"d_runspeed" Seems to be useless or not working.

"d_goto" Move to X, Y cords. Use "d_showpos" to help you.

"d_fly" Seems to be useless or not working.

"d_c2scmd" Maybe for sending some command to server? But wich commands?

"d_viewradius" Sight of your camera.

"d_relogin" Return to character selection screen.

"d_skill" Seems to be useless or not working.

"d_render_water" Show/Hide Water

"d_render_grass" Show/Hide Grasses

"d_render_forest" Show/Hide Trees

"d_render_shadow" Show/Hide Shadow

"d_render_outline" Show/Hide Outline

"d_turnaround" Seems to be useless or not working.

"d_testdist" Show the distance between your character and the cursor.

"d_gfx" Seems to be useless or not working.

"d_showpos" Show/Hide the cords for every NPC, MOB, PLAYER (and you).

"d_trnlayer" Seems to be useless or not working.

"d_a3dstat" Show/Hide 3D game information.

"d_gamestat" Show/Hide computer and game resources.

"d_treelod" Change the render of the trees.

"d_fps" Show/Hide FPS in the right upper corner of the screen.

"d_playerradius" Seems to be useless or not working.

"d_showid" Show/Hide character's ID instead of their name.

"d_skipframe" Seems to be useless or not working.

"d_modelupdate" Seems to be useless or not working.

"d_minidump" Write dumpe, close the game and show the Report Bug window.

"d_settimeofday" Change ingame time (client side only). Format: 10,00 (mean 10AM).

"d_getservertime" Show the server date and time.

"d_task" Seems to be useless or not working.

"d_mipmapbias" Changer render of mipmap/pixel.

"d_trncull" Seems to be useless or not working.

"d_gscmd" Maybe for make some changes on GS(gamed)?

"d_delcmd" Delete command?

"d_title" Seems to be useless or not working.

"d_namepos" Seems to be useless or not working.

## CLient to Server Console Commands
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