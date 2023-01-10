
# Warning! This is not the official repository

After some discussiong with the server manager, I believe it is better that I put it straight forward that what I do here is **NOT** the official repository and does not reflect the decisions of Zeddy and Detroid. I am doing this with the intentions on helping others and make playing on Zeddy for new players much easier. This is solely **MY** own project and not zeddy's, thus do not expect everything to be up to date.

## Additional Information

All map cycle related files are not updated frequently here! I will try my best to get updates and information, but there is no guarantee that everything here is the latest.

## Entwatch, Stripper, and BossHud config information

After much heated discussion and consideration, I have decided I will **NOT** be making all the configs public.

## How to Contribute to Song Name Configs

To contribute to song names, you can either:

1. Join our Discord server and head to the forum channel dedicated to submitting song names
2. Message me directly on discord *(koen#4977)* with your files
3. Make a GitHub pull request on this repository

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
