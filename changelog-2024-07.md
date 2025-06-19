---
title: Changelog - July 2024
description: Changelog entries for July 2024
published: true
date: 2025-06-19T23:04:51.998Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:51.998Z
---

# Changelog - July 2024

[← Back to Recent Updates](/en/Change-log-history) | [← June 2024](/en/changelog-2024-06) | [August 2024 →](/en/changelog-2024-08)

---

*34 updates in July 2024*

<a name="entry-1264807693298962432"></a>

## 2024-07-22 04:54 - Entry 1264807693298962432
**Author:** Retribution EQ #change-log

```
Pending Patch:

All World Buffs now correctly count down when in Bazaar.
Holy Elixir once again stacks with other HoTs
```

---

---

<a name="entry-1264518059532750898"></a>

## 2024-07-21 09:43 - Entry 1264518059532750898
**Author:** Retribution EQ #change-log

Rolling Next Update Changelog...
```
- Echo of Luck now guarantees Apocryphal rewards for quests
- Sympathetic Proc buffs now actually 16hr duration
- Sympathetic Procs can trigger even if the spell cannot apply to a mob (ie, Symp Heal can proc even if the buff was blocked)
- ST_SummonedPet handled correctly be implied targeting. (Petamorph wands)
- Bards are no longer compelled to sing forever.
- Fixed Berserkers not hitting more than 1x with Frenzy
- Fixed Froglok Beastlord warders.
- Familiar spells will no longer dismiss other types of pets when they fade.
- Ikaav's Venom now has a spell icon.

# Augmentation Overhaul #
- Augment Slots standardized across all items, into the following types;
   - Type 1 (Stats): All equippable items have at least one of these slots. Augs with only stats will fit into these slots.
   - Type 2 (Worn): Equippable items without a focus or worn effect will have one of these slots. Augs wih a Focus or Worn effect, along with Type 1 augs, will fit in these slots.
   - Type 3 (Spells): Currently unused.
   - Type 4 (Procs): All Weapons have at least one of these slots. Augs with Procs, Damage, Bane Damage, Elemental Damage, or Type 3 augments will fit in these slots.
   - Type 20 (Ornament): All PRI\SEC\RANGE items will have one of these slots for statless ornaments.
   - Type 21 (Ornament): All Visible Slot equipment will have these slots (Currently unused).
   - Two-Handed weapons have an additional Type 1 and Type 4 slot compared to 1-handed items.

- This should provide additional coherence to augment itemization, remove the relatively meaningless type 7\8 split, allow for items without foci\worn effects to be a little more valuable, and provide a much-needed boost to two-handed weapons.
- Any augments in slots which are no longer valid will be ejected from items when this gets deployed, and will need to be reinserted.

** THJ ONLY**
- (THJ) AA can be activated while casting
- (THJ) Items can be augmented even if it would result in an item that you can no longer use
- (THJ) Fixed Archery procs.
- (THJ) Fixed Reyfin Malakwa for Multiclass characters
- (THJ) Items upgraded to Legendary via Power Source now correctly show as attuned.
- (THJ) Legendary items may no longer be equipped in Power Source, and Enchanted->Legendary upgrades will eject the item from the Power Source instead of infinitely soaking XP
** THJ ONLY**
```

---

---

<a name="entry-1264297691672743948"></a>

## 2024-07-20 19:07 - Entry 1264297691672743948
**Author:** Retribution EQ #change-log

```
- Actually, for sure, definitely, REALLY fixed Eejag this time
- Phara Dar's adds should now aggro correctly.
```

---

---

<a name="entry-1263912204261134387"></a>

## 2024-07-19 17:35 - Entry 1263912204261134387
**Author:** Retribution EQ #change-log

Immediate Effect:
```
- Low-AA bonus increased to 400%. At 0AA, you will recieve a 4x bonus to AAXP, decreasing linearly until a total of 300AA have been earned
```

---

---

<a name="entry-1263752537756930080"></a>

## 2024-07-19 07:01 - Entry 1263752537756930080
**Author:** Retribution EQ #change-log

Pending Next Reboot\Patch
```
- Echo of Luck now guarantees Apocryphal rewards for quests
- Sympathetic Proc buffs now actually 16hr duration
- Sympathetic Procs can trigger even if the spell cannot apply to a mob (ie, Symp Heal can proc even if the buff was blocked)
- ST_SummonedPet handled correctly be implied targeting.
- Bards are no longer compelled to sing forever.
```

---

---

<a name="entry-1263652317794930688"></a>

## 2024-07-19 00:23 - Entry 1263652317794930688
**Author:** Retribution EQ #change-log

Consolidated Changelog:

```
- Help Baelin quest fixed.
- Battle Master Ska`tu loot tables fixed.
- Shaman Cudgel quest 6 fixed.
- Howling Stone final key fixed.
- Silver Wand and silvered guard fixed.
- Eejag now spawns where that impudent sprite is.
- Rage of Zomm and Dyzil's Deafening Decoy work once again.
- SK Viscious Bite of Chaos recourse now stacks with Lich instead of overwrites.
- Priest of Najena now correctly always drops Tarnished Bronze Key
- The Undertake Lord once again has a name.
- The Skeletal Sepulcher once again has a name.
- Spell: Invigor has been removed from all merchants.
- Ragebringer proc has had it's radius reduced.
- Robe of Living Fungus now has HP Regen again.
- The following rogue abilities may now be used in combat:
    Rogue Abilities Sneak Attack (20)
    Thief's Vengeance (52)
    Assassin's Strike (63)
    Kyv Strike (65)
    Ancient Chaos Strike (65)
    Daggerfall (69)
    Razorarc (70)

- 'Must Equip' items can be cast from inventory if they are attuned

- Sympathetic Strike of Flames replaced with Sympathetic Strike
- All Sympathetic 'Strike-like' abilities replaced with Sympathetic Strike
  - Prismatic Resist (average resist of target)
  - Partial resists enabled
  - 16h duration, undispellable
  - Triggers on EVERY cast (same as healing), stacks with all similar abilities, such as the Pyromancy AA from wizards

- Sympathetic Healing Burst replaced with Sympathetic Healing
 - 16h duration, undispellable

- Ground spawns are now present in non-respawning DZ
- Swarm pets will aggro everything that has their owner on its hate list
- Certain quests which check for the presence of an item in your inventory will work correctly with RC\Apoc items

- Inventory data is now sent in the seconds following a zone transition, instead of during the zone. This is intended to mitigate crash-on-zone issues.
IF YOU ENTER A ZONE AND HAVE AN EMPTY INVENTORY, ZONE BACK OUT IMMEDIATELY AND REPORT IT AS A BUG BY TAGGING A GM. Your items are safe as long as you don't manipulate your inventory while it is empty.


AA Exp Scaling has been enabled for the first 300AA.
This means there is a 200% AA exp bonus for your first AA that scales down as you approach 300. At 300 AA, this bonus goes away.
This change is meant to aid: players catching up, alts, and classes that take higher AA investments to come into their own.
This bonus stacks with the server wide EXP bonus.
```

---

---

<a name="entry-1263595829432946698"></a>

## 2024-07-18 20:38 - Entry 1263595829432946698
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

<a name="entry-1263523992602546348"></a>

## 2024-07-18 15:53 - Entry 1263523992602546348
**Author:** Retribution EQ #change-log

Pending Reboot:
```
* Fixed and re-enabled AAXP Scaling based on total earned AA
* Symp proc durations reduced to 16h from Permanent
```

---

---

<a name="entry-1263354038532182178"></a>

## 2024-07-18 04:37 - Entry 1263354038532182178
**Author:** Retribution EQ #change-log

```
AA Exp Scaling has been enabled for the first 300AA.

This means there is a 200% AA exp bonus for your first AA that scales down as you approach 300. At 300 AA, this bonus goes away.

This change is meant to aid: players catching up, alts, and classes that take higher AA investments to come into their own.

This bonus stacks with the server wide EXP bonus.
```
Edit: Temporarily Reverted.

Necromancer AA Soul Seeker CD reduction reduced to 2 minutes per rank. Leaving max rank LB at 5 minutes. Please do not pretend you though LB was supposed to have no CD. Thanks.

---

---

<a name="entry-1263233303608164353"></a>

## 2024-07-17 20:38 - Entry 1263233303608164353
**Author:** Retribution EQ #change-log

Still pending reboot:
```- 'Must Equip' items can be cast from inventory if they are attuned

- Sympathetic Strike of Flames replaced with Sympathetic Strike
- All Sympathetic 'Strike-like' abilities replaced with Sympathetic Strike
  - Prismatic Resist (average resist of target)
  - Partial resists enabled
  - 16h duration, undispellable
  - Triggers on EVERY cast (same as healing), stacks with all similar abilities, such as the Pyromancy AA from wizards

- Sympathetic Healing Burst replaced with Sympathetic Healing
 - 16h duration, undispellable


- Ground spawns are now present in non-respawning DZ
- Swarm pets will aggro everything that has their owner on its hate list
- Certain quests which check for the presence of an item in your inventory will work correctly with RC\Apoc items```

---

---

<a name="entry-1263204566200221839"></a>

## 2024-07-17 18:43 - Entry 1263204566200221839
**Author:** Retribution EQ #change-log

```
Pending Reboot:

- Help Baelin quest fixed.
- Battle Master Ska`tu loot tables fixed.
- Shaman Cudgel quest 6 fixed.
- Howling Stone final key fixed.
- Silver Wand and silvered guard fixed.
- Eejag now spawns where that impudent sprite is.
- Rage of Zomm and Dyzil's Deafening Decoy work once again.
- SK Viscious Bite of Chaos recourse now stacks with Lich instead of overwrites.
- Priest of Najena now correctly always drops Tarnished Bronze Key
- The Undertake Lord once again has a name.
- The Skeletal Sepulcher once again has a name.
- Spell: Invigor has been removed from all merchants.
- Ragebringer proc has had it's radius reduced.
- Robe of Living Fungus now has HP Regen again.
- The following rogue abilities may now be used in combat:

Rogue Abilities Sneak Attack (20)
Thief's Vengeance (52)
Assassin's Strike (63)
Kyv Strike (65)
Ancient Chaos Strike (65)
Daggerfall (69)
Razorarc (70)

```

---

---

<a name="entry-1262942533567250433"></a>

## 2024-07-17 01:22 - Entry 1262942533567250433
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

<a name="entry-1262828889718390885"></a>

## 2024-07-16 17:51 - Entry 1262828889718390885
**Author:** Retribution EQ #change-log

Immediate Effect:
```
- Parcels are now available.
- Various merchants associated with the League of Antonican Bards can send\recieve Parcels
- Mysterious Mailman added to Bazaar
- Bazaar purchases via Parcel are now enabled
```

---

---

<a name="entry-1262772314844565504"></a>

## 2024-07-16 14:06 - Entry 1262772314844565504
**Author:** Retribution EQ #change-log

(Next Reboot)
```
- Heroic Charisma is now applied as a direct resist adjustment to spells. (ie; 67 HCha is -67 additional resist check to all spells)
- Improved mob pathfinding
```

---

---

<a name="entry-1262638983905804308"></a>

## 2024-07-16 05:16 - Entry 1262638983905804308
**Author:** Retribution EQ #change-log

```
Pending Patch:
Rage of Rallos Zek AA - Endurance Cost Reduced by 1/4

Key requirements in Seb have been removed
```

---

---

<a name="entry-1262519984828055644"></a>

## 2024-07-15 21:23 - Entry 1262519984828055644
**Author:** Retribution EQ #change-log

Working through these right now, post in the related suggestion thread if you have any in particular you want to get hit. (https://discord.com/channels/1019251428637814874/1242512903136083968)
```
* The following spells have separated illusion and benefit components.
- Elemental Form: Air
- Elemental Form: Water
- Elemental Form: Fire
- Elemental Form: Earth
- Form of the Bear
- Form of the Great Bear
- Boon of the Garou
- Trickster's Augmentation
- Wolf Form
- Greater Wolf Form
- Share Wolf Form
- Form of the Great Wolf
- Share Form of the Great Wolf
- Form of the Howler
- Form of the Hunter
- Feral Form
- Spirit of the Black Wolf
- Spirit of the White Wolf
- Visage of the Dark Arachnid

* Added Vial of Prismatic Dye to possible rewards from 'A Mischievous Halfling'.
* Tradeskilled Poisons now stack to 100
* Tradeskilled Poisons with more than one 'hit charge' now have unlimited 'hit charges'
* Frenzied Burnout rank 2->6 are now available at level 51
```

---

---

<a name="entry-1262263403842633804"></a>

## 2024-07-15 04:24 - Entry 1262263403842633804
**Author:** Retribution EQ #change-log

```
* GlobalLoad updated (requires client patch)
* New Beastlord Warders
 * Human - Puma
 * Erudite - Kobold
 * Wood Elf - Green Drake
 * High Elf - Blue Drake
 * Dark Elf - Black Drake
 * Half Elf - Red Drake
 * Dwarf - Goblin
 * Halfling - Snake
 * Gnome - Junk Beast
 * Froglok - Sporali
 * Drakkin - Gold Drake
* Disabled mob summoning players who are already in melee range
```

---

---

<a name="entry-1262158250791534674"></a>

## 2024-07-14 21:26 - Entry 1262158250791534674
**Author:** Retribution EQ #change-log

Pending Patch/Reboot

```
Mage Epic pet now summons at lvl 58, up from 52.
Mage Water/Fire/Air/Earth pet (lvl 60 cast) with PP 10 now summons at level 58, down from 60.
Veksar ZEM increased to 2.0
All splitpaw respawn times have been corrected down to 10.5 minute spawns.
King-me cleaned up
Misc Upstream Bug fixes from upgrading to new binaries
MANY random crash fixes

/bazaar now functions! (Parceling does not yet work).
```

---

---

<a name="entry-1261703391629938810"></a>

## 2024-07-13 15:18 - Entry 1261703391629938810
**Author:** Retribution EQ #change-log

Pending Reboot:
```
All Beastlord's now have their own racial pets again. Pets added:

Human - Puma
Froglok - Fungusman
Dark Elf - Black Widow
Gnome - Junkbeast
Dwarf - Green Goblin
Halfling - Bixie
High Elf - Fairy
Erudite - Kobold
Half Elf - Giant Bat
Wood Elf - Wasp

Worlace now offers key Poison Making ingredients and has been joined by his cohorts Chryssa and Dolley. Rogues- yes you shoud be making poisons.

Many Misc Bug Fixes
```

---

---

<a name="entry-1261435868669808662"></a>

## 2024-07-12 21:35 - Entry 1261435868669808662
**Author:** Retribution EQ #change-log

```
- Removed the cost of most starting AA
- Added Group Shrink to Beastlord auto-grant AA
- All classes with pets now get auto-grant Summon Companion
- All classes with pets or charm now get auto-grant Pet Affinity
- Mage 'Companion's Fury' auto-grant replaced with 'Elemental Fury'
- Lay on Hands is now auto-granted as it becomes available through level 50
- Harm Touch is now auto-granted as it becomes available through level 50
- Archery Mastery is now auto-granted as it becomes available through level 50
```

---

---

<a name="entry-1261218240906919977"></a>

## 2024-07-12 07:11 - Entry 1261218240906919977
**Author:** Retribution EQ #change-log

Extra stuff for Kunark
```
- Replaced the level 51 Mage Seasonal AA.
- Replaced Companion of Necessity with Dimensional Armory. Summons a 10-slot, Lore, No-Drop, (Not Temporary) 100% WR container. Any items placed inside this container will be automatically equipped by your summoned pets.
- Pets will now properly proc augments and display ornaments.
- (Summoned) Pet base damage is now influenced by the weapons they are wielding.

- Some auto-granted AA had their costs removed. This may cause your total AA spend count to go down. Expect to see more of this in the future.
```

---

---

<a name="entry-1260981600993284190"></a>

## 2024-07-11 15:30 - Entry 1260981600993284190
**Author:** Retribution EQ #change-log

Pending Patch/Reboot:

```
Beacon of Loathing now correctly has an RC and Apoc counterpart.
Ranger AA Ranged Finesse no longer displays incorrectly.
Cleric AA Celestial Regeneration now stacks with their regular HoT lines.
Zerker AA Cascading Rage no longer slows you and correctly gives haste instead.
Echo of Luck and Echo of Focus can no longer be dispelled.
Rogue AA Seized Opportunity is now auto-granted at level 1 with maximum effectiveness.
Rogue AA Virulent Venom has had its first and second-rank costs reduced.
Rogues can now purchase an upgraded version of the Strikethrough AA.
Rogue AA Massive Strike base damage increased from 30 to 35.
Rogue AA Massive Strike Rk II is now available.
Monks now start with RK I of Killing Spree like all other pure melee.
Ranger AA Precision of the Pathfinder now affects Archery accuracy but at a reduced rate.
Gift of Mana now correctly shows its effect from level 30-70 spells.

```

**Kunark Launch time changed to 7PM EST, 6PM CST,  due to RL conflicts.** Spread the word.

---

---

<a name="entry-1260963856692285571"></a>

## 2024-07-11 14:20 - Entry 1260963856692285571
**Author:** Retribution EQ #change-log

```
- Mobs will no longer respawn at 22hr in Non-Respawning instances (to coincide with increased dz lifetimes)
```

---

---

<a name="entry-1260840422658277490"></a>

## 2024-07-11 06:09 - Entry 1260840422658277490
**Author:** Retribution EQ #change-log

```
- Temporary pet combat messages should now be visible.
- Pet names for temporary pets, familiars, etc are a bit more descriptive
```

---

---

<a name="entry-1260793098468986932"></a>

## 2024-07-11 03:01 - Entry 1260793098468986932
**Author:** Retribution EQ #change-log

```
- 'Unlocking' (Even if still time-locked) Velious now allows bypass of key requirement for Veeshan's Peak.
- 'Unlocking' (Even if still time-locked) Planes of Power now allows bypass of key requirement for Vex Thal.
```

---

---

<a name="entry-1260793093314183179"></a>

## 2024-07-11 03:01 - Entry 1260793093314183179
**Author:** Retribution EQ #change-log

```
- Sage of Anachronism can now expand your hole(s)
- Sage of Anachronism will replace lost First Orb of Retribution
```

---

---

<a name="entry-1260793044303613973"></a>

## 2024-07-11 03:01 - Entry 1260793044303613973
**Author:** Retribution EQ #change-log

```
- Pet taunt will now enable them to peel off of players.
- Pets will now taunt any mob attacking their owner during their taunt cycle, even if that is not the mob they are currently attacking.
```

---

---

<a name="entry-1260056954194366534"></a>

## 2024-07-09 02:16 - Entry 1260056954194366534
**Author:** Retribution EQ #change-log

```
- You will now recieve a notification when Echo of Luck or Seasonal status upgrades a quest reward.
- You will now recieve an upgrade when Seasonal status upgrades a loot reward.
- Really fixed Staff of Forbidden Rites charges.
```

---

---

<a name="entry-1260042653442117735"></a>

## 2024-07-09 01:19 - Entry 1260042653442117735
**Author:** Retribution EQ #change-log

On next patch:
```
- Echo of the Past added to The Howling Stones
- Zerker AA Decap has had its damage reduced
- Echo of the Past added to ChardokB
- Echo of the Past added to Veksar
- VP 2.0, ChardokB, and Veksar have had their items scaled down in anticipation of Kunark launch. VP 2.0 was done with the intent that end game Velious gear (NToV) outpaces it in most scenarios.
```
For those of you new to the server,  balance changes are ongoing, both buffs and nerfs will happen to outliers. I try to lean toward buffs for others instead of nerfs for the one- but outliers have to be handled.

---

---

<a name="entry-1259987424134565927"></a>

## 2024-07-08 21:40 - Entry 1259987424134565927
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

<a name="entry-1259187477865037886"></a>

## 2024-07-06 16:41 - Entry 1259187477865037886
**Author:** Retribution EQ #change-log

Rebooting to bring live pending changes as well as:
```
- Enchanters gain access to Bite of Tashani AA
- Sky weapon efreeti standard is now magic
- Summon Companion AA now available to Druids
- Sky quest rewards that were later swapped for better versions have now been swapped for their better versions.
- Inny no longer depops.
- Berserker AA Untamed Rage now correctly adds haste instead of subtracts.
- Several misc bugs/suggestions/king-mes completed.
- Magician Fire/Stone/Ice/Vapor Core AA cooldown reduced to 15min
- Charges on Staff of Forbidden Rites have been normalized and no longer scale with quality (Each version now has 50).
- Charm crashing zones *should* be fixed.
```
Thank you all for being here! Server buffs going out for unexpected reboots.

---

---

<a name="entry-1258612926680531044"></a>

## 2024-07-05 02:38 - Entry 1258612926680531044
**Author:** Catapultam

```
- Removed 'Expanded Pet Affinity' (for now, might do something with this concept later)
```

---

---

<a name="entry-1258140468093517824"></a>

## 2024-07-03 19:21 - Entry 1258140468093517824
**Author:** Retribution EQ #change-log

Pending Patch/Reboot

```
- Spirit Salve no longer requires line of sight to cast.
- WP added to Everfrost near Permafrost.
- Bixie Sword Blade now correctly drops from Bazzt Zzzt
- PoSky quest "Test of Body" now rewards the correct item
- Stein of Moggok changed back to it's original form. Apoc version maintains its sympathetic proc
- Eejag no longer spawns within invisible walls
- Rogue AA Mrylokar's Rigor now procs 25% of the time, up from 2.5%
- Echo of the Past removed from Feerrott. The Echo inside Fear by the WP now works correctly.
- Verina Tomb respawn timer lowered to 4 hours with a 30 minute variance
- Vessel Drozlin respawn timer lowered to 4 hours with a 30 minute variance
- The Tangrin, and Oracle of K`arnon respawn timer lowered to 4 hours with a 30 minute variance
- Keeper of Souls no longer double spawns
- Increased Enchanter AA Phantasmic Reflexes chance to proc (may be adjusted again)
- WP Added to TD
- Echo of the Past added to TD
- Echo of the Past added to FM
- WP Added to FM
- Beastlords can now purchase Group Shrink AA
```

---

---

<a name="entry-1257195892344225883"></a>

## 2024-07-01 04:47 - Entry 1257195892344225883
**Author:** Retribution EQ #change-log

Upcoming Changes Pending Patch/Reboot:

```
- Apoc Six Note Blade now WAI
- Cazic 2.0 loot brought into line with Classic expectations.
- Marsinger's Gem quest items brought into line with Classic expectations (this is a large change as it was late Luclin quality).
- Dyllin Starsine's quest drops increased.
- All Bard Instruments can now be equipped in the Range slot.
- Monk Sky Weapon Requisite, Brass Knuckles, now drop from Noble and Hand
- BST AA Frenzied Swipes now correctly lowers the CD of Feral Swipe to 3 seconds for 30 seconds.
- Disarm now moves the enemies equipment directly into inventory
- Luclin and PoP Necromancer pet power combinations have been updated based on enhanced classic stats
- Echo added INSIDE fear next to glyph circle.
- Nedaria's Landing should not be accessible until GoD.
- Rune spell cost brought in line to heal cost.
- Bards can once again use clickies while moving
- Fear, Mez, Charm, Silence, and Root will now check a players resist EVERY tick as intended
- Progression NPCs (Faded Memories) now look correct.
- Tykar Renlin works correctly again.

```
Quick note:

When something is found that is out of era that directly impacts player power, please report it. Assume any OoE item will be brought into line with expectations for availability in whatever expansion it becomes available here. We appreciate your support and understanding as we continue to make Retribution the best it can be.

Thank you!

---

---

