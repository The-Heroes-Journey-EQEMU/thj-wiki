---
title: Changelog - April 2024
description: Changelog entries for April 2024
published: true
date: 2025-06-19T23:05:04.895Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:05:04.895Z
---

# Changelog - April 2024

[← Back to Recent Updates](/en/Change-log-history) | [← March 2024](/en/changelog-2024-03) | [May 2024 →](/en/changelog-2024-05)

---

*6 updates in April 2024*

<a name="entry-1234957730041823334"></a>

## 2024-04-30 20:01 - Entry 1234957730041823334
**Author:** Catapultam

Deploying beta branch for testing. Have fun. Partial changelog below.

```
* Renamed Latent to 'Enchanted'
* Renamed Awakened to 'Legendary'
* Implemented Dynamic Items;
  - Framework for creating persistent runtime-created items. The ID of these items is not predictable, as they are assigned JIT.
  - Notable limitations:
    - Dynamic Items may not be sold to NPC vendors (forced to 0-value)
    - Dynamic Items may not be traded to NPCs
    - Dynamic Items may not dropped on the ground
* Implemented Artifacts;
  - Artifacts have a chance to be generated when a player recieves a Legendary item through Loot, Tradeskill, or Quests
  - Artifacts are Dynamic Items.
  - Artifacts are named after the player who found them, and can be discovered once per Season (Non-Season is Season 0)
* Implemented 'Leveling' items in Power Source slot
  - Items placed in Power Source slot block player from gaining XP normally
  - They accumulate XP until they reach a sufficient amount based on their stats, and then upgrade to the next tier (ie Normal->Tier1->Tier2)
```

---

---

<a name="entry-1234282565913804800"></a>

## 2024-04-28 23:18 - Entry 1234282565913804800
**Author:** Retribution EQ #change-log

```
Bazaar NPC overhaul.

Bazaar NPCs have been moved to give the Bazaar a more natural feel.

Check the back stalls for GMs, Spell Vendors, and Tomes.
```

---

---

<a name="entry-1232891641598050344"></a>

## 2024-04-25 03:11 - Entry 1232891641598050344
**Author:** Retribution EQ #change-log

```
- AoR for Yxxta has been moved.
- Enchanter pets over level 55 have had their damage increased.
- Necromancer AA Death Bloom is now available at 51... be careful.
- Classic Rogue poisons *actually* have 50 charges now.
- Rathe Council banishes now instance aware.
- Backstab Damage has been completely removed from weapons. This means that backstab will now use weapon damage as backstab damage. (This is a BUFF to backstab damage).
- Monks starting AA changed from Stonewall to Rk I of Techniques of Master Wu
- All pet classes now start with Pet Discipline
- Tendrils of Fire now hits for 450 and has a -450 resist mod
- Vrabbit Xloren is now instance aware when he ports you
- Ranger AA Trickshot Rk I now starts at 5% up from 2% and continues to increase by 2% per rank
- ALL RC and Apoc weapons now have the correct +10% and +20% proc mods they were meant to
- There is now only one Vacto
```

---

---

<a name="entry-1232318545015345263"></a>

## 2024-04-23 13:13 - Entry 1232318545015345263
**Author:** Retribution EQ #change-log

```
Bugfixes:
- Fixed Saryrn and Quarm (GoD and Fabled Naggy) flags
- Ancient Cragbeast Matriarch in Txevu no longer causes client disconnects
- Several misc bugfixes
- Muzzle of Mardu is no longer usable by players

New Features:
- Bazaar Portal will now return you to the place where you last used it if you use it while inside the Bazaar
- Items may now be Parceled
- Apocrypha in the Bazaar now offers an option to enhance the upgrade rate of all drops in the world for 4 hours. While in effect, this buff will cause any mob you kill to have an additional chance to upgrade each of its drops from normal to Rose Colored or from Rose Colored to Apocryphal. (This is a world-wide buff which affects all players while it is in effect).
```

---

---

<a name="entry-1232223984561553438"></a>

## 2024-04-23 06:58 - Entry 1232223984561553438
**Author:** Catapultam

PENDING REBOOT

```
Bugfixes:
- Fixed Saryrn and Quarm (GoD and Fabled Naggy) flags
- Ancient Cragbeast Matriarch in Txevu no longer causes client disconnects
- Several misc bugfixes
- Pet bag no longer endlessly upgrades items
- AA are instant-cast again
- All versions of Intricate Wooden Figurine which you are eligible will be awarded.

New Features:
- Bazaar Portal will now return you to the place where you last used it if you use it while inside the Bazaar
- Items may now be Parceled
- Apocrypha in the Bazaar now offers an option to enhance the upgrade rate of all drops in the world for 4 hours. While in effect, this buff will cause any mob you kill to have an additional chance to upgrade each of its drops from normal to Rose Colored or from Rose Colored to Apocryphal.
```

---

---

<a name="entry-1229610384810577930"></a>

## 2024-04-16 01:52 - Entry 1229610384810577930
**Author:** Catapultam

```
- THJ is now officially running entirely off of Retribution's database.
- More iteration to come in terms of scripts and content!
```

---

---

