# Preface
Hello to whoever is reading this. Same as BossHud, this is just a documentation of everything that has been changed so it's easier to keep track of what's going on. I'll update this as time goes on with what has been changed and improved. The main difference between this and BossHud's changed logs is that there is still a lot of room for changes/improvements so there will be a dedicated section talking about the roadmap for the plugin.

# Contributors
- [LuqS](https://steamcommunity.com/id/LuqSGood)
    - Creator of the plugin for Zeddy
- [tilgep](https://steamcommunity.com/id/tilgep/)
- [koen](https://steamcommunity.com/id/fungame1224/)

# Roadplan / Changes Planned
- [x] Update code to SM 1.11 syntax and fix compilation errors/warnings
- [x] Move leader plugin messages to a dedicated translation file for easier customizeability
- [x] Update the Hint Message when leader places a marker
- [x] Implementation of a Steam group system to give dedicated leaders in the community access to !leader
- [x] Reword/Rephrase plugin messages as well as updating colors
- [x] Create dedicated commands for placing markers (eg. `sm_mark`)
- [x] Improve the leader menu (reorganize the menu, add more information)
- [ ] Change marker system to be more clear and be attachable to entities/props so it stays on the prop
- [ ] Rework marker type
- [x] Fix markers being placed on teammates
- [x] Fix markers not being able to be placed on certain surfaces
- [x] Add an option to toggle the glow outline on leaders
- [x] Add Dynamic Channels support for the Hud Hint that displays when given leader
- [x] Add more settings/control over the hud hint due to `game_text` shenanigans
- [x] Add commands to directly place markers
- [x] `sm_leader` opens up leader menu if client is already a leader
- [x] Add an option to toggle the overhead sprite on leaders

# Changelog
- 1.0 (tilgep)
    - *(Version of the plugin that was given to me)*
    - Fixed an issue where markers were put on teammates instead of through them
- 1.1 (koen)
    - Moved plugin messages to a separate translation file
    - Rephrased and changed several plugin message and colors
    - Included Dynamic Channels for leader hud hint
    - Added convars for leader hud hint
    - Modified the center text that shows up when leader places markers
    - Fixed compilation warning messages
- 1.2 (koen)
    - Added commands for directly placing markers
    - Reformat plugin
- 1.3 (koen)
    - Minor code formatting for consistency
    - Changed names of certain cvars to match others
    - Added 2 new cvars for controlling if leader outline/sprite can be toggled by leaders
    - Added 4 new cvars for controlling what happens when leader is set (Should beacon/tracers/outline/sprite be enabled when a player is set as the leader?)
    - Rephrased some cvar description for better explanation
    - `sm_leader` will open leader menu if client is already a leader *(tilgep's suggestion)*
    - Added new functions for toggling outline and sprite
    - Reworked leader menu for better display and control
- 1.4 (koen)
    - Implemented SteamWorks for steam group leader access
    - Added several new plugin messages
    - Made `sm_leader` public but added diferent checks in the command callback