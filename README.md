# My Over-Thought & Under-Done STONE STORY Script!

Three files that, together, comprise the automation script for my Stone Story gaming. I make no claims to how optimal or capable this script is, as I put it together without seeking help from the larger Stone Story community (what can I say, I like to figure things out for myself)! I've added comments and some configuration features, which I'll outline below.

## Assumptions Before We Begin
As this is an evolution of my script as I played through Stone Story, it presumes a fairly 'end game' build, with all of the Lost Treasures and a large collection of enchanted weapons and shields.  Some of this can be configured and toggled off, but you may need to poke around in the script and make some custom changes to perfectly fit your game (and inventory!)

In particular, the script assumes you have the following items in your inventory. If you are missing any (or just want to change what to use/craft), you'll have to skim the script to make the necessary changes (or just accept the occasional "no \<X\> to equip" error message).

- Bardiche ('big damage' and for cooldown ability)
- Heavy Hammer (used vs. armor)
- Blade of the Fallen God
- Cultist Mask
- Bashing Shield
- Fire Talisman
- Dash Shield (no need to enchant or upgrade: just used for the dash)
- Quarterstaff (enchant with cooldown reduction)

## Usage
1. Download all three files (`Main.txt`, `Utilities.txt` and `HUD.txt`)
2. Put all of them into the root of your Stone Story Scripts folder, right next to `Fishing.txt` (which is there by default)
3. Go through the `==== CONFIG ====` section (at the top of `Main.txt`) and set the values to match your game
3. Save, then import 'Main.txt' via your Mind Stone, like so:
```
import Main
```

## Gameplay
The following keyboard controls can be used to change the behavior of the script during a run:
- `[Z]` --- Enable/Disable the HUD
- `[S]` --- Enable/Disable using the Quarterstaff to accelerate through the level
- `[A]` --- Enable/Disable trying to pick off kills with the Skeleton Arm _(to satisfy the quest)_
- `[C]` --- Enable/Disable forced melee combat & dashing over ranged weapons _(for maximum speed)_
- `[SHIFT]` --- HOLD to force-equip a (configurable) melee weapon
- `[CTRL]` --- HOLD to force-equip a (configurable) ranged weapon
- `[X]` --- HOLD to force-equip a (configurable) shield or offhand weapon

## The HUD
The HUD has a lot of info, but you can toggle it off whenever you like with the `[Z]` key.  

![HUD Image](https://i.imgur.com/xSaufOs.png)
