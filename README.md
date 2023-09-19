# My Over-Thought & Under-Done STONE STORY Script!

Three files that, together, comprise the automation script for my Stone Story gaming. I make no claims to how optimal or capable this script is, as I put it together without seeking help from the larger Stone Story community (what can I say, I like to figure things out for myself)! I've added comments and some configuration features, which I'll outline below.

## Assumptions Before We Begin
As this is an evolution of my script as I played through Stone Story, it presumes a fairly 'end game' build, with all of the Lost Treasures and a large collection of enchanted weapons and shields.  Some of this can be configured and toggled off, but you may need to poke around in the script and make some custom changes to perfectly fit your game (and inventory!)

In particular, the script assumes you have the following items in your inventory. If you are missing any (or just want to change what to use/craft), you'll have to skim the script to make the necessary changes (or just accept the occasional "no <X> to equip" error message).

- Bardiche ('big damage' and for cooldown ability)
- Heavy Hammer (used vs. armor)
- Blade of the Fallen God
- Cultist Mask
- Bashing Shield
- Dash Shield (no need to enchant or upgrade: just used for the dash)
- Quarterstaff (enchant with cooldown reduction)
- A Rune Hammer enchanted with extra health (required to take full advantage of defensive potions)

## Usage
1. Download all three files (`Main.txt`, `Utilities.txt` and `HUD.txt`)
2. Put all of them into the root of your Stone Story Scripts folder, right next to `Fishing.txt` (which is there by default)
3. Go through the `==== CONFIG ====` section (near the top of `Main.txt`) and set the values to match your game
3. Save, then import 'Main.txt' via your Mind Stone, like so:
```
import Main
```

## Gameplay
The following keyboard controls can be used to change the behavior of the script during a run:
- `[Z]` --- Enable/Disable the HUD
- `[S]` --- Enable/Disable using the Quarterstaff to accelerate through the level
- `[A]` --- Enable/Disable trying to pick off kills with the Skeleton Arm _(to satisfy the quest)_
- `[SHIFT]` --- HOLD to force-equip a (configurable) melee weapon, defaults to "bardiche"
- `[CTRL]` --- HOLD to force-equip a (configurable) ranged weapon, defaults to "repeating crossbow"
- `[X]` --- HOLD to force-equip your main shield _(useful when you want to increase your armor for as long as possible)_

## The HUD
The HUD has a lot of info, but you can toggle it off whenever you like with the `[Z]` key.  

![HUD Image](https://i.imgur.com/xSaufOs.png)

### HUD, Left Side
**Location: Name & Star Level**  
**Foe: Name (+total number of foes)**  
&nbsp;&nbsp;&nbsp;&nbsp;**\[...keywords\]**  
**Level = Distance, Damage, State:Time in State**  
**+** ...Buffs on **Enemy**  
**-** ...Debuffs on **Enemy**  
  
**+** ...Buffs on **Self**  
**-** ...Debuffs on **Self**  
*(Cooldowns)* **Sk = Skeleton Arm, BF = Blade of the Fallen God, Bh = Bashing Shield, M = Mindstone  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Q = Quarterstaff, Bd = Bardiche, H = Heavy Hammer**

### HUD, Right Side
*(Controls)* **\[Z\]** Activate/Deactivate HUD  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\[S\]** Activate/Deactivate Quarterstaff Jumping  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**\[A\]** Activate/Deactivate Skeleton Arm Kills (for artifact quest)  

**\<**Current Main Weapon, as determined by script**\>**  
**\[**Current Main Shield, as determined by script**\]**  
**\> **Current Main Ranged Weapon, as determined by script** \<**  

*(only present if active)*  
**Temporary Weapon/Shield Overrides** (will appear in pink)

**I: Current screen index    X: Current world position**  
*(AI States)* **\[AI\] \[Idle\] \[Paused\] \[Walk\]**
