[![Releases](https://img.shields.io/github/downloads/sheilan102/C2M/total.svg?style=for-the-badge)](https://github.com/sheilan102/C2M/releases) [![Discord](https://img.shields.io/discord/299813037920223234.svg?color=blue&label=CHAT&logo=discord&style=for-the-badge)](https://discord.gg/JcEvDBH) [![Twitter](https://img.shields.io/badge/-TWITTER-002640.svg?logo=twitter&style=for-the-badge)](https://twitter.com/SHEILANff)
# C2M - A fork of Husky, Call of Duty BSP Extractor.
Since Scobalula said he probably won't ever update Husky, as it was just experimental project, I decided to take over the project and update it with additional features.

With much respect to Scobalula's intial intentions, and all the modders out there, I won't be updating this tool with intentions to improve modding or mapping, but to provide the tools for moviemakers to use the maps in 3d softwares. If any modder finds use in this, I'll be more than happy.

The tool lets you extract map data (map geometry, xmodels, materials & textures) from several CoD games, and import them to Maya with the [import scripts](https://github.com/sheilan102/SHEILAN-Maya-Tools) (C4D & UE on the roadmap).

### Supported Games

* Call of Duty: Modern Warfare
* Call of Duty: Modern Warfare 2
* Call of Duty: Modern Warfare 3
* Call of Duty: Ghosts
* Call of Duty: Infinite Warfare
* Call of Duty: World at War
* Call of Duty: Black Ops
* Call of Duty: Black Ops 2
* Call of Duty: Advanced Warfare
* Call of DUty: World War 2
* Call of Duty: Modern Warfare Remastered


### Downloading/Using C2M

To download C2M, go to the [Releases](https://github.com/sheilan102/C2M/releases) and download the latest build.

To use C2M, simply run the game, load the map you want to extract, and run C2M, then click the paper airplane to export the loaded map. In some cases you may need to run C2M as an administator.

### Features

* Map terrain/geometry - **mapname**.obj
* OBJ Material - **mapname**.mtl
* Map file with models locations and rotations - **mapname**.map
* A search string of all images used for Wraith/Greyhound - **mapname**_search_string.txt
* A search string of all XModels used for Wraith/Greyhound - **mapname**_xmodelList.txt
* JSON file with model data for scripts to load & place models in 3d softwares - **mapname**_xmodels.json
* JSON file with material data - **mapname**_matdata.json
* Map entities (worldspawn settings, dynamic models & scripts) - **mapname**_mapEnts.txt
#### # mapEnts currently supported in
    COD4
    WAW
    MW2
    BO2
    AW

If you wish to use textures (be warned they can result in high RAM usage) then make sure to have the _images folder (use Wraith/Greyhound to export the required images) in the same location as the obj/mtl file and export PNGs (do not ask for other formats, it's staying as PNG, do a find/replace if you want to use other formats).

### License/Disclaimers

C2M is licensed under the GPL license and it and its source code is free to use and modify under the terms of the GPL. C2M comes with NO warranty, any damages caused are solely the responsibility of the user. See the LICENSE file for more information.

**All** BSP data extracted using C2M is property of the developers, etc. and with this in mind you need to understand the limitation of what you can do with the data. C2M simply parses it out, what you do with it, is your responsibility.

Some of the exported models can get pretty big. While all have loaded in Maya with no issue, make sure to have available resources available to load and view them.

## FAQ

* Q: C2M says it cannot find my game?

* A: Check the above list for a supported game, when searching for a supported game, C2M loops over all processes and stops at the first match, if it's not finding your game and it is supported, your exe is not the same name as what C2M expects or something is blocking .NET from returning its process.

* Q: C2M says my game is not supported?

* A: I verify the addresses on legitimate up to date copies of the supported games in the English locale. If you're using a modified executable (Pirated, etc.) I will not support it.

* Q: The exported OBJ is corrupt when imported?

* A: Tons of BSPs across all supported games have been verified, if you have find a legitimate instance of a corrupt export, please open an issue with the name of the map, etc. as much info as you can.

## Credits

* SHEILAN - Developer, game research.
* [Scobalula](https://github.com/Scobalula) - Original dev of the project, game research.
* [DTZxPorter](https://github.com/dtzxporter) - Normal Unpacking Code from Wraith, Half Floats code, Other misc info from Wraith.
* [Icon](https://www.freeiconspng.com/downloadimg/37219)

If you use C2M in any of your projects, it would be appreciated if you provide credit for its use, a lot of time and work went into developing it and a simple credit isn't too much to ask for.

## BUG REPORT

If you encounter any issue, or just want to suggest an idea, feel free to do it via issues for this repository or through one of the following sites.

[![twitter](icons/icon_twitter.svg)](https://twitter.com/SHEILANff)   [![youtube](icons/icon_youtube.svg)](https://www.youtube.com/user/kalaboKKz)
