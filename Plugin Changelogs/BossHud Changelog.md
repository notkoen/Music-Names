# Quick Preface:
Hello to whoever is/will read this in the future. I am making this file because I want to stop using `_test#` versions for boss hud changes anymore. Mainly for clarity reasons and to keep the scripting folder **clean**. No, I am not removing stuff and such, I am simply just making a separate doc to clearly list changes.

**Note:** Unfortunately, a lot of the change logs for older versions were either lost, or changes were not properly documented. 

# Contributors:
- [Antiteal/Strellic](https://steamcommunity.com/id/Strellic/)
    - The original creator of the boss hud plugin ([Original AM Post](https://forums.alliedmods.net/showthread.php?p=2559019))
    - Made a lot of improvements and changes for zeddy
- [tilgep](https://steamcommunity.com/id/tilgep/)
    - The person that added a lot of the modern features that Antiteal did not add into the plugin
    - Features added: `MultBoss`, Boss Damage Info, ETA kill time *(Deprecated)*, multiple hitmarker option, New HP bar display
    - General plugin improvements/optimization as well as testing/fixing bugs
- [koen](https://steamcommunity.com/id/fungame1224/)
    - Focused on making minor changes and updates to the plugin
- [CrazyKid](https://steamcommunity.com/id/crazy-kid/)
    - Creator of the popular BossHud plugin used on PSE, GFL, and most notably, ZED. Many features of the current BossHud plugin were taken from his plugin or inspired by his plugin

# Change Log
## Zeddy Bhud 1
- *no changelogs properly documented*
## Zeddy Bhud 2
- Check changelogs [here](https://forums.alliedmods.net/showthread.php?p=2559019)
## Zeddy Bhud 3
- Minor formatting changes to display
## Zeddy Bhud 4
- **4.0**
    - Added `MultBoss` feature
    - Added ETA timer
- **4.1**
    - Optimized ETA timer to use Spxctator's suggestion: average ETA timer between the last 3 ticks to get a more average timer
    - Removed overlay hitmarkers in favor of `game_text` hitmarkers
- **4.2**
    - Added support for multiple hitmarkers that clients can customize
    - Shooting bosses add to assists
    - Added one more color to HP display
## Zeddy BossHud 5
- *Renamed plugin*
- **5.0**
    - Rework of internal stuff (I don't know the details)
- **5.1.0**
    - Added damage rank info
    - Added check to prevent double cookie loading
    - Compacted top level cookie menu options
    - Added option to toggle bhud from cookie menu
    - Toggle hud command now works when cookies aren't loaded
    - Fixed hitmarker cookie not existing
- **5.1.2**
    - Fixed simpleHUD not displaying
    - Fixed boss death hintbox not showing properly (Top Boss Damage)
- **5.1.3**
    - Added new hitmarker styles
    - Added options to change hitmarkers
- **5.1.4**
    - Fixed new hitmarker styles not displaying properly
    - Removed ETA timer due to being unnecessary
    - Moved HUD display into translations for easier customization
## Zeddy BossHud Redux
- *Last Plugin Rename*
- **1.0.0**
    - Made hitmarker and boss damage info to display together in one channel
    - Added colour cookie for hitmarker/damage info
    - Fixed issue where hit count is off by 1 (Usually when entering boss room)
    - HitMarkerOnly now works for breakables larger than `MAX_BREAKABLE_HP`
    - *(Some other fixes that tilgep forgot to put down)*
- **1.0.1**
    - Removed Zombie:Reloaded depency from zombie hitmarkers to allow BossHud to work without Z:R plugin
    - Reworked BossHud display formatting
- **1.0.2**
    - Removed some unused/deprecated shit in the code
    - Code formatting and changes
- **1.1.0**
    - Added `RewardMoney` option to disable earning money/assists when shooting entities in the config (useful for breakable triggers)
    - Removed `MultHP` option and make the plugin autoreload the entity config immediately
    - A stupid shit hack to get money/assists working for `HitmarkerOnly` option (boss damage info won't show unfortunately)
- **1.2.0**
    - Reworked `MultHP` option: Readded the option back for configs so plugin will immediately reload only if the option is set (Having it auto-reload was causing issues with display for other maps)
    - Some more code formatting and comments
    - Re-added Zombie:Reloaded dependency so hitmarkers will show properly (Some edge cases where hitmarkers would show up for zombies :/)
    - Reworked `MultBoss` display to show percentage
- **1.2.1**
    - Revert percentage display back to integers
    - Revert HP color to just 3 different color indicators
    - Force all non-segmented bosses to show up with 12 HP bars
- **1.2.2**
    - Reworked the HP reset feature to not be as aggressive when resetting
    - Revert grey HP bar display to save space for more HP bars
