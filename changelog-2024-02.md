---
title: Changelog - February 2024
description: Changelog entries for February 2024
published: true
date: 2025-06-19T23:05:12.759Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:05:12.759Z
---

# Changelog - February 2024

[← Back to Recent Updates](/en/Change-log-history) | [March 2024 →](/en/changelog-2024-03)

---

*13 updates in February 2024*

<a name="entry-1212901460459659356"></a>

## 2024-02-29 23:17 - Entry 1212901460459659356
**Author:** Catapultam

```
- Tradeskills will always return (Awakened) items.
` Removed (Latent) tag from normal-quality gear. Henceforth 'untagged' tier.
- Renamed (Potent) tag to (Latent)
```

---

---

<a name="entry-1212887837637091349"></a>

## 2024-02-29 22:23 - Entry 1212887837637091349
**Author:** Catapultam

```
- Added MIT and AVG stats to inventory; These show ACTUAL mitigation and avoidance AC after softcap are taken into account
```

---

---

<a name="entry-1212880650231750686"></a>

## 2024-02-29 21:54 - Entry 1212880650231750686
**Author:** Catapultam

```
- Improved merchant filtering (patch needed)
- All activated are now instant-cast (patch + reboot)
- Augments no longer require distillers to remove (reboot)
```

---

---

<a name="entry-1212842973805420665"></a>

## 2024-02-29 19:24 - Entry 1212842973805420665
**Author:** Catapultam

```
- Soulbinders will also offer gates to bazaar and bind
```

---

---

<a name="entry-1212822578775855125"></a>

## 2024-02-29 18:03 - Entry 1212822578775855125
**Author:** Catapultam

```
- reverted 'humans look like monk thing' for now
- restored original UI
- custom UI can be loaded with /loadskin thj_ui
```

---

---

<a name="entry-1212579951899836436"></a>

## 2024-02-29 01:59 - Entry 1212579951899836436
**Author:** Catapultam

```
- Switching base class should no longer be required for any class combinations
- Please report any problems with spellcasting as high-priority bugs
- Humans and Iksar with Monk in their composition will look like Monks
```

---

---

<a name="entry-1212500743593001070"></a>

## 2024-02-28 20:45 - Entry 1212500743593001070
**Author:** Catapultam

```
(Patch Required)
- Merchantlist filter now properly accounts for your classes
- Levels displayed on spell scrolls is no longer wonky for shared spells
```

---

---

<a name="entry-1212457069127401575"></a>

## 2024-02-28 17:51 - Entry 1212457069127401575
**Author:** Catapultam

* Pending Reboot
```
- Added
RULE_INT(Spells, DOTsScaleWithSpellDmgPerTickPercent, 0, "Allow SpellDmg stat to affect DoT spells but by a per tick")
RULE_INT(Spells, HOTsScaleWithHealAmtPerTickPercent, 0, "Allow HealAmt stat to affect HoT spells but by a per tick")
RULE_INT(Spells, PetsScaleWithOwnerPercent, 0, "Allow Pet spells to use the owners stats when casting spells by a percent")
```

---

---

<a name="entry-1212296544359817266"></a>

## 2024-02-28 07:13 - Entry 1212296544359817266
**Author:** Catapultam

```
- Fixed Lavastorm (repatch needed)
- Fixed Patcher weirdness
- Abysmal Sea is accessible
- Added LoY, DoN, OoW, GoD zones to progression lockouts
- Any tag (Latent, Potent, or Awakened) can be used for quest turn-ins
- All AA are instant-cast.
- Fading Memories now uses mana
- Added Phinigel Autropos to Kunark unlock targets
- Attempting to zone to a disallowed zone will drop you in the nexus.
- Fixed Several bugs
- Fixed Neriak waypoint in the wrong location. Cleared all waypoints.
- Fixed pet buffs suspension after zoning
- Fixed detrimental spells suspending
```

---

---

<a name="entry-1211944847376777226"></a>

## 2024-02-27 07:56 - Entry 1211944847376777226
**Author:** Catapultam

```
- Disciplines should now no longer cause crash on zone
- Implied targeting should be much improved (corpses, procs)
- Pet buffs & heals no longer force change target to pet
```

---

---

<a name="entry-1211454275004141629"></a>

## 2024-02-25 23:26 - Entry 1211454275004141629
**Author:** Catapultam

```
- Re-enabled corpses
- Disabled quests from checking corpses for items (lag fix)
- You can now zone out of the Bazaar using a means other than the zone line
   - Expected behavior here is that zone lines take you to the source of your portal. If you don't have one somehow, you'll go to the nexus if you have luclin unlocked or your bind point otherwise.
   - Leaving the zone by any means other than a zone line will clear your saved portal source location
- Corrected zoning into Highpass (New version for now, will work on legacy version again later)
- Implemented Faded Writ quest
- Removed all Fabled mobs from spawn lists
```

---

---

<a name="entry-1210879145433628741"></a>

## 2024-02-24 09:21 - Entry 1210879145433628741
**Author:** Catapultam

```
- Disabled corpses for now to work around a crash bug
```

---

---

<a name="entry-1210783101270102156"></a>

## 2024-02-24 02:59 - Entry 1210783101270102156
**Author:** Catapultam

```
- Hello!
- Fixed the No-XP bug
- Fixed base mana regen
- Fixed crash on interacting with GM
```

---

---

