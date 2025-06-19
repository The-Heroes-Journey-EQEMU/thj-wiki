---
title: Changelog - June 2025
description: Changelog entries for June 2025
published: true
date: 2025-06-19T23:04:06.267Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:06.267Z
---

# Changelog - June 2025

[← Back to Recent Updates](/en/Change-log-history) | [← May 2025](/en/changelog-2025-05) | 

---

*5 updates in June 2025*

<a name="entry-1385309046139256943"></a>

## 2025-06-19 17:23 - Entry 1385309046139256943
**Author:** Catapultam

## Jun 19 - Hotfix
### Bugfixes
* Increased proc rate of most Proc-On-Kill AAs

---

---

<a name="entry-1384236759839408208"></a>

## 2025-06-16 18:22 - Entry 1384236759839408208
**Author:** Catapultam

## June 16
### Bugfixes
  * Fixed a number of issues causing client crashes.
  * Dispelled (Suspended) buffs returning to pets should no longer cause server + client crash.
  * Low-level bow damage has been normalized back to correct values.
  * High-level DoT damage has been restored to correct values.
  * Fixed issue with on-kill procs triggering at a lower than expected rate.
  * Removed a number of broken Glamour items from the game.
### Pets
  * Pets will limit their attempts to assist and retarget to once a second.
### Play Modes Prep
  * Jeweler Imua has also contracted out some work to a helpful gnome and a kind shaman, and can also make a Philter of Major Translocation and some select tinkering goods he's heard might be in demand.

---

---

<a name="entry-1383200966580371556"></a>

## 2025-06-13 21:46 - Entry 1383200966580371556
**Author:** Catapultam

## Jun 13
* Speculative fix for client crashes.

---

---

<a name="entry-1382858174951985194"></a>

## 2025-06-12 23:04 - Entry 1382858174951985194
**Author:** Catapultam

## Bugfixes
* Wake The Dead style abilities (WTD, Army of the Dead, Necropotence, Shadow Curse) no longer create pets which can cast Fear, Gate, Shadowstep, Charm, and other problematic spell types.
* Necropotence and Shadow Curse now create pets based exclusively on the corpse of the mob that triggered them.
* All Glamour weapons are now Primary\Secondary
* All Glamour Bows\Throwing are now Ranged only
* All Glamour Shields & Misc are Secondary only
* Familiar buffs now correctly stack with other spells. (Notably, Zombie Bunny & HP buffs). This does not affect if Focus effects stack, but the buff itself will stick.
* Spell Gem #1 is no longer disabled when using `/cast`
* An Undead Knight in the Temple of Sol Ro now appropriately responds to expected quest text. ( @MWadstein)
* Guardian of the Forest will no longer be a permanent buff duration at rank 1.
* Rev The Mysterious will now allow other Hero's to Join in on the encounter without delay.
* A goblin captain should now drop the quest item required to complete the Treant Fists quest.
* Corrected various loading screen typos, and updated for newer changes.
* Adjusted dialog for reaching the 7th Hammer
* Staff of the Wheel quest piece in high pass will no  longer spawn out of bounds.
* Precision timers now correctly fade buffs on their tooltip specified times. Optimized communication of buff timer remaining sent to client, so buffs timer on client matches server with precision timer.
* Fixed quest ground spawns in Kithicor Forest to no longer be out of reach of players.
* Bonus loot credit is no longer tracked for Seru when players do not actually engage with his encounter, and exploit certain mechanics to have him start a lower hp total.
* Mobs should now more reliably choose to path home when they lose their way.
* Fixed incorrect damage calculation for bow damage at certain level breakpoints.
* Barter/Buyer should now correctly work across zone shards

---

---

<a name="entry-1382858107209777174"></a>

## 2025-06-12 23:04 - Entry 1382858107209777174
**Author:** Catapultam

## June 12
### New Feature - Character Select Overhaul
* Use your Character Slots to create more than 12 characters!
* Organize those characters into Character Sets!
* 24 Character Slots and 2 Sets initially available.
* Up to 12 additional Slots and 3 additional Sets are available via EOM unlocks.
* Additional Slots and Sets will become available in the future as gameplay & event rewards.
### New Feature - Dispel Suppression
* Buffs are now 'Suppressed' for 36s instead of removed when Dispelled.
* Suppressed buffs return when the suppression expires, but cannot be recast until then.
### Combat
* Heroic Strength contribution to autoattack damage now has diminishing returns over 100.
* Heroic Dexterity now directly scales bow damage.
* Spell Effects not cast from spell gems no longer can incorrectly inherit the Heroic Intelligence or Wisdom bonus because you were casting a spell from a spell gem when the effect occurred.
* Spell Effects from AA abilities (not procs or combat skills) now receive Heroic Intelligence or Wisdom bonuses.
* The "darkness" line of dot / snare debuffs for Shadow Knights and Necromancers will now still apply their dot if the target is immune to movement speed changes.
* Debuffs on Non-Pet NPCS are now tracked with 'Precision timers', so that their full duration is applied regardless of tic timing.
### Warrior
* Rage of Rallos Zek now has a fixed duration of exactly 12 seconds, and is unaffected by either buff extension effects or server tic timing.
### Beastlord
* Bloodlust now has a fixed duration of exactly 24 seconds, and is unaffected by either buff extension effects or server tic timing
### Necromancer
*  Necromancers now have access to inherent DoT critical chance, similar to Wizard's ability to inherently crit DDs. This chance is a seperate roll for crit if the primary crit roll fails, and is not affected by any other source of crit chance.
### Wizard
* Wizard inherent critical spells now use the player's critical damage instead of a lower randomized value. They also now print a message critical informing the player their Wizard ability triggered.
### Ranger
* Archery minimum damage increased.
### Bard
* Bard DoT song damage increased.
### Rogue
* The Sneak Attack line (Sneak Attack, Thief's Vengeance, Assassin's Strike, Kyv Strike) is now usable during other disciplines, and provide a 12-second buff with their original effect rather than a discipline lockout.,
* Backstab will now use either your primary or your secondary weapon, whichever will produce the more damaging Backstab.
* The Sneak Attack line now has a fixed duration and is no longer extendable.
### UI
* Map Filter is no longer it's own unique window, rather integrates into the existing Map Window.
### Misc
* Jeweler Imua in the Bazaar has been practicing his enchanting and can make you an enchanted platinum bar for a modest fee.
* Burrower Event Spawn timers have been reduced
* A number of NPCs in FV have had their dialogue fixed and accept multiple spell swap turn ins simultaneously

---

---

