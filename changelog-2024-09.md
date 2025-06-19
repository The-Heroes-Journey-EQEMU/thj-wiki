---
title: Changelog - September 2024
description: Changelog entries for September 2024
published: true
date: 2025-06-19T23:04:43.462Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:43.462Z
---

# Changelog - September 2024

[← Back to Recent Updates](/en/Change-log-history) | [← August 2024](/en/changelog-2024-08) | [October 2024 →](/en/changelog-2024-10)

---

*24 updates in September 2024*

<a name="entry-1290078652939112509"></a>

## 2024-09-29 22:31 - Entry 1290078652939112509
**Author:** Aporia

Pending Patch:

```
- Iron Oxide spawns fixed in Steamfont Mountains.
- SH Casino (Therin Asakith) now properly rewards all illusion items
- Lambent Boots, Gaunts, and Greaves quest turn ins have been fixed
- Staff of Writhing proc rate has been fixed across all versions
- Satchel of the Hero is now no drop and has 100% WR
- Gnome Warrior GM, Narron Jenork has returned and once again offers his Watchman Boots quest
- Ranger AA Protection of the Spirit Wolf CD reduced to 15 minutes
- Plane of Sky quest Test of Preparation fixed
- Lower Guk WP move from Safe Hall to Undead Side Entrance
- Jboots click effect changed for Lego version!
- Spirit of Cheetah recast time lowered to 3 minutes
- Swarm Pet Mistwalker HP increased to 600
- Clarified description on Paladin's Blessing of Light AA
- Shaman AA Rabid Bear now gives double attack/regen/cold resist at rank 1. These stats and proc chance have been lowered across Rk 2 and 3.
- Cleric AA Divine Avatar now gives higher stats at lower ranks but has had its effect cap reduced on max ranks.
```

---

---

<a name="entry-1288893446676807752"></a>

## 2024-09-26 16:02 - Entry 1288893446676807752
**Author:** Catapultam

PENDING

```
* Added Beastlord and Berserker to a number of old-world items which were missing them
* Reduced aggro transfer from taunt-off pets to owner
* Consume Item will no longer delete items as they become Legendary
* Improved NPC Model Upgrade routines
  - Fixed Wolf Models
* Racial skills add to skillcaps
* Improved skill-up messages (shows current/cap)
* Fixed access to #myskills
* Fixed access to #mystats
* Reduced CD of Bestial Alignment
* SE_MeleeLifetap applies to SpecialAttackDamage
* Fixed containers for 'Strike of Shissar N' poisons
```

---

---

<a name="entry-1288338475724312656"></a>

## 2024-09-25 03:17 - Entry 1288338475724312656
**Author:** Catapultam

```
* EoM Loot Buff increases Item XP rate
* Mobs will IGNORE pets which have pet taunt off; all aggro the pet would have generated is transferred to their owner.
* Pet AoEs now work without the pet having aggro on each mob individually first.
* Legendary Augments are no longer attuneable.
```

---

---

<a name="entry-1288303500970692668"></a>

## 2024-09-25 00:58 - Entry 1288303500970692668
**Author:** Catapultam

```
* Fixed infinity buff stacking from non-class sources
* Fixed crash bug
* Fixed attune-on-exp bouncing
```

---

---

<a name="entry-1287917817815109632"></a>

## 2024-09-23 23:25 - Entry 1287917817815109632
**Author:** Catapultam

```
* Fixed Bard foci (again)
* Legendary items are once again Attuneable
* Attuneable items become no-drop when you gain experience with them equipped, rather than immediately upon equip.
* Fixed pet target HoTT
* Fixed per commands breaking if you have a familiar as first pet
* Fixed familiars attacking if you have something other than a familiar as first pet
* Improved coherency of pet window swapping
* Fixed losing access to pet window if charm pet was focused pet when it died\charm broke
* Buff stacking is bypassed for spells you cast against other buffs you cast which don't share a class
```

---

---

<a name="entry-1287147068732997703"></a>

## 2024-09-21 20:22 - Entry 1287147068732997703
**Author:** Catapultam

```
* Only Must-Equip clickies will become attuned when clicking from inventory
* Numerous quest script fixes
* Honey, I shrunk the bats.
```

---

---

<a name="entry-1286425410141290609"></a>

## 2024-09-19 20:35 - Entry 1286425410141290609
**Author:** Catapultam

```
- Fixed Disc Timers
- Totally nuked all traces of LDON camps
- Lost track of bug fixes.
- FD should no longer cure debuffs
- Pet debuffs should be removed on resting, skipping ones cast by their owner to faciliate charm.
- Pet bag and multiple pets plays nice now
- Project Illusion now works on Pets.
- Fixed BS with non-1hp damage
- Power Source no longer applies stats.
- Improved stacking of proc spells (multi-class proc spells will stack)
- Improved stacking of DS (multi-class DS will stick, but not every DS from same class)
```

---

---

<a name="entry-1286236109008797730"></a>

## 2024-09-19 08:03 - Entry 1286236109008797730
**Author:** Retribution EQ #change-log

Pending Patch

```
- Instruments now display their correct Resonance level based on item tier.
- Tier 1 and 2 items are always magical.
- Bard Epic instrument effect corrected
- Fixed Bash reuse timer w\ haste
- Fixed clockwork summons
- Fixed wizard sword\cleric hammers
- Added Beastlord and Berserker to a number of old-world items which were missing them
- Reduced CD of Bestial Alignment
- SE_MeleeLifetap applies to SpecialAttackDamage
- Fixed containers for 'Strike of Shissar N' poisons
```

---

---

<a name="entry-1286022083201208392"></a>

## 2024-09-18 17:52 - Entry 1286022083201208392
**Author:** Catapultam

```
* Restored Fury of Magic, Spell Casting Fury, Destructive Fury to Hybrids
* (Ingenuity was never removed)
* Ingenuity now works as described - it ONLY affects spells from items (Procs, Clicks)
* Return to the Valley Beneath the Son of Fixing Power Source Dupes
* Removed several duplicated AA
* Adjusted client validation so that it does not boot players from Bazaar, and gives more info on how to get correct client.
```

---

---

<a name="entry-1285646038744567849"></a>

## 2024-09-17 16:58 - Entry 1285646038744567849
**Author:** Catapultam

```
* Hopefully fixed power source dupe (again again)
* Removed Fury of Magic AA from Hybrids again
```

---

---

<a name="entry-1285383939115978868"></a>

## 2024-09-16 23:36 - Entry 1285383939115978868
**Author:** Catapultam

```
* Clickies become attuned when successfully clicked.
* Fixed power source upgrading from duping items (for real this time)
* Mandatory 0.5s recast removed Beneficial instant-clicks.
* Exclude Pacify and Mez from Cascade of Decay
* Pets will taunt undead mobs now (?!)
* All Weapon Proc (SPA 85) spells stack
```

---

---

<a name="entry-1285073862718918656"></a>

## 2024-09-16 03:04 - Entry 1285073862718918656
**Author:** Aporia

Pending Patch:

**Discipline Timer Rework**

As you know shared timers between different class discs for melee and hybrid classes has been a huge hinderance in their expected cross performance.

A decision was made on how to make this work within the confines of the system.

After next patch:

ALL OFENSIVE DISCIPLINES, BETWEEN CLASSES, WILL NO LONGER SHARE A COOLDOWN.

Offensive disciplines that shared a cooldown WITHIN a single class, continue to share a cooldown.

ALL DEFENSIVE DISCIPLINES, BETWEEN CLASSES, WILL NOW SHARE A COOLDOWN. (All riposite Discs will share a timer, all dodge, parry, and damage reduction Discs will share a timer).

Defensive disciplines that shared a cooldown WITHIN a single class, continue to share a cooldown.

This will be a net increase in DPS for those stacking melee classes and a net decrease in certain mitigation combinations.

*Note: This is disciplines ONLY not AA.*

---

---

<a name="entry-1285072099698016303"></a>

## 2024-09-16 02:57 - Entry 1285072099698016303
**Author:** Retribution EQ #change-log

Pending Patch

```
Trueshot Discipline increased hit chance was broken. It has been fixed (0 to 12%).

Berserker Discs - Head Strike, Leg Strike, Leg Cut, Head Pummel, Head Crush, Divertive Strike, and Distracting Strike, have had their reagent requirements removed. They also now share a CD with Throw Stone.

Berserker Disc Focused Fury increased hit chance was broken. It has been fixed (0 to 50%).

Warrior Disc Precision increased hit chance was broken. It has been fixed (0 to 50%).

Monk Discs - Phantom Wind, Zephyr, Echo, and Call now share a CD with Throw Stone
```

---

---

<a name="entry-1284796823336259585"></a>

## 2024-09-15 08:43 - Entry 1284796823336259585
**Author:** Retribution EQ #change-log

```
* Hole door is now 'click to enter' instead of being a literal door
```

---

---

<a name="entry-1284767213877854229"></a>

## 2024-09-15 06:46 - Entry 1284767213877854229
**Author:** Catapultam

```
* Fix dupe when upgrading items with power source
* Low-level characters get a multiplier on power source leveling rate.
* Unresistable spells are actually unresistable
* Short-Duration buffs no longer zone with pet.
```

---

---

<a name="entry-1284649224260292678"></a>

## 2024-09-14 22:57 - Entry 1284649224260292678
**Author:** Aporia

```
Hell levels removed for real this time.
```

---

---

<a name="entry-1284637798019633182"></a>

## 2024-09-14 22:11 - Entry 1284637798019633182
**Author:** Retribution EQ #change-log

Pending Patch

```
Enchanter AA Phantasmic Reflex has been changed. ALL SPELLS cast by an enchanter, now have a SMALL chance to grant the caster SMALL rune.

Legendary Staff of Writhing and Legendary Ancient Prismatic Staff now have had their proc restored in addition to their click.
```

---

---

<a name="entry-1284366282204123227"></a>

## 2024-09-14 04:13 - Entry 1284366282204123227
**Author:** Catapultam

```
* Attempt to resolve issues with power source upgrading to legendary
* Reduced floor on legendary experience scalar for item upgrading
* AA Abilities now use implied targeting
* Spirit of Cheetah moved to short duration buff box
* Combat Mana\HP\Endurance Regeneration is now displayed the actual value from the server.
* Resists now display the actual value on the server
```

---

---

<a name="entry-1284232804883890287"></a>

## 2024-09-13 19:22 - Entry 1284232804883890287
**Author:** Catapultam

```
* Druid DS now scales correctly
* Fixed several issues surrounding being unable to manipulate inventory while casting.
* Expected behavior\Please test the following specifically;
  - Inventory, Hotkeys, Skills, etc should be usable while casting
  - Spell casting messages (for self and other) should be created correctly.
  - Spell interrupt messages should be created correctly.
  - Bard Song interrupt messages should be created correctly (no cast messages for Bard Songs)
  - Monk alt-appearance gear should use unique graphics
```

PATCH REQUIRED

---

---

<a name="entry-1283931437963149325"></a>

## 2024-09-12 23:25 - Entry 1283931437963149325
**Author:** Catapultam

```
* Debuffs now clear automatically when ending combat
* Fixed bug causing 'You are weakened and cannot rest' to display inappropriately.
* Rogues can backstab with any weapon
* Cleaned up casting and interrupt messages (THIS WAS ACTUALLY REALLY CLEVER GUYS)
* There is now a minimum time between activating Bandolier sets (10 seconds).
* Monk skill attacks now trigger Fists of Steel proc (but not damage)
* Added Situational Awareness AA - Increases Tracking skill by 10 points per rank.
```

---

---

<a name="entry-1282507287625469994"></a>

## 2024-09-09 01:06 - Entry 1282507287625469994
**Author:** Catapultam

```
- Detrimental spells now stack with beneficial spells.
  - ie; If you have SoW and get Snared, your run speed is now SoW speed minus the Snare reduction
- Short Duration spells (Song Window) no longer have stacking conflicts with normal buffs.
- If somehow a short duration buff overwrites a long duration buff, or vis versa, they will go to the correct window.
```

---

---

<a name="entry-1281396861147676696"></a>

## 2024-09-05 23:33 - Entry 1281396861147676696
**Author:** Retribution EQ #change-log

```
Spirit of the Howler Pet level increased.
Nature Walker's Behest Pet HP reduced.
Torturing Winds Debuff reduced to 2 minutes from 2 hours.
```

---

---

<a name="entry-1280206113660473560"></a>

## 2024-09-02 16:42 - Entry 1280206113660473560
**Author:** Retribution EQ #change-log

```
- Deleted several RC and Apoc 'tradeskill tools'
- Quests which check for the presence of items now correctly detect when those items are in the bottom two slots of inventory.
_ Clockwork Bankers and Merchants now work again, and are no longer 'pets'.
_ Mage Epic pet is affected by pet focus items once again
- Tearel should be more reliable
_ AHR now triggers correctly when all other bosses in zone are dead.
- AHR spawn conditions survives zone reset.
- Thylex of Veeshan is far less talkative
- Fixed SoL-completion Bag Upgrade
```

---

---

<a name="entry-1280040224138727529"></a>

## 2024-09-02 05:42 - Entry 1280040224138727529
**Author:** Retribution EQ #change-log

```
Effective now:

remains of Vah Kerrath no longer randomly eats Soul Essences

NE Tower in Sanctus Seru now has working teleporters

Luclin BST pet has slightly increased base stats and now correctly benefits from PP20 gauntlets from VT

On reboot:

Certain ranger selfbuff procs that were unable to proc from archery, now proc from archery

Certain item clickies no longer require reagents

Group ports now work again when players are in an instance
```

---

---

