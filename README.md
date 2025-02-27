# de_supermarkt
This is a custom map, originally made for CS:GO, but being adapted for Garry's Mod.

## Adding the correct texture paths
This map uses textures from both CS:GO, and CS Source. To add the correct paths for these in Hammer, firstly, the *mount.cfg* file in your GMOD folder needs to reference the texture folders of both games. 

 - The *mount.cfg* file is found in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/cfg*
 - In the mount file, CSGO directory follows *{STEAMAPPSFOLDER}/common/Counter-Strike Global Offensive/csgo*
 - CS Source directory follows *{STEAMAPPSFOLDER}/common/counter-strike source/cstrike*

Next, the custom models need to be added to the correct directory. Add the content in *custom_assets/{maps, materials, resource}* folders to your folders of the same name, in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/{maps, materials, resource}*

Next, launch Hammer. If there are still textures and models missing, it may be missing textures from CSGO, that were lost from the move to CS2. From Steam, navigate to CS2->Properties-> Betas, then opt in to *csgo_legacy*, and *csgo_viewer*. This should download the correct textures to the correct location.

If CS Source textures are missing, they can be found elsewhere online.

## Compilation
In Hammer, select File -> Run Map. Choose normal options for everything, but select *HDR* and *Don't run the game after compiling*.  Click ok and it will compile. After this, check the compiled map is in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/maps/de_supermarkt.bsp*. You should be able to then run the map in GMOD using the in-game console command *map de_supermarkt.bsp*.

## de_supermarkt
This is a custom map, originally made for CS:GO, but being adapted for Garry's Mod.
