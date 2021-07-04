<!---
Shields.io Github badges!
-->

![GitHub release (latest by date)](https://img.shields.io/github/v/release/4Luke4/PnP-Potions?color=yellow&style=flat)
![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/4Luke4/PnP-Potions?color=yellow&style=flat)
![Platform](https://img.shields.io/static/v1?label=platform&message=windows%20%7C%20macOS%20%7C%20linux%20%7C%20Project%20Infinity&color=informational&style=flat)
![Language](https://img.shields.io/static/v1?label=language&message=English%20%7C%20Italian%20%7C%20French%20%7C%20German%20%7C%20Spanish%20%7C%20Simplified%20Chinese%20%7C%20Russian%20%7C%20Polish%20%7C%20Portuguese%20%7C%20Japanese%20%7C%20Hungarian%20%7C%20Czech&color=teal&style=flat)
![Supported games](https://img.shields.io/static/v1?label=supported%20games&message=BG%3AEE%20%7C%20BG2%3AEE%20%7C%20IWD%3AEE%20%7C%20EET&color=dodgerblue&style=flat)

![GitHub repo size](https://img.shields.io/github/repo-size/4Luke4/Pnp-Potions?style=flat)
![GitHub all releases](https://img.shields.io/github/downloads/4Luke4/PnP-Potions/total?color=cyan&style=flat)
![GitHub release (latest by date)](https://img.shields.io/github/downloads/4Luke4/PnP-Potions/latest/total?color=cyan&style=flat)
![Maintenance](https://img.shields.io/static/v1?label=maintained%3F&message=yes&color=greenlight&style=flat)
![GitHub contributors](https://img.shields.io/github/contributors/4Luke4/PnP-Potions?color=blueviolet&style=flat) [![Contributors Display](https://badges.pufler.dev/contributors/4Luke4/PnP-Potions?size=30&padding=5&bots=true)](https://badges.pufler.dev)

![GitHub issues](https://img.shields.io/github/issues/4Luke4/PnP-Potions?color=red&style=flat)
![GitHub pull requests](https://img.shields.io/github/issues-pr/4Luke4/PnP-Potions?color=brown&style=flat)

##

<div align="center"><h1></a>PnP Potions</h1></div>

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