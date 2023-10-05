# Learning StoneScript
The [Scripts-Annotated](https://github.com/Eunomiac/stone-story/tree/71a3a8ac396cbab9e1ecf6a541c8845ec9bb35f0/Scripts-Annotated) folder contains scripts that aren't part of my main scripts, but may be helpful to people just starting out or who want to learn StoneScript.  Every script in this folder is fully annotated with comments explaining almost every line, as well as comments offering more general suggestions and advice.  Most files contain a section at the end containing just the code, without my comments.

- [Attack Animation Cancelling](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Annotated/AttackAnimationCancelling-Annotated.txt) — A simple function you can run every frame to dramatically increase your attack speed by cancelling the animation of your weapon after it has dealt damage. This is a powerful scripting trick that everyone should use; check out [this video for a demonstration of its impact](https://youtu.be/BGKyCCMCUXY).
- [SimpleRockyPlateau](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Annotated/SimpleRockyPlateau-Annotated.txt) — A bare-bones script for farming the Rocky Plateau level _(requested by someone who was out of stones!)_. It includes Attack Animation Cancelling, as well as full combat logic for all three phases of the Dysangelos boss battle. It's fully annotated, and I've uploaded [a video showing it in action](https://youtu.be/EFTAjH8eCd0).
- [Romanize & xLookup](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Annotated/HelperFunction-CrossLookup-Annotated.txt) — Two helper functions you can drop right into your code and start using: A simple function to convert integers into Roman numbers, intended to set the stage for a much more versatile and useful function, `xLookup`, which you can use to "map" any value onto any other value.

# My Over-Thought & Under-Done STONE STORY Script!
Three files that, together, comprise the automation script for my Stone Story gaming. I make no claims to how optimal or capable this script is, as I put it together without seeking help from the larger Stone Story community (what can I say, I like to figure things out for myself)! I've added comments and some configuration features, which I'll outline below.

## Assumptions Before We Begin
As this is an evolution of my script as I played through Stone Story, it was initially coded for a fairly 'end game' build, with all of the Lost Treasures and a large collection of enchanted weapons and shields. I have since added checks and validation to (hopefully) ensure the script functions without presuming anything about the contents of your inventory, but know that the script operates best when you have the following:

- a Bardiche ('big damage' and for cooldown ability)
- a Heavy Hammer (used vs. armor)
- a Blade of the Fallen God
- a Cultist Mask
- a Bashing Shield
- a Fire Talisman
- a Dash Shield (no need to enchant or upgrade: just used for the dash)
- a Quarterstaff (enchant with cooldown reduction)

> [!WARNING]
> Be sure to break apart all unwanted zero-star items in your inventory before using this script, or the script may erroneously equip something it shouldn't!

Please post an Issue if you see any errors (such as "`no <X> to equip"`) while running the script. Be sure to include the full text of the in-game error message, including the line number and the file (i.e. `Main`, `HUD` or `Utilities`) if one is referenced.

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

> [!WARNING]
> This was prepared very very quickly and has yet to be tested by me, so I apologize in advance for any bugs. DM me on Discord if you'd like me to let you know when a more robust version of this file is available!

1. Copy and paste the entire contents of [this page](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Mobile/MainMobile.txt) into a text editor (not your Mind Stone, as the wonky line breaks in there will make configuring the script in the next step a real headache).
2. Go through the `=== CONFIG ===` section and set the values to match your game *(I have removed the explanatory comments to keep the wordcount low for mobile users; [click here](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-PC/Main.txt) to see the CONFIG section of the PC script, which contains all of the comments, or [click here](https://raw.githubusercontent.com/Eunomiac/stone-story/master/Scripts-Mobile/MainMobileGuide.txt) for a (hopefully) mobile-friendly text guide)*
3. Copy and paste the whole thing directly into your Mind Stone.  It will _look_ awful, with lines screaming off to the right in a brazen display of reckless disregard for page boundaries and common sense — but it should _work_ just fine.

## Gameplay (PC ONLY)
The following keyboard controls can be used to change the behavior of the script during a run:
- `[Z]` — Enable/Disable the HUD
- `[S]` — Enable/Disable using the Quarterstaff to accelerate through the level
- `[A]` — Enable/Disable trying to pick off kills with the Skeleton Arm _(to satisfy the quest)_
- `[C]` — Enable/Disable forced melee combat & dashing over ranged weapons _(for maximum speed)_
- `[X]` — HOLD to force-equip a (configurable) ranged weapon
- `[D]` — Immediately trigger a dash by equipping a Bashing or Dash Shield
- `[W]` — Immediately equip & activate Blade of the Fallen God
