repo for game settings for adding support for different games for [SimpleModManager](https://github.com/ConfuzzedCat/SimpleModManager)

Example:
```jsonc
{
    "Id" : "cyberpunk2077", // nexusmods id for the game: https://www.nexusmods.com/<gameid>/mods/<modid>
    "Name" : "Cyberpunk 2077", // Display name
    "SteamId" : "1091500", // steamid for the game
    "ModStructures" : [ // for handling mods with no folder structures
        {
            "ModPath" : "archive/pc/mod", // where to place the file
            "FileExtensions" : [".xl", ".archive"] // the extension found
        },
        {
            "ModPath": "r6/scripts", 
            "FileExtensions": [".reds"]
        },
        {
            "ModPath": "red4ext/plugins", 
            "FileExtensions": [] // leave empty for mods that uses folders
        },
        {
            "ModPath": "bin/x64/plugins/cyber_engine_tweaks/mods",
            "FileExtensions": []
        },
     	{
            "ModPath": "bin/x64/plugins/cyber_engine_tweaks",
            "FileExtensions": [".asi"]
        }
    ]
}

```