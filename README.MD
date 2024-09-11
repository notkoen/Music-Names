
# Music Names

This repository stores music name and lyric configs for Zombie Escape and Zombie Survival maps. These configs are currently used on [Sunrust](https://sunrust.org/).

> [!NOTE]
> Music configs under the `legacy` folder were configs used on zeddy's, which followed an old config format. Only use this folder to find names of music.

## How to Contribute

Various way of contributing:

1. Join the [Sunrust discord server](https://discord.gg/sunrust) and send the files in the [#zs-content-creation](https://discord.com/channels/353474260112769026/495994723559931915) channel
2. Message me directly on discord (*notkoen*)
3. Make a pull request

> [!NOTE]
> There is currently a `10,000` ember bounty for each config made

## Config Formatting

### Music Name

```yaml
"music"
{
    "filename.mp3" "Artist - Title"
    "level1_boss.mp3" "Pendulum - The Tempest (Live at Brixton Academy)"
    "level2_boss.mp3" "Pendulum - Slam"
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

> [!CAUTION]
> File extensions must be **included** *(such as `.mp3`)* for music to be detected and displayed

> [!CAUTION]
> File names must be **lowercase**

- Follow `<Artist> - <Song Title>` format
- Use `//` to add comments to configs
- Add extra song details if needed (e.g. `"Pendulum - The Tempest (Live at Brixton Academy)"`)
- Song names in other languages are fine, but try to keep english names if there is one
- For files that contain multiple songs, please follow this format: `Artist - Title 1, Artist 2 - Title 2, Artist 3 - Title 3` and so on
- Custom music added externally should also be included (may require further access to stripper configs)

## Special Thanks

- [tilgep](https://github.com/tilgep) for the idea and making the original plugin
- [Detroid/rynerwolf](https://github.com/RynerWolf) for managing zeddy and allowing me to maintain these configs
- [Snowy](https://github.com/snorux) for making the tool to port zeddy configs to GFL
- *Bomberman*, *Haruka*, *Hibiki*, *Detroid/RynerWolf*, *Heavy*, *Kiriya*, *DVC*, *Watdoink*, *Chong0074*, *WhiteCat*, *kun*, *Owlfy*, *Cylops*, *tapch0w*, *Chinny*, *BAN*, *Tsukasa*, *FroZRil*, *kaomunkai*, *KingMagress*, *Hichatu*, *tilgep*, *WILD BANAN*, *TuPu*, *Beppu*, *Sprinuts*, *ShiroNeko*, *Berke* for making the original configs used on zeddy
