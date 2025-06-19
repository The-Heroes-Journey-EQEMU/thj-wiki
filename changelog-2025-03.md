---
title: Changelog - March 2025
description: Changelog entries for March 2025
published: true
date: 2025-06-19T23:04:18.831Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:18.831Z
---

# Changelog - March 2025

[← Back to Recent Updates](/en/Change-log-history) | [← February 2025](/en/changelog-2025-02) | [April 2025 →](/en/changelog-2025-04)

---

*11 updates in March 2025*

<a name="entry-1354667173997449316"></a>

## 2025-03-27 04:03 - Entry 1354667173997449316
**Author:** Catapultam

```
- Removed level requirement from the Plane of Time.
- Exp gain from level 63 to 65 has been increased.
- Pet level adjusted for BST/NEC/ENC pets using Time focus.
- Respawn time in Plane of Tactics and Plane of Water have been reduced to match other respawn times.
- Pheonixs in Plane of Fire no longer charm (and/or crash your game).
- Echo added to Tenebrous Mountains.
- Echo added to Dalnir's Crypt.
- Aid Grimel should now be able to be completed.
- Added 2nd Type 4 augment slot to Bows
- Augments currently Slotable in type 1 & 2 are now also slotable in type 4.
- Plane of Time - Phase 4 and later bosses should no longer double-spawn
- NUMEROUS Plane of Time fixes and adjustments to bring events more in-line to expectations
- Reworked Plane of Earth ring events
- Askr no longer despawns in Non-Respawning instances
- Trial of Torture now properly granting flags

- The approximately one thousand characters who achieved level 65 prior to this patch will recieve the title 'of the One Thousand'
```

---

---

<a name="entry-1352847240527609957"></a>

## 2025-03-22 03:31 - Entry 1352847240527609957
**Author:** Catapultam

Running changelog for Post-PoP hotfixes.
```
- Corrected flagging logic for Aerin`Dar event.
- Corrected flagging logic for Grummus event
- Corrected flagging logic for Hedge event
- Corrected goup port logic for PoJ trials (@Gregggggg)
- Corrected group port logic for Keeper of Souls (@Greggggg)

- Fixed zone crash related to tradeskills
- Fixed inability to mix enchanted\legendary in standard tradeskill combines
```

---

---

<a name="entry-1352780161384317089"></a>

## 2025-03-21 23:05 - Entry 1352780161384317089
**Author:** Catapultam

Part 2
```
*** KNOWN ISSUES ***
- The Plane of Time expedition does not currently recover cleanly from being fully shut down during PHASE 3. Please complete Phase 3 before leaving the zone for any extended period of time.

Misc
 - Removed all spells and disciplines from vendors which are otherwise obtainable from quests in PoP.
 - Celestial Fists are now Must-Equip to click (Reminder, Must-Equip can click from inventory once attuned)
 - Mobs should no longer restore from saved state with 0 hp
 - Mobs should no longer slowly levitate into the air as zone is suspended and reloaded
 - Adjusted several PoP ZEMs
 - Nerfed Mnk/Mnk/Mnk
 - Added PoK book to Bazaar
 - Added many new Enchanted\Legendary items, should have full coverage now.
 - Valentine's Day buffs have come to an end!

POP Events
 - Planes of Power progression flags are *account wide*
 - Check the Storyline window for a flagging guide!
 - HoHA - Crazed Norrathians now have a one minute timer before spawning in each room. (Pippz)
 - Agnarr - Stun duration cut in half. 15s Recast Added.
 - Tallon Zek PoTactics - Knockback distance cut in half. Proc chance reduced to 20%.
 - Hebabbilys the Ragelord - Max damage and slow mitigation reduced.
 - High Councilman of the Queen - No longer have a chance to softblur every 6 seconds.
 - PoAir - Wave of White Noise now correctly has a 45 second recast.
 - Wind of Xegony is now a magic debuff instead of a curse as it should be.
 - The Rathe Councilmen are no longer immune to CC.
 - Trash in Time P3 is now susceptible to some form of CC or kiting.
 - Rallos Zek's stun reduced to 4sec duration.
 - Quarm is no longer slowable.
 - Vallon Zek no longer FDs his target and instead stuns and swaps targets.
 - Rallos Zek and Innoruuk should no longer be able to be separated from their adds.

Quests
 - Fused Mnemonic of Khati Sha is now completable.
 - Increased stats of Signet of the Arcane
```

---

---

<a name="entry-1352780052215107604"></a>

## 2025-03-21 23:04 - Entry 1352780052215107604
**Author:** Catapultam

Part 1
```
Augmentations
  - Reworked Augment slot schema
   - All Visible Slot (head\arms\chest\legs\feet\wrist) have a Type 21 (Armor Glamour) slot
   - All Weapon\Shield Slot (Pri\Sec\Range) have a Type 20 (Weapon Glamour) slot
   - All items EXCEPT pri\sec\range\charm\ammo have Type 1 slot
   - All items EXCEPT charm\ammo have Type 2 slot
   - All pri\sec\range have Type 2 and Type 4 slots (2 total slots)
   - All 2-handed primary have extra Type 2, Type 4 slots (4 total slots)
  - Removed LORE from Kerafyrm augments
  - All LEGENDARY augments are now ATTUNABLE, and will attune when slotted
  - Renamed all Glamour-Stones to `Glamour - 'Item Name'
  - It is now possible to create augmented items which are both NO TRADE and unusable by you.

Bazaar
 - Purveyor of Glamour will now randomly reward Weapon or Armor Glamours when asked to provide a random Glamour.
 - Purveyor of Glamour will now accept 4 Glamour augments to produce a new random Glamour
 - The 'Prestiege' Bazaar search paramter has been replaced with 'Glamour' and can be used include or exclude those items from search.
 - Vision of Ayonae will reset AAs for 5 EoM (down from 10), and no longer imposes a cooldown.
 - Vision of Ayonae will refund all now-unusable AA when removing a class.

Spells
 - Dispel can now be cast on other players without redirection by implied targeting.
 - Dispel cast by a player on a player or player's pet can no longer remove beneficial effects.
 - Dispel cast by a player on a player or player's pet can no longer remove any effects with counters (poison, disease, curse, etc)
 - Melee damage no longer interrupts casted direct healing spells. (Movement, stun, silence, etc, still can)
 - Calliav line is now instant-cast
 - Removed scaling of Bard rune songs via Heal Amount.
 - Bard rune songs are no longer expended via damage, instead offering a flat damage reduction.
 - All single-target DoT spells and songs have had their cast times reduced to 1 second, the amount removed from their cast time added to recast time.
 - All single-target DoT spells with a base duration greater than 30 seconds have had their durations doubled.
 - All single-target DoT songs have had their duration increased to 1 minute.
 - NEW SPELL: Aspect of the Reptile (DRU 60)

Disciplines
 - Puretone discipline now stacks with all other bard mods
 - Puretone discipline now additionally grants immunity to silence for the duration

AA
 - The following AA always stacks with all other effects: Rabid Bear, Union of Spirits, Ancestral Aid, Guardian of the Forest, Hunter's Fury, Killing Spree, Spirit of the Black Wolf, Spirit of the White Wolf

Pets
 - Substantially reduced direct mitigation bonuses from pet buffs.
 - Added Greater Syncrosatchels for Necromancer, Enchanter, Beastlord; Available from Merchant Aina at level 60
 - Pets are no longer valid targets for NPC Rampage while they have taunt off
 - Sympathetic (Healing) will no longer affect all pets when triggered by a pet-only spell, and will instead behave similarly to sympathetic buffs with other AoE spells (It will hit your current target or implied target when cast).
 - Reworked aggro sharing with pets; pets with taunt off will now give a SMALL amount of aggro to their owner (just enough to get their owner on the mob's aggro list), and a LARGE portion of their aggro to other pets with taunt on.
 - Pets with taunt off and an owner who is feigned or invisible will not transfer aggro in this way, but will temporarily lose the ability to be immune to gaining aggro.
 - Fixed pet caption on Charm
 - MR from Gear and Buffs is no longer considered when checking for charm break
```

---

---

<a name="entry-1349491176792658022"></a>

## 2025-03-12 21:16 - Entry 1349491176792658022
**Author:** Aporia

This is a changelog post to test the new patcher.

```
Words. Changes. Nerfed monks.
```

---

---

<a name="entry-1349425683507708005"></a>

## 2025-03-12 16:55 - Entry 1349425683507708005
**Author:** Catapultam

Hotfix -> Requires new zone zervers to take effect
```
- Fixed pets not correctly calculating spell proc rate
```

---

---

<a name="entry-1349412549308842084"></a>

## 2025-03-12 16:03 - Entry 1349412549308842084
**Author:** Catapultam

```
- Doppelgangers now respect spell recast times of spells they inherit from their owner.
- Swarm pets inherit spell modifiers from their owner even when their owner has no other pets
- Zone State restoration is now improved in such a way as to prevent spawning multiple mobs on zone restore.
```

---

---

<a name="entry-1348875672461901824"></a>

## 2025-03-11 04:30 - Entry 1348875672461901824
**Author:** Catapultam

```
- Re-enabled Zone State Preservation
- Fixed Bazaar Parcel Purchase Discount
- Fixed incorrect mobs spawning in restored respawning instances
- Fixed The Polymorphist not accepting Echo of Memory for deity changes
- Praeserti no longer flee
- Fixed Bladed Song
- Removed Parcel fee for Bazaar purchases in EC and Bazaar
```

(Yes, this changelog is posted again on purpose.)

---

---

<a name="entry-1347823190017052734"></a>

## 2025-03-08 06:48 - Entry 1347823190017052734
**Author:** Catapultam

```
- Re-enabled Zone State Preservation
- Fixed incorrectly calculated stat caps
- Fixed crash that could occur with certain player events (@Neckkola)
- Fixed Class-Specific titles not working
- Fixed Bazaar Parcel Purchase Discount
- Titles are now deduplicated
- Fixed incorrect mobs spawning in restored respawning instances
- Adjusted most Summoned items to not require equipping to cast.
- Fixed The Polymorphist not accepting Echo of Memory for deity changes
- Praeserti no longer flee
- Fixed Bladed Song
```

---

---

<a name="entry-1347615496207466548"></a>

## 2025-03-07 17:02 - Entry 1347615496207466548
**Author:** Catapultam

```
- Updated to EQEmu v23.2
  - Zone State Preservation
    - Zone States are now preserved when the zone is internally shut down or the server is restarted
    - Spawned Mobs (including PH\Named or scripted spawns), Loot, and other zone parameters will be restored after zone shutdown.
    - Some EVENT SCRIPTS may still break if you unload a zone during the event. Please report these as bugs.
  - Fix various crashes (https://github.com/EQEmu/Server/releases)

- Bug Fixes
  - Fixed ATK not being applied properly from items.
  - Pet-only spells should more reliably land on pets.
  - Mobs should no longer summon players under the world.
  - Beneficial DoT (read, Lich) should no longer break rogue sneak/hide

- BREAKING CHANGE
  - Items will now attune IMMEDIATELY upon being equipped. No reimbursement will be given for accidentally attuned items.
  - Items with 'Must Equip' type click effects will ONLY be castable from inventory slots if ATTUNED
  - Explorer Progression Path is now ACCOUNT BOUND. This will reset progress made at the per-character level. Please contact a guide if you require reimbursement.

- Changes
  - Players will become immune to being summoned for 10 seconds after being summoned.
  - Removed Snare and Slow components from shaman Torpor line
  - Moved shaman Torpor line into short-duration buffs
  - Echo of Power should now properly stack with all other buffs
  - Global Buffs should more reliably re-apply.
  - Removed several useless\nonworking AA (Extended Shielding, Trap Navigation)
  - All versions of Dire Charm are now undispellable
  - Fixed an exploit with Parcels
  - Adjusted pet aggro transfer rules.
  - Fixed crash zoning into North Ro
```

---

---

<a name="entry-1347611729353244775"></a>

## 2025-03-07 16:47 - Entry 1347611729353244775
**Author:** Aporia

```
Return Bash now available to Paladins and Warriors and functions similarly to Return Kick

The following items have had their heroic stats and mod2 stats corrected:

Crown of the Defender (Legendary)
Bone Ring of Disharmony (Legendary)
Vial of Suspended Mana (Legendary)
Strands of Power (Legendary)
Bone Collar of the Possessed (Legendary)
Armband of Serenity (Legendary)
Boneweave, Bracer of the Enslaved (Legendary)
Crown of the Undead Warmaster (Legendary)
Earring of Death (Legendary)
Earring of Fond Memories (Legendary)
Gauntlet of the Fire Ring (Legendary)
Gem Encrusted Choker (Legendary)
Seer's Orb of Power (Legendary)
Skull Charm of the Oracle (Legendary)
Totem of the Corpsemaster (Legendary)
Warmaster's Mask of Battle (Legendary)
Bracelet of the Manawielder (Legendary)
Grimling Medallion of Power (Legendary)
Grimling Archmage's Nosering (Legendary)
Medallion of the Hero of Shar Vahl (Legendary)

Avatar of Agony, Avatar of Suffering, Avatar of Pain, and Avatar of Anguish are now the only mobs on their spawn table.

The following items are now no drop:

Screaming Sphere
Quintessence of Elements
Enchanted Ring of Torden
Symbol of Torden
Mark of Torture
Mark of Lashing
Mark of Flame
Mark of Stone
Mark of Suffocation
Mark of Execution
Gryme's Crypt Key
Mound of Living Stone
Globe of Dancing Flame
Sphere of Coalesced Water
Amorphous Cloud of Air
Crystalline Globe
Wind Etched Key

Runic Strike should now stack with Rune

The following explorer progression items have been made all/all so that they can be leveled by any hero:

Mask of Secrets
Sebilite Scale Mask
Helot Skull Helm
Helm of Rile
Stronghorn's Horn
Shackle of Auctoririas
Sword of Pain
Siren Hair Earring
Ring of the Shissar
Shadel Bandit Ring
Zekhas' Katar
Blade of Insanity
Elemental Binder
Djarn's Amethyst Ring
Crown of the Froglok Kings
Scalp of the Ghoul Lord

The explorer progression path for Luclin no longer requires the Unadorned Scepter and now requires a Burning Ring from Umbral Plains.
```

---

---

