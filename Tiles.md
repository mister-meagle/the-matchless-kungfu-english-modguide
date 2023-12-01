## Create a copy of the 1x1 or 2x2 template:
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/31b58dae-90f3-47b4-8767-a4cf0f9d6826)

## Rename the three copied files to your NewMapName, NewMapName_Save, and NewMapName_Save:
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/7e693260-afc0-44c1-aef2-1b64bcc68d8b)

## Double click your new map, set the VoxelWorld save to your new _Save file, and remove the template edit level, replacing it with your new one:
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/bf88e8a8-201f-4dfe-9321-6f6d50f5e7f1)

Under level, select the template _Edit level and press delete to remove it.  Then drag and drop your new _Edit file.
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/c9be2cae-8503-4864-a05b-b7429bd16ef2)

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/5e72139c-aab6-458c-9773-6ffe80af51eb)

## Draw the level with the voxel tools:
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/967c8ec4-8667-4793-90f1-10a974da3b66)
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/98643a70-b269-4b9d-92f7-fb556826f468)
Make sure the edges with the red, green, yellow, and blue remain flat.  Those 4 colors are special surface types that blend with adjoining tiles.  Hold shift to invert sculpting if you want to dig.

## Placing Monsters, buildings, decorations, etc:
Change to the edit layer to properly place buildings, resources and creatures:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/c05d15fe-2a20-4504-9ace-9823ce435609)

You can find buildings and creatures in the content browser under Content\EditorContent\BuildBluePrint:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/e87a185e-cd98-4232-a020-5d272f95ff78)

Decoration blueprints are in Entity\Blueprints:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/560e7b4f-c58e-46f2-ae55-3cc9d1c01945)

When finished, save everything:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/d32aa87c-1d7c-464f-b223-cd497b538c1a)

## Create a new TileAbility for the tile:
Right click on Content\Map\Tile and add a new TileAbility to the folder:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/bdaa5fc1-f2ad-4af2-a064-e0c10f503195)

It must NOT be named the same as your map.  So instead of NewMapName, call it NewMapTile:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/e0dd6e81-3d67-4b68-aba5-fa94d8d8622e)

Point the tile ability to your map:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/01e854ab-30c0-450f-b92c-f80db1c60970)


Add at least tile init, NPC respawn, and decoration respawn and connect them to the root node.  If you are adding monsters, use monster respawn as well.  Click Export JSON and make sure it succeeds:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/4c74f850-b5b5-4301-8f7a-e15552fbaa68)

## Cook your 3 tile assets:
![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/a40ec0c7-ea5f-46e4-91fc-851f56af101b)

When finished, the files will be in Saved\HotPatcher\Paks.  Rename the pak file to something to do with the tile so you don't forget what is what later:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/e347d007-fd26-447c-b2e3-0d054e8756b2)

## Create a 128x128 or 256x256 image to serve as the map preview:

It must have the SAME name as your tile.  128x128 is for 1x1 and 256x256 for 2x2 tiles.  Then drag it into the Content\UI\Textures\DiXingYuLan folder in the editor:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/adf7065e-7ad2-4470-8cf8-9c42d7989864)

Double click your new image and set the compression to UserInterface2D, and texture group to UI, then save it:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/dd55a01a-d1b4-4f1b-909f-aa5725a2c388)

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/19582cb7-2c4c-45da-a17f-d1548c6f71ea)

Now cook and pak the preview image the same way as the tile and rename it to something sensible:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/c91acd62-0313-4c1e-a107-21e9cfe91527)

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/7bef53e0-e188-405f-83cc-10e13217ddd6)

## Create a tile.csv entry for your new tile

You'll need the ID of your map from the tile ability.  Using EmEdit, provided with the Matchless Kung Fu mod tools, create an entry at the bottom of tiles.csv in Content\Etc:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/624fa7ba-c04b-409e-9247-ff57cf51ae5e)

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/cc2a2ac6-73f5-47fb-8cc8-e44276a31e8a)

Save tiles.csv and now when launching the Login map and using F9 to debug open plots of land your tile will be available.

## Copy everything to your mod folder:

The mod folder is available in Content\Javascript\Mods after you have created a mod via the uploader:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/8f9ac6f5-85bc-4db2-800e-1915b3ca9d15)

Copy both pak files and the JSON we exported earlier to the Content\Tile subfolder.

The JSON file is in Content\Etc\Tile:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/51c42236-ad80-47dd-8c51-ab256ef4c318)


![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/0c0c5680-eb41-49ec-9c2b-bc5987a4fc5a)

Copy tile.csv from Content\Etc to your mod's Content\Table subfolder:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/6cd9c3dc-030a-4422-a066-352b4ceb8ba7)

Edit it again and remove everything but the entry for your tile:

![image](https://github.com/mister-meagle/the-matchless-kungfu-english-modguide/assets/151403205/906413b8-c5ef-4d29-bdc5-7fc1962725af)

## You are ready to upload the mod.



