# de_supermarkt
This is a custom map, originally made for CS:GO, but being adapted for Garry's Mod.

The steam workshop listing is: https://steamcommunity.com/sharedfiles/filedetails/?id=3443674966

## Adding the correct texture paths
This map uses textures from both CS:GO, and CS Source. To add the correct paths for these in Hammer, firstly, use the *mount.cfg* template provided to update the file in your GMOD folder. It needs to reference the texture folders of both games. 

 - The *mount.cfg* file is found in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/cfg*
 - In the mount file, CSGO directory follows *{STEAMAPPSFOLDER}/common/Counter-Strike Global Offensive/csgo*
 - CS Source directory follows *{STEAMAPPSFOLDER}/common/counter-strike source/cstrike*

Next, the custom models need to be added to the correct directory. Add the content in *custom_assets/{maps, materials, resource}* folders to your folders of the same name, in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/{maps, materials, resource}*

Next, launch Hammer. If there are still textures and models missing, it may be missing textures from CSGO, that were lost from the move to CS2. From Steam, navigate to CS2->Properties-> Betas, then opt in to *csgo_legacy*, and *csgo_viewer*. This should download the correct textures to the correct location.

If CS Source textures are missing, they can be found elsewhere online.

## Compilation
In Hammer, select File -> Run Map. Choose normal options for everything, but select *HDR* and *Don't run the game after compiling*.  Click ok and it will compile. After this, check the compiled map is in *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/maps/de_supermarkt.bsp*. You should be able to then run the map in GMOD using the in-game console command *map de_supermarkt.bsp*.

## TTT Specific
*ttt.fgd* needs to be added to the *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/materials* folder, before going into *tools->options->Game Data Files* and adding the TTT fgd file we just put in the materials file. This will let you see the correct TTT objects in hammer.

## Custom Particle Effects
There are a few custom particle effects, in *custom_assets/particles/...*. To enable these to work correctly in your game, you need to add the particle *.pcf* to the folder *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/particles*. Then add references to the *particles_manifest.txt*, using the same style as the one in this repository.

For example:
  -  *custom_assets/particles/de_supermarkt/particles.pcf* is copied to *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/particles/de_supermarkt/particles.pcf*
  -  The line *"file"		"particles/de_supermarkt/particles.pcf"* is added to *{STEAMAPPSFOLDER}/common/GarrysMod/garrysmod/particles/particles_manifest.txt*
