## [v4.0: Check Butter - Spread it evenly!](https://github.com/Iristallite/deBlob_manual_apworlds/releases/tag/release-v4.0)
Published: 2026-03-29 @ 23:10 UTC  
An issue I've felt these manuals have is that most checks get sent near the end of the levels.  
I have implemented many new check options for the console/PC games, and touched up the DS game a little bit.  
Shoutouts to the Metal Gear Rising and Sonic CD OSTs for carrying me through the final stretches of working on this massive update.

* DEV: Rebased to latest stable ManualAP release [20260319](https://github.com/ManualForArchipelago/Manual/releases/tag/manual_stable_20260319)
* DEV: Reformatted internal json files with my "semi-minified + heavily-aligned" style to MASSIVELY improve readability and maintainability
* Readme: Disfigured the DS box art to fit in the preview image
* Readme: Glazed the PS3 version of de Blob 2 and insulted every 2018 port
* ALL: `.apworld` files are now compressed, reducing sizes from ~350kb to ~75kb
* ALL: Moved DeathLink option to the top of the yaml next to prog balancing and accessibility
* ALL: Added a time-wasting option to shuffle the SKIP BUTTON as an item because it's funny
* ALL: Used `sort_key` feature to sort check lists by hand
* ALL-ish: Added new preset yamls:
* `Zip's Choice`: A quick and breezy preset that excludes many "hundo" checks, ideal for beginners
* `Arty's Masterpiece`: My ideal default settings
* `Prof's Classic`: Rough equivalent to v3 and earlier behaviour
* `Bif's Fullsanity`: ALL THE CHECKS!
* `Comrade Black's Little Black Book`: Beware...
* dB1+dB2: Added a completely cosmetic yaml option to signify what version you're playing on
* dB1+dB2: Added options to restrict *optional* Power-Up usage with collectible items
* DS: Renamed "Musical Collector" to "Musician"
* DS: Renamed "Rocket Parts" McGuffin to "Launch Access Codes" to distinguish it from the console game's McGuffin
* DSi: Removed `dsi_enhanced` yaml setting in favour of more granular options
* DSi: The Chroma Crystal can now be shuffled as shards or a permanent upgrade, rather than just as a consumable cheat
* dB1: Massive refactor
* dB1: Renamed "Level Complete" to "Level Complete (Bronze Medal)"
* dB1: Renamed "Street Artist" to "Billboard Artist"
* dB1: Renamed "Blimp Painted" to "Pilot"
* dB1: Re-arranged check categories
* dB2: Renamed "Railyards Liberated" to "Mutant Inky Defeated (Railyards Liberated)"
* dB2: Still didn't add Blob Party
* dB2: Became even more baffled by how badly the Switch port got screwed up
Added the following checks as toggleable options:
* dB1: Gold Medals for story levels
* dB1: 100% Painted
* dB1: All pre-existing awards
* dB1: Silver Medals for story levels
* dB1: Silver/Gold medals for bonus missions
* dB1: 25%, 50%, 75% Painted
* dB1: Clearing levels in Free Paint Mode
* dB1: 20 unique checks for doing specific things in each Bonus Mission (and one for Free Paint)
* dB1: Sector Gates (gatesanity)
* DS: Musician, Liberator, and Chroma Camera
* dB2: Most prior things (S Rank, Gold Medals Collector awards)
* dB2: Bronze and Silver medals for Liberation, Environment, and Clean-Up
* dB2: Transform Engines, with Heavy or Light modes (transformsanity, this took a lot of work)

## [v3.1: $25 Apple Polishing Cloth](https://github.com/Iristallite/deBlob_manual_apworlds/releases/tag/release-v3.1)
Published: 2026-01-09 @ 23:57 UTC

A little bit of polish goes a long way.  
<sup>yes, apple actually sells a [$25 cloth...](https://apple.com/ca/shop/product/mw693am/a/polishing-cloth)</sup>

* Changed the game names in the apworlds to look slightly nicer. This **will** break existing yamls.
* Shrank header sizes in changelog and readme to look slightly nicer
* Removed compiled apworlds from the base repository so git doesn't try to delta-patch them and waste ~0.7MB each time
* Linked v3.0 in the readme because I apparently forgot to
* Removed `www.` from readme links to save an inconsequential amount of space that was immediately used again several dozen times over by this unnecessarily long changelog note
## [V3: The Great Options update!](https://github.com/Iristallite/deBlob_manual_apworlds/releases/tag/Release-V3.0)
Published: 2025-12-01 @ 11:00 UTC

And now for something... more customizable!   
* Added many yaml options
  * Trap toggles
  * Cheat toggles
  * Pinky toggle
  * Shuffled/Progressive level modes
  * Option to remove the worst level in dB1 (10-2: Sinking Feeling)
* Renamed `Comrade Black's Plans` to `Comrade Black's Blueprints` for arbitrary reasons
* Renamed `+10 Minutes` to `Time Bonus`
* Removed the `INKT Informed` check since the trophy pops after beating the goal level
* Combined the DS and DSi versions of de Blob 2 into a single apworld with a DSi Enhanced™ toggle
* Actually fixed DeathLink being broken on the dB2 apworld <sup>(The V2 hotfix was identical to V2...)</sup>
* Fixed a few typos in the readme
* Tidied up my office

Shoutouts to [BigBradley](https://github.com/BigBradley)'s [Mario Kart 7 manual](https://github.com/BigBradley/Mario-Kart-7-Manual-APworld), which I referenced to set up the new yaml options!  

As always, the dB2 PC Audio Patch is included. Steam tested, GOG support not guaranteed.  
**I tested this by running 100 generations of 10 mixed-settings worlds, and got no gen failures!**  
**If anything breaks with the apworld, please either open an issue or send me a message on discord (iristallite)** 
<sup>Blob Party mode for *de Blob 2* coming eventually.</sup>

## [V2: The first public release](https://github.com/Iristallite/deBlob_manual_apworlds/releases/tag/release-V2)
## [V2: The first public release](https://github.com/Iristallite/deBlob_manual_apworlds/releases/tag/release-V2)
Published: 2025-08-16 @ 00:34 UTC

After several days of work, a test-run in a short async with some friends, more work, a brief hiatus due to a heatwave, and a bit more work, the de Blob series apworlds have been released!

Please enjoy.  
Contains apworlds for:

* de Blob 1 (Console/PC)
* de Blob 2 (DS)
* de Blob 2 (DSi)
* de Blob 2 (Console/PC)  
Also includes a patch for the Steam version that fixes a nasty audio bug where Blob's "pain" sound will keep looping indefinitely.  
To apply, drag the `Data` folder from `deBlob2_Steam_AudioPatch.zip` directly into the `de Blob 2` game folder in `steamapps/common` and overwrite, wherever that is on your device.
<sup>The patch might work on the GOG version, but I only own the Steam version so I can't test.</sup>  
<sup>I am also aware that this is technically distributing game files, but all these files do is tell the game where and which sound effects to play, and as such I believe that no copyrighted assets are contained within.</sup>  
**If anything breaks with these, please either open an issue or send me a message on discord (iristallite)**  
<sup>hotfix 2025-08-19: add missing deathlink support to dB2 PC</sup>  
<sup>Hilariously, despite the new zip having `hotfix` in the name... I forgot to add the hotfixed apworld. OOPS</sup>