# Big P's Mod Bonanza

## Install

These are my mods. Contents of mods folder should go in `common/PAYDAY 2/mods`, except for the contents of the directory `mod_overrides`. That content needs to be placed in your `PAYDAY 2/assets/mod_overrides` directory, then you can delete the `mod_overrides` directory in here.

## Configuration

Like 80% of the mods work just fine together and in fact some of them are able to detect the prescence of one another, which prevents crashes.

But there are some configuration options that should still be set to prevent primarily the HUD mods conflicting.

### VanillaHUD Plus

To avoid conflicts with Better Assault Indicator and VoidUI go to Mod Options > VanillaHUD Plus and change the settings to:

- VanillaHUD Plus > General Hud Panels Options > Select HUD Type Vanilla
- VanillaHUD Plus > General Hud Panels Options > Uncheck Enable Enhanced Objectives Panel
- VanillaHUD Plus > General Hud Panels Options > Uncheck Use Real Ammo
- VanillaHUD Plus > General Hud Panels Options > Chat Options > Uncheck Custom Chat
- VanillaHUD Plus > General Hud Panels Options > Suspicion Options > Uncheck Enable Suspicion Options
- VanillaHUD Plus > General Hud Panels Options > Assault Banner Options > Uncheck Center Assault
- VanillaHUD Plus > Tabstats Options > uncheck Use Tabstats
- VanillaHUD Plus > Interaction Options > check Custom HUDS Support and Uncheck Show Remaining Time
- VanillaHUD Plus > HUD Info Options > Set Right List Offset to 70
- VanillaHUD Plus > HUD Info Options > Set Left List Offset to 170
- VanillaHUD Plus >General Hud Panels Options > Other HUD Options > Uncheck Colored Joker Outlines

#### Better Assault Indicator Compatability

- Go to BAI -> HUDList -> Uncheck Move HUDList option

Finally, play around with the layout some. HUD Info Options is a good place to start. Off the bat, I recommend going to the "Right info panel" and moving it's Y position down so as to not be covered by the Void UI Assault panel.

### VoidUI

#### Jokers Keepers Mod Compatability

If you keep the Jokers Keepers Names mod, go to VoidUI Options and go to:

Labels & Waypoints > Enable Name Labels > Unchecked

This will remove VoidUI default name labels for converted cops, which would otherwise conflict with the custom Joker names.

#### Better Assault Indicator Compatability

### Extra Heist Info

Some of the timers may seem redundant with what VanillaHUD and VOID give you. After adjusting the settings for VanillaHUD above, enter a heist and test out what you have. I recommend a loud heist like Cook Off on normal mode or something, that will render many info boxes and timers.

### Joy's Score Counter + Hotline Miami Combo Counter

HM Counter has Joy's Counter as a dependency. So you get redundant information from these two by default. Remove one, remove both, keep both if you want. I keep just the Hotline Miami counter and set it's location to the bottom right above the Player Panel (my ammo, health etc)

### Pre-launch extras

There are two more things I recommend, AFTER you've installed all of the mods from this repo (or most), but BEFORE you next play the game. One is pretty much mandatory, two is up to you.

1. The "4GB patch" gives the Payday2 Windows executable more access to your machine's virtual memory. This is recommended all over the place in the PD2 mods community especially if you have a large amount of mod_override files. The executable found [https://ntcore.com/?page_id=371](at this page) will patch your PD2.exe or any other x86 executable you want to access more VRAM.
2. [Reshade](https://github.com/crosire/reshade) is a generic .exe that greatly improves lighting, ambient occlusion, etc for many games. There are lots of presets out there for Payday2. I'm using the [Scorbunny](https://modworkshop.net/mod/36474) preset. It's a little dark and I'm not crazy about it, but there are many others: https://www.nexusmods.com/payday2/mods/151, https://www.nexusmods.com/payday2/mods/198, etc

## The List

### Mods

Assume you need Beardlib and BLT installed in `mods` (NOT `mod_overrides`) for all of these to work.

- Adjusted Perk Descriptions

https://modworkshop.net/mod/35257

Perk deck descriptions from the game are fairly shitty, this improves them to better explain the benefits and drawbacks of each

- Anti Player State

https://modworkshop.net/mod/33580

Monitors and protects against state changes from the host. Basically an anti-crash/anti-grief mechanism

- Anti Stop the Cheater

https://modworkshop.net/mod/22560

Another anti-grief mechanism. Netiher of these are things that really have ever happened to me, so they might not really be necessary. I just figure why not hedge

- Anticrash

https://pd2mods.z77.fr/anticrash.html

3rd party (TdlQ is arguably the biggest modder in the pd2 scene, and the author of BLT) lua error handler. Extendable, for more complex error handling

- Ammo Break Invulnerability Effect

https://modworkshop.net/mod/33030

Renders a color overlay over the HUD when Anarchist's invulnerability effect kicks in. You don't need it if you don't use the Anarchist perk deck

- Auto-Discard parachute

https://pdmods-arc.berigora.net/paydaymods.com/mods/patchnotes/279/1/index.html

Birth of Sky heist has a parachute carryable that is easy to forget. It's a loud heist and you have to bag money at one point under fire. Protects against stoner brain reflex to forget.

- BeardLib

https://modworkshop.net/mod/14924

Dependency for virtually every mod

- Better Assault Indicator

https://modworkshop.net/mod/22712

Much better Assault wave indicator. Colorized for each part of the assault (control, assault, etc), customizable.

- Better Bots

https://modworkshop.net/mod/12736

Your AI teammates suck out of the box. This makes them good. Makes solo play at high difficulties in loud heists much more managable.

- Borderless Windowed Updated

https://modworkshop.net/mod/27683

Must have for dual monitors. Gives the game a "Fullscreen Windowed" option in Options > Display > Display Mode

- base

This is from SuperBLT. You should probably install SuperBLT manually (and beardlib) and not just paste it into `mods` from this repo, like you can with all the other mods. But honestly, that might not even matter.

- BuildDB

https://pd2mods.z77.fr/buildb.html

Adds the ability to save a custom build config file and import those builds to your skills tree on-demand.

- Carry Stacker Reloaded

https://github.com/enragedpixel/Carry-Stacker-Reloaded

Carry more than one bag at once, with a weight penalty (or not ;) ).

- ColorPicker

https://modworkshop.net/mod/29641

Dependency for several of these mods that let you choose custom colors. It's similar to MacOS or Windows color pickers

- CustomFOV

https://modworkshop.net/mod/20801

Turn FOV up to eleven

- Drag and Drop Inventory

https://pd2mods.z77.fr/drag_and_drop_inventory.html

It's great

- Extra Heist Info

https://modworkshop.net/mod/31915

Shows trackers in your HUD for remaining time, interactions, achievement progress, etc. Helpful but will overlap with VanillaHUD and Void UI out of the box. See "Setup" section above

- Extra Profiles & Skill Sets

https://modworkshop.net/mod/26702

More is always better!

- GoonMod's Custom Waypoints

https://pd2mods.z77.fr/goonmod_custom_waypoints.html

Lets you mark your own waypoints. Dependency for one of the bot improvement mods found here, also

- Hotline Miami Combo Counter

  https://modworkshop.net/mod/30999

  Animated score and kill counter

* Immersive Dodge Sounds

  https://modworkshop.net/mod/35278

  Makes a much better wooooosh noise when the dodge effect in your build kicks in and a bullet goes flying by. Woosh

* Intro Cinematics

  https://modworkshop.net/mod/27164

  Plays awesome cutscene-type angles of the heist map as the game loads in, replacing the loading screen. Not necessary but cool

- Iter

  https://pd2mods.z77.fr/iter.html

  Fixe the garbage NPC pathing in this game

- Joy's Score Counter

  https://modworkshop.net/mod/24730

  Dependency for Hotline Miami Combo Counter. I generally hide this one and just display the Hotline Miami counter. You can use either one, or neither if you don't want care about tracking kills and score functionality. Or both I guess if you wanted to. In stealth, kill and score counts don't matter, so make of that what you will.

- Keepers

  https://pd2mods.z77.fr/keepers.html

  Issue orders to AI/friendly NPCs. Plays really nicely with Better Bots. In the game options > mod keybinds, you can set hotkeys to make your AI team hold and follow.

- Less Inaccurate Weapon Laser

  https://pd2mods.z77.fr/less_inaccurate_weapon_laser.html

  Guess what this does?

- Map-based Optimizations

  https://modworkshop.net/mod/30521

  Perf improvements for most of the heists in the game

- Menu Backgrounds

  https://modworkshop.net/mod/17160

  Custom menu backgrounds. Comes with a few out of the gate, but ModWorkshop has a ton of options too. In this repo, all of the backgrounds I already downloaded can already be found in `Menu Backgrounds/Assets`. To set different backgrounds go to Mods > Mod Options > Menu Backgrounds.

- Meth Helper Updated

  https://modworkshop.net/mod/25950

  Automatically spits the next meth ingredient out into the chat, as a message from you (e.g. THE CJ CAR: Add Caustic Soda)

- More Paint Schemes

  https://modworkshop.net/mod/36509

  Adds a bunch more paint schemes in weapon mods. Schemes are the manner in which a skin is applied e.g. "Tactical", "Broken in", "Mint condition" etc

- No Concussion Tinnitus

  https://modworkshop.net/mod/22127

  Removes tinnitus effect (ear "ringing") effect when you get hit with a flashbang

- No Duplicated Bullets

  https://pd2mods.z77.fr/no_duplicated_bullets.html
  Fixes some desync issues when playing as a client online

- No prints

  https://modworkshop.net/mod/21549

  Purely performance related improvement - disables a bunch of debug invocations that the game devs put in all over the place (lol)

- No Screen Shake

  https://modworkshop.net/mod/22471

  Shoutout to Rocket League

- Advanced Crosshairs, Hitmarkers + Hitsounds ("ACH")

  https://modworkshop.net/mod/29585

  Better crosshair and audio/visual feedback when capping a MFer

- PD2-hoplib-master

  This is a dependency for something. Not sure what.

- Keepers Jokers Names

  https://modworkshop.net/mod/21416

  Gives converted police a unique human name like "Greg", lol

- PECM Bug Fix

  https://modworkshop.net/mod/32373

  Fixes a bug where pocket ECM can crash your game. It's never happened to me before, but I installed this just in case, because I use Hacker consistently in Stealth. If you don't use Hacker at all this is worthless

- QuickKeyboardInput

  https://pd2mods.z77.fr/quick_keyboard_input.html

  Dependency for BuilDB

- Search Inventory

  https://pd2mods.z77.fr/search_inventory.html

  Query inventory view with string input

- Sensitivity Fixer

  https://modworkshop.net/mod/12823

  Changes game options mouse sensitivity to 0 - 1 range rather than 0.7 - 1.7

- Silent Assassin

  https://pdmods-arc.berigora.net/paydaymods.com/mods/304/silentassassin.html

  huehuehuehuehue

- Simple Mod Updater

  BLT dependency. auto-installs with BLT

- The Fixes

  https://modworkshop.net/mod/23732

  Must-have fixes some bugs that exist in the game out of the box

- VanillaHUD Plus

  https://modworkshop.net/mod/25629

  This is the latest stable iteration of what was formerly called WolfHUD. Best HUD mod available to display in-game info.

- VoidUI

  https://modworkshop.net/mod/20997

  Greatly enhances readability and pretty-ness of menu and UI elements of the game. I love this one but it is a little opinionated. It can be replaced by HoloUI, among others, if you don't like it. HoloUI, similar to Void, has autodetection of other HUD mods built in. Check VanillaHUD's official mod page for compatability settings with HoloUI and other UI mods.

- VoidUI Hotline Miami Vibe

  https://modworkshop.net/mod/36209

  Beautiful color scheme for VoidUI

- Yet Another Flashlight

  https://pd2mods.z77.fr/yet_another_flashlight.html

  Greatly improves the in-game flashlight quality. Makes seeing in the dark much nicer

### Mod Overrides

- HOXTON BREAKOUT - Thomas
  Turns the truck into Thomas the Tank Engine
- Deskinned... mods, Luxurious Weapon Colors
  Beautiful skins for your weapons
- 00 FEDNET Icons + Fednet player styles
  Improved visual icons and player styles for the menus
- Alternative Cocaine Bags
  Nicer stacks of coke before bagging
- Belle Daphine body bag case
  I just like the purple color it makes the body bag case lol
- Beneath the mountain keycard
  Custom murkywater keycard replaces gen sec keycard
- Better Camera Beeps
  Makes the security cam beeps MUCH less annoying
- Boiling Point - Russian keycard
  Russian keycard replaces gensec in boiling point
- Capitol Meme Gallery
  Replaces art in the art gallery hesits with memes
- Clean Drill Screen
  Gives the drill screen a flat black background, easier to read due to the higher contrast
- Default - Gensec keycard
  Improved keycard
- Enhanced Glass Cutting
  Makes the glass cutting noise for several stealth heists MUCH less annoying
- Even More Visible Power Box
  Replaces default power box textures with a much more visible black, makes them easier to find in White House, Diamond Heist, etc
- Golden Grin Keycard
  Keycard texture replacements for Golden Grin Casino, replaces gensec keycards
- Hank Hill - Dallas
  Makes Jacket say "Dallas" like Hank Hill from King of the Hill
- High Quality Ammo Bags
  improved ammo bag texture
- Highlighter
  Adds contour / highlight lines for a TON of stuff: cameras, planks, gage packs, keycards, gas cans, and more. Huge time saver
- IceTech$Support... mods
  Improved visual quality for loose loot items + money
- Improved SWAT Van
  Makes SWAT van less stupid looking and boring
- Joy High socks and shorts
  ( ͡° ͜ʖ ͡°)
- KingPin Injector Indicator
  You don't need it if you don't use the Kingpin perk deck
- LC_MacroPack_Smoke
  Makes smoke look better in game
- Looking for Tracy Tzu
  Replaces "Drifting" original game song. This is the custom track I use in Preplanning
- Master Indigos... mods
  Improve visual quality of First Aid Kits, grenade case, doctor bag, and in-store items in heists
- Miami Heat Jacket
  Custom outfit scheme for Jacket. Basically you should install this so that _my_ character looks awesome when we play
- Mute Joy Score
  Joy shouts out annoying things like "Taser Down, 7 points!" this mutes that
- Mute Dentist in Pre-planning
  "Let's put this boat in the water..." Let's not. Shut up, Gus Fring
- Nepgearsy weapon case
  Improves visual quality of assault weapons loot case
- Payday Two Intro
  Replaces game launch intro with one from Yakuza game. Don't need it if you don't play the Yakuza games.
- Pink Cursor =)
  What can I say, man?
- Running in the 80s
  Great custom track. Makes a nice replacement for the game's title music at the menus, which is how I use it.
- Sirens in the Air Tonight
  Replaces in-game song "Sirens in the distance" with Phil Collins In the Air Tonight
- Sweet tooth
  Makes the getaway van have a polka dot and ice cream scheme like sweet tooth from twistedd metal's ice cream truck
- TexGyre
  Replaces the default game typeface with a custom one that looks 1 million times better IMO
- Two-tone camera
  Non-TITAN cameras look nicer
- Unique Loot
  Changes lootbags from being the same navy blue to different depending on contents. Each has a logo. Borderline must-have IMO
- Uzi's N Carnations Shirt for Sangres
  Gives Sangres an awesome shirt that I wish I had IRL
- Vengance Custom Track
  Awesome song for loud hesits
- Weapon Texture Reworks
  Makes weapons look better
- Wish Bodybag
  Gives bodybags the WISH.com color and logo
- Yakuza 0 Logo
  To go with my Yakuza intro video mod. Not necessary if you don't play yakuza
