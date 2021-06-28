# PnP Potions
**Author**: Luke

**Discussion:** [Beamdog Forums](https://forums.beamdog.com/discussion/82300/)

## Overview
*This mod is meant to implement PnP potion behavior.*
## Contents
After installing this mod, all in-game potions will behave as follows.
Quaffing a potion while the effects of any potion were still active might trigger one of the following events:
- **1%** chance to explode.
	- `5d10` fire damage on the drinker, `+ 1d10` fire damage in `5'` radius (small fireball) (total of `6d10` on the drinker).
- **2%** chance for instant poison death.
	- Unless the drinker is completely immune to poison damage.
- **5%** chance for Strength & Dexterity loss.
	- It will cause `1` Strength and `1` Dexterity loss.
	- This result will also cause sleep (nausea) for `1` round.
- **7%** chance to cancel/remove all active potion effects.
- **10%** chance the current potion does nothing.
- **10%** chance the current potion has half effectiveness.
	- For instance, *Potion of Magic Blocking* would last for `15` seconds (instead of `30`).
	- For instance, *Elixir of Health* would heal the drinker for `5` Hit Points (instead of `10`).
- **8%** chance the current potion has `+50%` effectiveness.
	- For instance, *Potion of Magic Blocking* would last for `45` seconds (instead of `30`).
	- For instance, *Elixir of Health* would heal the drinker for `15` Hit Points (instead of `10`).
- **1%** chance the current potion has permanent/double effectiveness.
	- For instance, *Potion of Magic Blocking* would last indefinitely (until dispelled).
	- For instance, *Elixir of Health* would heal the drinker for `20` Hit Points (instead of `10`).

Permanent potions, such as potions of healing, would be considered still in effect for `1` turn (`60` seconds) after drinking them.

The aforementioned special events can occur only upon quaffing **potions**.
As a result, there is no risk in using 1 Oil and 1 Potion, as oils are applied to the skin, not consumed, so they wouldn't mix.