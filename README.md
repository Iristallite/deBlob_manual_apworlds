# deBlob_manual_apworlds
Manual apworlds for the de Blob Series, made with [Manual for Archipelago](https://github.com/ManualForArchipelago/Manual).

# How do I use this?
I will refer you to the offical [Archipelago setup guide](https://archipelago.gg/tutorial/Archipelago/setup_en) for how to set up Archipelago.

Use the `Install APWorld` option in the Archipelago launcher to install the `.apworld` files from the [Releases tab](https://github.com/Iristallite/deBlob_manual_apworlds/releases/latest)  
I have also provided some template `.yaml` files with the release.  
<sup>You can also just grab the `.apworld` and `.yaml` files from the folders, but I'd recommend sticking to the Releases for simplicity's sake.</sup>

# What's a *de Blob?*

<center>
  <img
    src=".deBlob12.png"
    alt="de Blob and de Blob 2 copyright 2008-2011 THQ Nordic GmbH"
    width=50%
    height=50%
  ></img><br>
  <sup><b>de Blob</b> and <b>de Blob 2</b> copyright 2008, 2011 THQ Nordic GmbH</sup><br>
</center>

de Blob and de Blob 2 are 3D platformers all about color!<sup>[sic][^1]</sup>  
<sup>I'm sorry if you're colorblind.</sup>

de Blob 1 is more open-ended; you can complete level challenges in any order, and the only thing blocking the exit is your score.  
de Blob 2 is more story-driven; you have to complete each level's missions in order.<sup>...unless you use speedrun skips</sup>  
de Blob 2 (DS/i) is a linear 2D platformer that still retains some gameplay elements from the console games.
# Where can I get the games?
* de Blob 1: [Steam](https://store.steampowered.com/app/532320/de_Blob), [GOG](https://gog.com/game/de_blob), [Switch](https://nintendo.com/store/products/de-blob-switch), [Xbox One](https://xbox.com/games/store/de-blob/c092flk91x41), [PS4](https://store.playstation.com/product/UP4389-CUSA09934_00-DEBLOBONEUS00001), Wii<sup>[^2]</sup>
* de Blob 2 (DS/DSi): Unfortunately you'll need to find a second-hand cartridge for this one.
* de Blob 2: [Steam](https://store.steampowered.com/app/563190/de_Blob_2), [GOG](https://www.gog.com/game/de_blob_2), [Switch](https://nintendo.com/store/products/de-blob-2-switch), [Xbox 360](https://xbox.com/games/store/de-blob-2/btzcngwlqpz0)<sup>[^3]</sup>, [Xbox One](https://xbox.com/games/store/de-blob-2/c360xv52r4nl), [PS4](https://store.playstation.com/product/UP4389-CUSA10447_00-DEBLOB2US0000001), PS3<sup>[^4]</sup>
* de Blob 1 (DS): It never released.<sup>[^5]</sup>
* de Blob 1 (Mobile): Possibly delisted?<sup>[^6]</sup> There is an `.apk` of the Android version floating around online though. Maybe I'll do it someday?
* de Blob Revolution: Exclusive to 32-bit iOS<sup>[^7]</sup> and *Windows Phone,* the latter of which I *somehow* have an `.xap` for, but I can't sideload it onto my HTC 8X because nobody cares about non-Lumia Windows Phones.
* There is also a [Steam bundle](https://store.steampowered.com/bundle/44665/de_Blob_Bundle/) of de Blob 1 and de Blob 2.

# How does this manual apworld work, exactly?
...It doesn't! At least in terms of connecting to the game.<sup>well, duh, it's a *manual* apworld</sup>  
More seriously, you'll have to rely on 100% save files <sup>([dB1](https://www.speedrun.com/de_Blob/resources/m5gk0), [dB2](https://www.speedrun.com/dB2/resources/ezw7w), [dB2 DS](https://www.speedrun.com/db2ds/resources/iix74))</sup> and/or [ingame cheats](#ingame-cheats) to affect the game directly.  
This apworld shuffles each level as an item, as well as a specific amount of "McGuffins" that you'll need to open the final level(s).  
In addition, there are some traps, cheats, upgrades (dB2), and some extra-special *diabolical traps* that are sure to ruin your day... if you're playing in a sync multiworld.<sup>...receiving a "Restart Level" when you're playing a different game... entirely defeats the point, eh?</sup>  
Also there's DeathLink if you're into that.
# Wait, how does DeathLink work in a manual?
1. Locate the nearest source of damage or bottomless pit
2. Touch it until Blob dies and loses a life
3. Acknowledge you have received the deathlink by pressing the button in the client
4. If you continue from a game over in dB2, you should probably say goodbye to your S rank  
If you die accidentally, *you* send a deathlink to everyone else
# de Blob 1: Options
* `levels_shuffled`: Shuffle all levels as items.  
This mode is recommended for solo-slot and multiworld play.  
* `levels_progressive`: Shuffle 30 "Progressive Level" items that unlock the levels in order.  
This mode is only recommended if you want to integrate a standard playthrough of *de Blob* into an Archipelago multiworld.  
* `traps_30fps`: Enable/disable the `High-Performance Ink` trap item.  
Please disable this if you don't have any way to change the FPS limit mid-game. (ie: Gamescope on Linux or [Special K](https://www.special-k.info/) on Windows)  
<sup>PS: SteamOS/Bazzite's "gaming mode" ***is*** gamescope.</sup>  
* `traps_restart_level`: Enable/disable the diabolical `Restart Level` trap item.  
It might be a good idea to disable this in an async multiworld, because otherwise if you aren't playing when you receive it... nothing happens.
* `traps_broken_brakes`: Enable/disable the `Broken Brakes` trap item.
* `traps_invert_camera`: Enable/disable the `Invert Camera` trap item.
* `traps_mute_music`: Enable/disable the `Free Lossless Ink Codec` trap item.
* `sinking_feeling`: Add/remove level 10-2 (Sinking Feeling), as it is incredibly difficult without turbo or Wiimote/Nunchuk shaking...  
...and impossible at 30fps, which is what the Switch version runs at in handheld mode. <sup>I get the feeling THQ Nordic rushed Blitworks a bit too much...</sup>  
Only applies to shuffled level mode, as 10-2 and 10-3 are excluded in progressive mode.  
* `cheats_time_bonus`: Enable/disable the `Time Bonus` cheat item.
* `cheats_extra_life`: Enable/disable the `Extra Life` cheat item.
* `cheats_invulnerability`: Enable/disable the `Temporary Invulnerability` cheat item.
# de Blob 1: Checks
* `Level Complete`: Complete the level.  
For Bonus Levels (`X-2`/`X-3`), I have arbitraily decided that you need to get a Gold Medal. You *can* ignore this, but I'll frown at you.
* `Gold Medal`: Self-explanatory.
* `100% Painted`: Paint *everything* in the level. If you can't find the last thing, try holding the Compass button!
* `Challenger`: Complete all *Challenges* within the level. This usually also gets you the `Architect` check (Landmarks Award) as well.
* `Speedrunner`: Beat the target *Time* listed under `(Main Menu) --> EXTRAS --> AWARDS --> (LEVEL)`. Stringing together combos is the key!
* `Stylist`: What a *style!* Collect them all!
* `Naturalist`: Save the *trees!* Restore them all!
* `Architect`: Shake! Shake! Shake! Restore all the *landmarks* INKT has defaced!
* `Street Artist`: You hate advertising, don't you? Tag all the *billboards!*
* `Transformer`: Optimus Paint Engine.  
Activate all the *Transform* Engines in each level; they spawn at certain Score intervals, and will always interrupt you with a skippable cutscene when they do.  
<sup>Yes, "Optimus Paint Engine." is the actual description of the trophy (called Transformers, I might add) that you get for doing this in every level.</sup>
* `Liberator`: They may take away our color, but they'll never take away our freedom!  
Free all the *Raydians* in each level from the Graydian suits the INKT Corporation has locked them in!
* `Blimp Painted`: To *blimp* and beyond!  
At certain points in each level, the Color Underground's *blimp* will appear. Tag it for a check!  
<sub>A bunch of these are references to the trophy descriptions in the HD re-release.</sub>
# de Blob 1: Items
#### Levels
* `Progressive Level`: 30 available. If you have 4, you can play 1-1, 1-2, 1-3, and 2-1.  
Only available when `levels_progressive` is set to `true`.  
* `X-X: LevelName`: Should be obvious. I'm not going to list all 29 of them.  
Note: `X-1` is the main level, while `X-2` and `X-3` are "Bonus Missions".  
Only available when `levels_shuffled` is set to `true`.  
#### McGuffins
McGuffins are only applicable when `levels_shuffled` is set to `true`.
* `Comrade Black's Blueprints`: `9` out of `12` required to access `10-1 (Lake Raydia)` and beat the game.  
#### Traps
All trap items can be individually removed via yaml settings.
* `Restart Level`: Press the `RESTART` button in the pause menu to restart the level. <sup>...Diabolical.</sup>
* `High-Performance Ink`: Cap the game at 30fps for 5 minutes.  
**If you're unable to change the FPS cap without restarting the game, you should probably remove it.**
* `Broken Brakes`: For 5 minutes, you are not allowed to press Brake (`B`/`R2`/`RT`/`ZR`) to brake in mid-air.   
<sup>...wow that's a lot of different buttons</sup>  
You are still allowed to press Brake to crouch while on solid ground.  
* `Invert Camera`: Change the "Invert Camera" option, and change it back when you get another.  
There's an even amount, so you'll loop back around to your preference eventually.
* `Free Lossless Ink Codec`: Turn the Music volume down to 0 for 2 minutes, then turn it back up.
#### Cheats
All cheat items can be individually removed via yaml settings.
* `Time Bonus`: Self-explanatory, refer to the table below.
* `Extra Life`: Self-explanatory, refer to the table below.
* `Temporary Invulnerability`: Each `Temporary Invulnerability` item is worth 30 seconds of the "Invulnerability" cheat being turned on.  
If you're not playing the Wii version, the cheat activation text is flipped vertically... for some reason?  
As an example, you can use 2 of them together for 1 minute of invulnerability.  
As an example of how you could use this *cleverly*, you can skip a certain section of `9-1 (Ministry of Ink)` by swimming through a pool of Ink while Invulnerability is on.
#### Shiny Filler
* `Color Wheel`: Named after the slightly uncommon collectible worth 1000 points, unfortunately this does nothing... but there are only `6` of them!~
# de Blob 2 (DS): Options
* `levels_shuffled`: Shuffle all levels as items.  
This mode is recommended for solo-slot and multiworld play.  
* `levels_progressive`: Shuffle 31 "Progressive Level" items that unlock the levels in order.  
This mode is only recommended if you want to integrate a standard playthrough of *de Blob 2 (DS)* into an Archipelago multiworld.  
* `dsi_enhanced`: Activate DSi Enhanced mode, adding 15 more checks - the DSi-exclusive Chroma Camera collectibles!  
* `cheats_chroma_crystal`: Enable/disable the `Chroma Crystal` cheat item. **REQUIRES DSi ENHANCED MODE**
* `traps_256x192`: Enable/disable the `High-Resolution Ink` trap item.  
Please disable this if you plan to play entirely on console.
* `traps_restart_level`: Enable/disable the *diabolical* `Restart Level` trap item.  
It might be a good idea to disable this in an async multiworld, because otherwise if you aren't playing when you receive it... nothing happens.
# de Blob 2 (DS): Checks
* `Level Complete`: Complete the level.<sup>...pretty self-explanatory. again.</sup>
* `Musical Collector`: Maybe collecting the *3 big music notes* will save this game's terrible audio quality? <sup>It won't.</sup>
* `Liberator`: Rescue all the Raydians!
* `Chroma Camera`: Only present on certain levels, these do... well, nothing if they've already been collected on the save, otherwise you get a stupid but charming camera-gimmick minigame.  
The `Chroma Camera` checks are only available when `dsi_enhanced` is set to `true`.
Unfortunately, dB2 DS doesn't reset the in-level progress trackers if you replay from a 100% save, so... bust out the pen and paper!
# de Blob 2 (DS): Items
#### Levels
* `X-X: LevelName`: Should be obvious. I'm not going to list all 30 of them.  
Only available when `levels_shuffled` is set to true.  
* `Progressive Level`: Each world has 5 levels, so if you have 7 `Progressive Level`, you can play up to level 2-2.  
Only available when `levels_progressive` is set to true.  
#### McGuffins  
McGuffins are only applicable when `levels_progressive` is set to true.  
* `Rocket Parts`: `30` out of `36` required to access `7-1 (The Final Showdown)` and beat the game.  
#### Traps  
All trap items can be individually removed via yaml settings.
* `High-Resolution Ink`: Lower the internal resolution to 1x for the duration of the next level, or play the next level on console.  
**If you're playing on a real console or not increasing the emulated IR, *remove this item.***
* `Restart Level`: Press the `RESTART` button in the pause menu to restart the level. <sup>...Diabolical.</sup>  
#### Cheats
* `Chroma Crystal`: `dsi_enhanced` only, press SELECT to choose any color!  
If you misinput and select the wrong one, you get a "grace use" and can try again.
#### Shiny Filler
* `Big Music Note`: Named after the 3 big music notes in each level, unfortunately this does nothing... but there are only `6` of them!~
# de Blob 2: Options
* `levels_shuffled`: Shuffle all levels as items, and lock the final levels behind "McGuffins".  
This mode is recommended for solo-slot and multiworld play.  
* `levels_progressive`: Shuffle 12 "Progressive Level" items that unlock the levels in order.  
This mode is recommended if you wish to integrate a standard-ish playthrough of *de Blob 2* into an Archipelago multiworld.  
* `add_pinky`: Adds the `Pinky` item, which allows the use of 2-player mode.  
`add_pinky` also adds the `Trophies: Pinky to the Rescue` check, earned by activating 2-player mode.  
On console, connect a second controller and press whatever your platform equivalent of the `START` button is.  
On PC, press P on the keyboard, then you can control Pinky with the mouse!  
If you do some clever mapping with a gyro/touchpad-enabled controller, you can probably play as both Blob and Pinky simultaneously, which I imagine has quite some potential!  
I recommend setting this to false unless you have a friend or are playing on PC, where you can map both players to 1 input device.  
The Steam version of *de Blob 2* supports Remote Play Together, so pseudo-online multiplayer is possible.  
* `extra_pinky_x`: Adds up to 3 extra `Pinky` items. Sorry for the jank, I don't know Python.
* `traps_30fps`: Enable/disable the `High-Performance Ink` trap item.
* `traps_restart_checkpoint`: Enable/disable the `Restart Checkpoint` trap item.
* `traps_restart_level`: Enable/disable the `Restart Level` trap item.
* `traps_broken_brakes`: Enable/disable the `Broken Brakes` trap item.
* `traps_invert_camera`: Enable/disable the `Invert Camera` trap item.
* `traps_zap_pinky`: Enable/disable the `Pinky Short-Circuit` trap item.
* `traps_mute_music`: Enable/disable the `Free Lossless Ink Codec` trap item.
* `cheats_time_bonus`: Enable/disable the `Time Bonus` cheat item.
* `cheats_extra_life`: Enable/disable the `Extra Life` cheat item.
* `cheats_armor_refill`: Enable/disable the `Armor Refill` cheat item.
* `cheats_chroma_crystal`: Enable/disable the `Chroma Crystal` cheat item.
# de Blob 2: Checks
* `(LevelName) Liberated`: Not your typical "Level Complete" check; dB2 has a sort of "micro-postgame" in most of its levels!
You can tick off this check once you see the Pinky icon that lets you fast-travel between checkpoints and exit the level.
* `S Rank`: If you do *everything* in each level, (and don't get any Game Overs), you should easily get the S rank.
* `Trophies: Blob Survivor`: Simply complete a level without dying to earn this.<sup>...if you're playing with DeathLink on, *good luck.*</sup>
* `Trophies: Piston Partisan`: In the level `State College`/`Comrade Black U.`, there are a few sections where you can chain together piston jumps. Do 10 in a row for the check!
* `Trophies: Pinky to the Rescue`: This is basically a free check, if it's enabled that is.  
`Trophies: Pinky to the Rescue` is removed if the `shuffle_pinky` yaml setting is set to `false`.
# de Blob 2: Items
* `Progressive Story Level`: The most straightforward version of the item.  
If you have 3, you can play the `Paradise Island`, `Downtown`, and `Blanctown` levels.  
Only available when `levels_progressive` is set to `true`.
* `Paradise Island`, `Downtown`, `Blanctown`, `The Senate`, `State College`, `Soda Falls`, `Hydro Station)`, `House of Fun`, `Orbital Habitats`, `Railyards`: Level unlocks.  
Please note that once `The Senate` is completed, the names on the level select for levels 5-10 (`State College` through `Railyards`) change due to story reasons.  
This only applies if you haven't cleared the respective level, however.  
The alternate names are provided in (brackets) in the manual tracker to prevent confusion.  
Only available when `levels_shuffled` is set to `true`.
#### Upgrades
* `Life Upgrade`: Increases your maximum life count by 1. Probably the least useful upgrade.
* `Size Upgrade`: Increases Blob's maximum size by 20 paint points.
* `Armor Upgrade`: Allows you to carry 1 extra Armor pickup.  
Armor pickups only appear in level 4 (The Senate) and onward.  
^These upgrades have 5 tiers.
* `Charge Upgrade`: Decreases the cost of Blob's charge attack by 20 paint points.
* `Pinky Upgrade`: Increases Pinky's maximum ammo by 50.  
*Not* removed when Pinky is disabled, since it's part of the `Maximum Blob` trophy.  
^These upgrades have 3 tiers.  
In Iris's opinion, the most useful upgrades are the Charge and Size upgrades.  
Base Blob can only charge attack *once* at full size. "Maximum Blob" can do it *ten* times.
#### McGuffins  
McGuffins are only applicable when `levels_shuffled` is set to `true`.
* `Rocket Parts`: `12` out of `16` required to access `Rocket Range` and build the `Color Underground Rocket`.
* `Color Underground Rocket`: Received for completing `Rocket Range`. Required, alongside `7 Color Energy Beams`, to access the final level `Hypno Ray`.
* `Color Energy Beam`: `7` out of `12` required, alongside the `Color Underground Rocket`, to access the final level `Hypno Ray` and beat the game.
#### Traps
All traps can be individually removed via yaml settings.
* `High-Performance Ink`: Cap the game at 30fps for 5 minutes. **If you're unable to change the FPS cap without restarting the game, *remove this item.***
* `Broken Brakes`: For 5 minutes, you are not allowed to press Brake (`B`/`T`/`R2`/`RT`/`ZR`) to brake in mid-air, with two exceptions.  
<sup>...wow that's a lot of different buttons</sup>  
1: You are still allowed to press Brake to crouch while on solid ground.  
2: You are still allowed to press Brake immediately following a Charge Attack, as prevention against the *Launch Glitch.<sup>[^8]</sup>*
* `Invert Camera`: Change the "Invert Camera X/Y" options, and change them back when you get another.  
There's an even amount, so you'll loop back around to your preference eventually.
* `Free Lossless Ink Codec`: Turn the Music volume down to 0 for 2 minutes, then turn it back up.
* `Pinky Short-Circuit`: Bans the use of the second player (Pinky) for 5 minutes. **If you're not playing with Pinky, *remove this.***
* `Restart Checkpoint`: Quit the level and enter it again from the menu. **DO NOT USE THE `RESTART` BUTTON IN THE PAUSE MENU; THAT WILL RESTART THE *ENTIRE LEVEL***
* `Restart Level`: Press the `RESTART` button in the pause menu to restart the level. <sup>...Diabolical.</sup>
If the `Restart Level` trap hits you while the game is closed, you must delete any saved checkpoint data.
#### Cheats
All cheats can be individually removed via yaml settings.
* `Time Bonus`: Self-explanatory, refer to the table below.
* `Extra Life`: Self-explanatory, refer to the table below.
* `Armor Refill`: Self-explanatory, refer to the table below.
* `Chroma Crystal`: Semantics time! One "use" of this allows you to input the cheat *as many times as you need* until you're at the desired color, *then* it's been "used up".
#### Shiny Filler
* `Big Color Atom`: Named after the common collectible worth 1000 points, unfortunately this does nothing... but there are only `3` of them!~

# Ingame Cheats
<a name="ingame-cheats"></a>
The "Cheat" items literally allow you to use ingame cheats!  
You can use each cheat once for each of the corresponding item you have.  
To use a cheat, hold down the Activator and then press the corresponding button sequence.  
`T` and `S` are Triangle and Square buttons respectively.  
The "Unlock All Levels" cheats must be input at the main menu.  
If there's no "Unlock All Levels" cheat for your specific game, here are 100% save files: <sup>([dB1](https://www.speedrun.com/de_Blob/resources/m5gk0), [dB2](https://www.speedrun.com/dB2/resources/ezw7w), [dB2 DS](https://www.speedrun.com/db2ds/resources/iix74))</sup>
dB1 Cheats:
| Console | Activator  | Time Bonus | Extra Life | Invulnerability | Unlock All Levels |
| ------- | ---------- | ---------- | ---------- | --------------- | ----------------- |
| Wii     | C (Nunchuk)| `1 2 1 2`  | `1 1 2 2`  | `1 1 1 1`       | `B B 1 2 1 2 B B` |
| Xbox/PC | View/Back  | `A Y A Y`  | `A A Y Y`  | `A A A A`       | Unknown           |
| PS4     | Touchpad   | `X T X T`  | `X X T T`  | `X X X X`       | Unknown           |
| Switch  | Unknown    | Unknown    | Unknown    | Unknown         | Unknown           |
  
dB2 Cheats:
| Console | Activator  | Time Bonus | Extra Life | Armor Refill | Chroma Crystal (Change Color) | Unlock All Levels |
| ------- | ---------- | ---------- | ---------- | ------------ | ----------------------------- | ----------------- |
| Wii     | C+Z        | `1 2 1 2`  | `1 1 2 2`  | `1 2 1 1`    | `2`, then D-Pad Left/Right x3 | `1 2 2 1 1 2 2 1` |
| Xbox/PC | LB+LT      | `Y X Y X`  | `Y Y X X`  | `Y X Y Y`    | `X`, then D-Pad Left/Right x3 | `Y X X Y Y X X Y` |
| PS3/PS4 | L1+L2      | `T S T S`  | `T T S S`  | `T S T T`    | `S`, then D-Pad Left/Right x3 | `T S S T T S S T` |
| Switch  | L+ZL       | `X Y X Y`  | `X X Y Y`  | `X Y X X`    | `Y`, then D-Pad Left/Right x3 | `X Y Y X X Y Y X` |

For dB2 DSi, simply press Select to use a Chroma Crystal. It even has actual UI!

# Future Ideas
I'm also thinking of making a manual apworld for the original [*Utrecht School of the Arts **student project*** version of "De Blob"](https://archive.org/details/TheBlob_201501) (note the capital D).  
I don't have much in the way of "receivable items", but I could probably squeeze a few checks out of it.  
<sup>Sidenote: As if the Switch ports of the de Blob games weren't bad enough already, those bastards capitalized the *de!!!*</sup>  
With actual game integration, there are a few things we could do that we can't do right now.  
If a "Restart Level" trap is received, we could set lives to 0 and kill Blob to force a game over (I personally find dB1's game over sound hilarious)  
Traps that *lower* the timer, and a *diabolical trap* that sets the timer to something ridiculously low like 30 seconds, hope you can find a timer pickup!!!

[^1]: I'm Canadian and we spell it "colour", but since we get the same versions of games as the US, *all* of the games have a blatant "typo" everywhere (sigh)
[^2]: You can find the Wii version of de Blob 1 second-hand at retro game stores and on sites like eBay.
[^3]: The Xbox 360 version, strangely enough, is backwards compatible with Xbox One and Series X/S consoles.  
If you can get Xbox Live sign-in to work on your 360, it'll still show up in your purchase history if you buy the BC version... for now at least.  
Source: I did this with the Banjo-Kazooie games so I could play them on a CRT
[^4]: I'm pretty sure the PS3 version of de Blob 2 is still available to purchase, but you'll need to add funds via the PSN website (or a PS4/PS5) and then visit the store on an actual PS3 to find it.
[^5]: THQ shut down the developer Helixe mid-production.  
There is a prototype ROM floating about, but it's too unstable for me to consider an apworld for it, and it would probably also get flagged for piracy in the official Archipelago discord.
[^6]: I do own the iOS version, and I know it was still listed as late as 2017, so maybe it'll still show up if you search for it on a device running iOS 10 or older?
[^7]: Same situation with dB1 mobile where I own the iOS version but not a device old enough to run it.
[^8]: The *Launch Glitch* depends on *your PC's hardware* ***and*** *which level you're playing.* For example, it happens in Rocket Range on my PC, but not in the same level on my Steam Deck.
