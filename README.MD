
# Song Name Configs

All song name configs used on Zeddy's Zombie Escape server. These song name configs are only compatible with `Map Music Control Interface (v4.2.3)`. If you wish to convert too GFL's song name format, you can use this [tool](https://github.com/snooooowy/music-config-parser) written by Snowy.

## How to Contribute

To contribute, you can either:

1. Join our [Discord server](https://discord.gg/zeddysze) and head to the forum channel dedicated to submitting song names
2. Message me directly on discord *(not koen#4977)* with your files
3. Make a GitHub pull request on this repository

## Config Guidelines

Make sure to follow the song name config format:

```yaml
// Comments are allowed
<full path to song name>.<extension>||<song name>
bestmap/songs/extreme/ab_cd_efgh.mp3||Some Shitty Artist - Some Shitty Song
```

Importan guidelines to follow when making song name configs:

- **Always** exclude the first `sound/` folder and just follow the directory after it
- Use `/` when there are subfolders (back slash can cause issues)
- Make sure to include the file extension (`.mp3` or `.wav`)
- Follow `<Artist> - <Song Title>` format
- You can use // to add comments to configs
- Do not leave spaces before and after the `||`
- Do not add extra song details (eg. `[Official Audio]`), just put the name.
- Song names in other languages are fine, but try to keep english names if there is one
- For files that contain multiple songs, please follow this format: `Artist - Title 1, Artist 2 - Title 2, Artist 3 - Title 3` (use a comma to separate them)
- Try to upload song configs for the latest maps (older version configs are accepted)
- Custom RTV stage music should also be added (these you cannot find the location without either the stripper or looking into your songs folder)
