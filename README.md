# Unofficial Ostim Community Modlist

This is a relatively lightweight modlist made for mid range computers. Most textures are 1-2k, with only skin textures and a few misc items that you will rarely see being 4k. The lowest my FPS dropped was around 50 in Falkreath. My system specs are: Ryzen 5 5600g, RX6600 8gb, and 16gbs of ram @ 2900 mhz. The only hard requirement is a CPU that supports at least AVX2.

This modlist should only require an installation of Skyrim SE through the Steam store, without any modifications done to the files that come stock with the game. If you have done any modifications to the base game files, you can validate your game through the steam store by right clicking the game -> properties > local files -> > verify integrity of game files. Alternatively, you can completely uninstall the game and all related folders and files, and reinstall it through Steam. 

The textures included are compatible with ENB Complex Parallax. While its not a huge performance hit, its still turned off by default in this list's pre-packaged ENB. To enable it, right click Rudy - Zandgar Edit (bottom of the [root] seperator) -> open in explorer -> root -> enbseries.ini
Scroll down, just above [COLORCORRECTION] youll see the following lines

EnableTerrainParallax=false
EnableComplexGrass=true
EnableComplexGrassCollisions=true
EnableTerrainBlending=true
EnableComplexParallax=false
EnableComplexParallaxShadows=true
EnableComplexTerrainParallax=false
EnableComplexTerrainParallaxShadows=true

change them to look like the following

EnableTerrainParallax=false
EnableComplexGrass=true
EnableComplexGrassCollisions=true
EnableTerrainBlending=true
EnableComplexParallax=true
EnableComplexParallaxShadows=true
EnableComplexTerrainParallax=true
EnableComplexTerrainParallaxShadows=true

Pre-generated LODs are not included, both for performance reasons, and because we fully expect, and encourage you to add to this list. If you wish to generate your own LODs, make sure you disable everything in the [Flat World Map Framework] seperator before you do. After youre done generating, you can re-enable FWMF, but make sure you keep everything there *below* DynDOLOD and Occlusions in the load order. Your load order should look like this

1. DynDOLOD
2. Occlusions
3. FWMF for Fantasy Paper Maps
4. Additional FWMF Maps

If you do decide to change weather and enb, make sure you disable [Rudy - Zandgar Edit] and [Rudy ENB Cathedral Weathers ADDONS and REQUiRED Files] in the mod organizer. You can either install your prefered ENB through the mod organizer (recommended), or by going to the Skyrim Special Edition 1.6.353 directory in the MO2 Portable Profile. If you want to use NAT, Azurite, Vivid Weathers, or Aequinoctium, you need to re-install [Flat World Map Framework] and select
1. Flat Map Markers AE (1.6.353)
2. All Skyrim Maps + DLCs + Worldspace Mods
3. FWMF for Fantasy Paper Maps
4. Weather overhauls requiring a patch + Yes on Water for ENB
5. And Yes to ELVAS fix (beta)

Your load order needs to be adjusted to 

DynDOLOD (If you did generate your own LODS)
Occlusions (If you did generate your own LODS)
FWMF for Fantasy Paper Maps
FWMF Weather Patch
Additional FWMF maps
