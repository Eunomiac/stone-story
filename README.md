# My Over-Thought & Under-Done STONE STORY Script!

Three files that, together, comprise the automation script for my Stone Story gaming. I make no claims to how optimal or capable this script is, as I put it together without seeking help from the larger Stone Story community (what can I say, I like to figure things out for myself)! I've added comments and some configuration features, which I'll outline below.

## Assumptions Before We Begin
As this is an evolution of my script as I played through Stone Story, it presumes a fairly 'end game' build, with all of the Lost Treasures and a large collection of enchanted weapons and shields. I have included checks to avoid throwing errors should you be lacking an item that the script expects, but know that the script operates best when you have the following in your inventory:

- Bardiche ('big damage' and for cooldown ability)
- Heavy Hammer (used vs. armor)
- Blade of the Fallen God
- Cultist Mask
- Bashing Shield
- Fire Talisman
- Dash Shield (no need to enchant or upgrade: just used for the dash)
- Quarterstaff (enchant with cooldown reduction)

Please post an Issue if you see any errors (such as "`no <X> to equip"`).

## Usage (PC)
1. Download all three files (`Main.txt`, `Utilities.txt` and `HUD.txt`)
2. Put all of them into the root of your Stone Story Scripts folder, right next to `Fishing.txt` (which is there by default)
3. Go through the `==== CONFIG ====` section (at the top of `Main.txt`) and set the values to match your game
3. Save, then import 'Main.txt' via your Mind Stone, like so:
```
import Main
```

## Usage (Mobile)
If you're unable to download files, or import from multiple sources, I've consolidated my scripts into a single file that you can copy & paste directly into your Mind Stone.  Note that some functionality (including the HUD) is missing.
### Warning: This was prepared very very quickly and has yet to be tested by me, so I apologize in advance for any bugs. DM me on Discord if you'd like me to let you know when a more robust version of this file is available!
1. Copy and paste the entire contents of [this page](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Mobile/MainMobile.txt) into your Mind Stone
2. Go through the `=== CONFIG ===` section and set the values to match your game *(I have removed the explanatory comments to keep the wordcount low for mobile users; [click here](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-PC/Main.txt) to see the CONFIG section of the PC script, which contains all of the comments, or [click here](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Mobile/MainMobileGuide.txt) for a (hopefully) mobile-friendly text guide)*

## Gameplay (PC ONLY)
The following keyboard controls can be used to change the behavior of the script during a run:
- `[Z]` --- Enable/Disable the HUD
- `[S]` --- Enable/Disable using the Quarterstaff to accelerate through the level
- `[A]` --- Enable/Disable trying to pick off kills with the Skeleton Arm _(to satisfy the quest)_
- `[C]` --- Enable/Disable forced melee combat & dashing over ranged weapons _(for maximum speed)_
- `[SHIFT]` --- HOLD to force-equip a (configurable) melee weapon
- `[CTRL]` --- HOLD to force-equip a (configurable) ranged weapon
- `[X]` --- HOLD to force-equip a (configurable) shield or offhand weapon
- `[D]` --- Immediately trigger a dash by equipping Bash Shield or a Dash Shield
- `[W]` --- Immediately equip & activate Blade of the Fallen God
