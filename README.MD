
# Music Names

This repository stores music name and lyric configs for Zombie Escape and Zombie Survival maps.

> [!NOTE]
> Music configs under the `legacy` folder were configs used on zeddy's, which followed an old config format.

## How to Contribute

1. Message me directly on discord (*notkoen*)
2. Make a pull request

## Config Formatting

### Music Name

**CS:S/Gmod configs:**

> [!CAUTION]
> File extensions must be **included** *(such as `.mp3`)* for music to be detected and displayed

> [!CAUTION]
> File names must be **lowercase**

```yaml
"music"
{
    "filename.mp3" "Artist - Title"
    "level1_boss.mp3" "Pendulum - The Tempest (Live at Brixton Academy)"
    "level2_boss.mp3" "Pendulum - Slam"
}
```

**CS2 configs:**

> [!CAUTION]
> CS2 configs use **sound events** instead of sound files to match and display names. Use [Source2Viewer](https://valveresourceformat.github.io/) to open maps and find the `.vsndevts_c` file to see all the sound events.

```jsonc
{
    "SoundEvent1": "Artist - Song Title",
    "SoundEvent2": "Artist 2 - Song Title 2, Artist 3 - Song Title 3",
    "SOundEvent3": "Artist 3 - Song Title 4/Song Title 5/Song Title 6"
}
```

### Lyrics

```lua
GM.ZELyrics = {
    ["filename.mp3"] = {
        {time = 1.0, text = "Example of lyric at 1 second"},
        {time = 2.4, text = "Example of lyric at 2.4 seconds"},
        {time = 3.0, text = "Example of holding text until next lyric shows up", autohold = true},
        {time = 5.0, text = "This text will clear previous text at 5.0 seconds,"},
    },
    ["filename2.mp3"] = {
        {time = 1.0, text = "Example of a second song and lyrics"},
        {time = 3.0, text = "Put as many text for any lyrics"},
    },
}
```

## Config Guidelines

- Follow `<Artist> - <Song Title>` format
- Use `//` to add comments to configs
- Add extra song details if needed (e.g. `"Pendulum - The Tempest (Live at Brixton Academy)"`)
- Song names in other languages are fine, but try to keep english names if there is one
- For files that contain multiple songs, please follow this format: `Artist - Title 1, Artist 2 - Title 2, Artist 3 - Title 3` and so on

## Special Thanks

- [tilgep](https://github.com/tilgep) for the idea and making the original plugin
- [Detroid/rynerwolf](https://github.com/RynerWolf) for managing zeddy and allowing me to maintain these configs
- [Snowy](https://github.com/snorux) for making the tool to port zeddy configs to GFL format
- [When](https://github.com/whennya) for being a cutie and making/updating a lot of configs
- *Bomberman*, *Haruka*, *Hibiki*, *Detroid/RynerWolf*, *Heavy*, *Kiriya*, *DVC*, *Watdoink*, *Chong0074*, *WhiteCat*, *kun*, *Owlfy*, *Cylops*, *tapch0w*, *Chinny*, *BAN*, *Tsukasa*, *FroZRil*, *kaomunkai*, *KingMagress*, *Hichatu*, *tilgep*, *WILD BANAN*, *TuPu*, *Beppu*, *Sprinuts*, *ShiroNeko*, and *Berke* for making the original configs used on zeddy
