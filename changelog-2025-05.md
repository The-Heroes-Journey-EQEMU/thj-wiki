---
title: Changelog - May 2025
description: Changelog entries for May 2025
published: true
date: 2025-06-19T23:04:10.282Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:10.282Z
---

# Changelog - May 2025

[← Back to Recent Updates](/en/Change-log-history) | [← April 2025](/en/changelog-2025-04) | [June 2025 →](/en/changelog-2025-06)

---

*12 updates in May 2025*

<a name="entry-1378090541618823219"></a>

## 2025-05-30 19:19 - Entry 1378090541618823219
**Author:** Catapultam

## Expanded Pet Command Update
* You can now issue commands specifically to **swarm pets** using the `/pet` command!
```
/pet swarm attack       # Swarm pets attack your current target
/pet swarm ghold on     # Swarm pets will GHold
/pet follow             # Regular pets follow (swarm pets unaffected)
/pet swarm attack       # Swarm pets attack (regular pets unaffected)
/pet all swarm hold on  # Both regular AND swarm pets set hold on
```
* Supported Swarm Commands
    * `attack` — Attack your current target
    * `back` — Back off from combat
    * `hold on/off` — Toggle hold
    * `ghold on/off` — Toggle greater hold
    * `focus on/off` — Focus on your target
    * `assist on/off` — Toggle assist mode (**default: on**)
* Set swarm behavior *before* summoning, which will apply to all future swarm pets.
* Pet commands issued from the pet window will now apply to all non-swarm pets.
* `/pet all <commands>` and `/pet <commands>` will not include swarm pets.
* All pet toggle settings now persist between zones and login sessions, and will also automatically apply to future pets of the same class ('swarm' is considered a class).
---
## Passive AA Toggle
* You can now toggle **passive AAs** on or off at will.
```
/alt toggle <aa_id>
```
* Settings persist through zoning and relogging.
* AA descriptions now include their relevant slash command
  * Activatable AAs: `/alt activate <id>`
  * Passive AAs: `/alt toggle <id>`
---
## Out of Combat Casting
* You can cast unmemorized spells while out of combat
```
/cast "Minor Shielding"    # Cast by name (checks gem, then spellbook)
/cast 1543                 # Cast by spell ID (checks gem, then spellbook)
/cast 1                    # Cast from spell gem slot 1 (unchanged)
```
* Always works on **memorized spells**, even in combat
* Intended for out-of-combat buffing, or hotkeys for memorized spells.
---
## Bugfixes
* Players can now say "return" when killing Berserker's Image and looting their Axe of lost Souls to return. (@Eldarian)
* Client updates have been made over the last week to reduce the incidence of crashing when zoning or switching characters.
* Necropotence and Shadow Curse will correctly trigger when mobs are killed in melee.
---
## Encounters
* Zebuxoruk will no longer transition to phase 2 time rewinds and accelerations while any summoned echoes (boss adds) remain alive. Defeat them to disrupt his temporal shield. (@ammordius)
* His rewinds have decreased in effectiveness and each time Zebuxoruk rewinds time, the amount of health he recovers is reduced, stacking. (@ammordius)
---
## Misc
* The Polymorphist in the Bazaar now sends tells instead of using quest::Say. This change was made to avoid players accidentally changing features they didn't intend by clicking say messages while others use the feature. (@ammordius)
* A Marquee message will be displayed when a player attempts to leave the Bazaar with a Trader's Satchel
* Detrimental spells no longer use precision buff timers.
* It is no longer possible to claim a title that you already have.
* Crucible of the Elements is now twice as likely to drop from the Elemental Gods.
* The Elemental Gods can now drop both a crucible and their essence instead of one or the other.

---

---

<a name="entry-1375327656756908104"></a>

## 2025-05-23 04:21 - Entry 1375327656756908104
**Author:** Catapultam

## Hotfix 05-22-2025 1

* Reduced the number of client crashes when zoning or switching characters
* Removed Map Filter window
* Added Map Filter options to main Map window
* Removed particles from Druzzil's Mystical Familiar (@Tacc)

---

---

<a name="entry-1375144061475885087"></a>

## 2025-05-22 16:11 - Entry 1375144061475885087
**Author:** Catapultam

## Enchanter
* Doppelganger casts spells more intelligently
* Doppelganger cannot be affected by Bloodlust or Rage of Rallos Zek
## Druid
* Neverending Swarm / Beeeeees! will no longer affect players.
## Wizard
 * Familiars have returned! Familiars are now tied to their buff and cannot be dismissed without removing the buff.
## Warrior
 * Gut Punch reduced to 25% damage increase
## Shaman
 * Shaman heal over time spells have had their cast times halved and durations doubled.
 * Tnarg's Mending has had it's cast time reduced and base mana cost and effectiveness adjusted.
## General
* Decoupled buff timers from global tick timer. Buffs should always last their full duration in seconds, regardless of where in the tick cycle they were activated.
* Mobs automatically riposted via disciplines are now only attacked back once a combat round. All attacks are still blocked. (@ammordius)
* Properly increased the base damage of all DoT spells.
* Implemented `/castmode [normal/bard/toggle]` switches between normal and bard-style (click gem during casting to interrupt) for non-Bard spells
* Purge Enchantment is no longer unresistable (@Eldarian)
* Mind Crash AA no longer bugs out and has a 5 minute CD when hastened AA is maxed out.
* Vision of Ayonae now automatically uses free class and AA resets if available to you. (@ammordius)
* Proc-On-Kill effects (Necropotence, Killing Spree, etc) can now trigger when your pets kill mobs.
* Fennin Ro will no longer depop if left up for too long.
* Speculative fix for rare issue causing zone crash on death of Seru
## Encounters
* Zebuxoruk on hard and normal difficulty will drop at least two splinters for groups of 3 or more players. (@ammordius)
## Bug Fixes
* Sword of Truth, Reforged - Singing Resonance now works correctly
* Restored all default waypoints for new accounts.
* Fixed issue causing mouse to be unresponsive in some circumstances.
* Trigger-on-DoT tick abilities are no longer triggered on cast of other spells.
## Platform
* Updated to EQEmu 23.7.0

---

---

<a name="entry-1373717024785825935"></a>

## 2025-05-18 17:41 - Entry 1373717024785825935
**Author:** Catapultam

## Known Issues
* Critical Hit messages for autoattack do not account for Heroic Strength scaling
* Beeeeeees! should not affect players.
* Staff of Solusek Ro focus should affect AoE spells like other foci of the same type do.
* Doppelganger is underperforming

---

---

<a name="entry-1373675756659671040"></a>

## 2025-05-18 14:57 - Entry 1373675756659671040
**Author:** Catapultam

## The Magic Map
  * Interact with the Magic Map in the Bazaar or East Commonlands directly.
  * Tearel can still provide group and expedition feature unlocks
## General Combat Changes
  * Autoattack (not Archery) damage is increased by Heroic Strength.
  * Archery now has a minimum amount of damage per successful hit, determined by Heroic Dexterity.
  * Berserker Snares will no longer consume axes (@Eldarian)
  * Pets now obey the Spell Damage\Heal Amount cap
## General Spell Changes
  * Damage Over Time
    * Dramatically increased the effectiveness of Burning Affliction type spell focuses
    * Dramatically increased the base damage of most DoT spells
    * Sympathetic Strike I-X no longer triggers on DoT spells
    * Reworked DoT damage calculations to fix several bugs with Critical DoT tics being overly intense.
  * Slow, Mez, and Charm immunity is now reported when a mob is considered.
## Wizard
  * Reduced Elemental Familiar damage bonus.
## Necromancer
 * Cascade of Decay can now trigger on DoT tics, and is a Lifetap.
 * Lifeburn adjusted -> Instantly consume 40% of your maximum HP to inflict a powerful DoT spell on your opponent. Blocked by and Blocks Mana Burn.
 * New AA: Necropotence
   * Requires Rank 6 Army of the Dead
   * Passively create undead minions as you kill your enemies.
## Shadowknight
  * New AA: Shadow Curse
    * Requires Rank 6 Touch of the Cursed
    * Passively create undead minions as you kill your enemies.
## Enchanter
 * Doppelganger pets no longer gain access to spellcasting stats provided by their owner's buffs.
 * Doppelganger pets spellcasting priority adjusted to cast more of their spells instead of preferring the lowest spell gem not on cooldown
 * Doppelganger pets now use combat skills (Kick, Bash, etc) from your classes.
## Shaman
  * New AA: Shamanic Curse
    * Sympathetic Proc which can trigger on DoT tics
    * Single-Target DoT which also applies a direct increase to attack delay (not *slow*)
## Druid
  * New AA: Beeeees!
    * Sympathetic Proc which can trigger on DoT tics
    * Area Effect DoT which also increases spell damage taken
## Encounters
 * Nitram Anizok will respawn if killed during his event. (@ammordius)
 * Debuffs cast by the Thought Horror Overfiend have been given a 30s recast timer.
## Items
* Substantially improved the items rewarded from Vortex of the Past
* Removed 'No Drop' from items rewarded by Vortex of the Past
## Bug Fix
* Fixed Theft of Life AA no longer affects heal spells.
* Fixed error related to Mez, Silence, and Charm in debuff logic (This might be what is randomly killing pets) (@Zimp)
* Certain messages related to Ranged Attack Mode are now rate-limited.
* It is now possible to sort the tracking window.
* Fixed movement casting with Dimensional Shield.
* Fixed zone crash around Behemoth event in PoI (@zimp)
* Gram Dunnar will now craft figurines for you for your new classes (@ammordius)
* Fixes to Brianna Falsrinay quest
* Initiate Symbol of Brell should now be completable
* Non-Bard Song spells can no longer be interrupted by Bards by spam-clicking the spell gem.
* Critical Hit messages for Melee, Skills, and Ranged attacks should now more accurately report the correct damage value
* NPCs are removed from hatelists more consistently on depop and despawn. (@ammordius)
* Fixed serveral bugs related to Extended Target (@ammordius)
* Different ranks of Cryomancy and Pyromancy no longer stack.
* The Goblin King in Runnyeye can no longer double spawn.
* Fixed over a dozen quests in Classic which could not be completed due to script errors.
## Misc
* Many broken Glamours have been removed from the game and replaced with Token of Shifting Glamour, which can be turned into the Purveyor of Glamour for a new random glamour.
## Platform
  * Updated to [EQEmu 23.6.0](https://github.com/EQEmu/Server/releases/tag/v23.6.0)

---

---

<a name="entry-1370146880595693650"></a>

## 2025-05-08 21:14 - Entry 1370146880595693650
**Author:** Catapultam

# Balance Adjustments
* Improved Damage I, II, and III have been reduced in effectiveness.
# Misc
 * `/camp` is now instant only in the Bazaar and East Commons while out of combat.
 * Cleaned up instant-camp to not show disconnected screen and more rapidly return to character select.
 * Improved Crash Handler
 * Updated Lore Description on XL Combinerator
# Bug Fixes
 * Corrected zone crash related to pet assist mode.
 * Corrected zone crash related to Mana Burn.
 * Corrected zone crash related to Lord Inquisitor Seru encounter.
 * Restored group scaling on Zebuxoruk encounter
 * Fixed issue where Sympathetic Strike focus effects could trigger each other
 * Revisions to Druzzil Ro event (@ammordius)
 * Revisions to Herald of Druzzil Ro event (@ammordius)
 * Fixes to Relv the Mysterious event (@Eldarian)

---

---

<a name="entry-1369886137379983400"></a>

## 2025-05-08 03:58 - Entry 1369886137379983400
**Author:** Catapultam

# Hotfix

## Misc
 * Camp timer is skipped when out of combat (OOC Regen active), allowing for instant camp instead
 * Updated Lore Description on XL Combinerator
## Bug Fixes
 * Revisions to Druzzil Ro event (@ammordius)
 * Revisions to Herald of Druzzil Ro event (@ammordius)
 * Fixes to Relv the Mysterious event (@Eldarian)

---

---

<a name="entry-1369707907456831498"></a>

## 2025-05-07 16:10 - Entry 1369707907456831498
**Author:** Catapultam

# Hotfix

* Reverted 'Songs with a 3 second base cast time have been lowered to 2.5 seconds.'
* Reverted 'Bard songs are no longer affected by any spell focuses.'
* Bard songs can no longer be affected by Improved Damage type focuses, but can be affected by other spell focuses.

---

---

<a name="entry-1369700491662987505"></a>

## 2025-05-07 15:40 - Entry 1369700491662987505
**Author:** Catapultam

[This patch has a theme song.](https://www.youtube.com/watch?v=Yps9mkxnHS8)

---

---

<a name="entry-1369699960169435266"></a>

## 2025-05-07 15:38 - Entry 1369699960169435266
**Author:** Catapultam

# Pets
 * Pets with taunt off ACTUALLY, REALLY, FOR REAL are ignored by Rampage
 * Corrected Literally Unplayable typo in `/pet health` output
 * `/pet health` aliases added -> `/pet stats` `/pet inventory` etc
 * Added `/pet assist` command (on\off toggle available). When this mode is enabled, pet will follow owner's autoattack & damaging spell targets, as well as automatically assist any pet with `taunt on` if the assisting pet has `taunt off`
 * Added popup stats window to `/pet health` output
 * Added chat inventory output to `/pet health`
 * Added support for some multi-word pet commands; notably `/pet get lost`
 * Pet taunt and aggro generation revised.
   * Pet taunt always succeeds to put them at the top of hate list (with a smaller buffer than players get from the Taunt skill, which can fail)
   * Pets with`taunt on` inherit ALL of their owner's aggro (before aggro-reduction modifiers), and having a pet in this state reduces their owner's aggro by 50%.
   * Net result is that solo players will not take aggro from mobs as long as their tank pet is alive, and grouped players will not have perfect aggro on their tank pet (but can generate enough aggro cumulative with the tank pet to make pet tanking in groups viable)
 * Pet Illusions survive zoning
 * Petamorph wands can target individual pets.
# Tradeskills
 * There is now a higher minimum chance to skill-up when performing a tradeskill combine.

---

---

<a name="entry-1369699915567071363"></a>

## 2025-05-07 15:38 - Entry 1369699915567071363
**Author:** Catapultam

# Encounters
 * Time Vortex in Plane of Time no longer proc Time Warp, but instead cast it on a 30 second cooldown.
 * The disease counters on Time Warp have been reduced to 30.
 * Reworked Zebuxoruk encounter - Druzzil Ro can assist the player by reducing the difficulty of the encounter in exchange for reduced loot awards
 * Kerafyrm, Lord Inquisitor Seru, and Zebuxoruk will offer additional loot for those who challenge them as a group (3 or more players).
 * Reduced the difficulty of certain mechanics in the Zebuxoruk encounter.
 * Plane of Time reworked; a Herald of Druzzil Ro will guide you through the initial parts of the zone. The Herald will also accept a Time Phased Quintessence in order to allow you to skip Phases 1-3 of the zone.
 * Lowered the time between waves for several ring events in Acrylia Caverns
# Paladin
 * Adjusted Act of Valor to consume 50% of Max Mana in order to heal group for 2 hp per mp consumed
# Warrior
 * Warlord's Fury AA added
   * 1 minute CD. 100% All Skill Damage for up to 12 seconds.
 * Press the Attack adjusted - now causes initial damage and reduces target's AC for up to 12 seconds.
 * Grappling Strike adjusted - now causes initial damage and reduces target's evasion for up to 12 seconds.
 * Gut Punch adjusted - now causes initial damage and increases target's physical hit damage taken by 50% for up to 12 seconds
# Wizard
* Harvest of Druzzil restores 40% of user's maximum mana when activated.
* Cryomancy and Pyromancy AA effects will stack with all buffs.
* Cryomancy and Pyromancy have had their proc chance increased to 35%.
* Pyromancy now does initial damage like Cryomancy in addition to a DoT
* Cryomancy now has additional DoT damage like Pyromancy in addition to initial damage
* Pyromancy DoT now leaves a massive -Cold Resist debuff
* Cryomancy DoT now leaves a massive -Fire Resist debuff
* Added Dimensional Shielding AA
  *  While active, the Wizard will be immune to spellcasting interruption
* Mana Burn\Blast\Blaze & Volatile Mana Blaze rebalanced
  * Consumes 10/20/30/40% of the player's total mana pool and converts it instantly to damage.
  * Mana Burn\Blast\Blaze\VMB no longer consumes mana or triggers a cooldown when used on a target which cannot be Mana Burned again yet.
  * With full Hastened Mana Burn AA, Reuse on all four abilities 15 minutes.
# Magician
 * Increased Fire Focus on Heart of Flames to 100%
 * Increased Fire Focus on Fire Core to 150%
# Bard
 * Scaled up DD Focus songs to 10x (still randomized)
 * Songs with a 3 second base cast time have been lowered to 2.5 seconds.
# Shaman
* Languid Bite AA effect will stack with all buffs.
* Rabid bear now gives 15/20/25% hundred hands effect instead of haste
* Spirit of the Leopard now lasts for 3 minutes and is no longer a short duration buff.
# Beastlord
 * Bestial Alignment AA effect will stack with all buffs.
 * Blood Frenzy corrected.
# Cleric
* Divine Avatar AA effect will stack with all buffs. (Stacking limits to certain effects apply)

---

---

<a name="entry-1369699861905277003"></a>

## 2025-05-07 15:38 - Entry 1369699861905277003
**Author:** Catapultam

# General Changes
* Most Focus Effect types which previously had a randomized effect now have a static effectiveness.
* Improved Damage Focus increased in effectiveness by 1000%.
* Many Improved Damage Focus will now be effective on AoE spells.
# Automated IP Exemptions!
* Two Gnomish Causality Engineers have appeared in the Bazaar! These will help you obtain an IP exemption if you follow their quest.
  * This system relies on our trust in our players to not abuse this system.
  * Players found to be abusing this system to multibox outside of the Bazaar will have consequences for every account which they have ever logged into.
# Bug Fixes
 * Corrected bug which caused abnormally accelerated attack rates when using `/attackmode ranged`
 * Players with certain titles should no longer crash when opening title window
 * Updated a number of augments (including Easter Eggs) to correctly be attunable at the Legendary quality level
 * Speculative fix for crash at 0% in certain encounters
 * Added validation to make sure that items you buy from vendors is actually the item you are trying to buy.
 * Vision of Ayonae dialogue text revised.
 * Maligar in West Karana should more reliabily path back to his spawn
 * Updated ALL legendary augments (including Easter Egg augments) to be attunable.
 * Augments with Focus Effects containing Sympathetic Procs can now function if the host item already has a focus effect
 * Battle Cry of the Mastruq now correctly decreases weapon delay instead of increasing it.
 * Tracker Azeal will no longer be spawning multiable copies of himself (@Eldarian)
 * Added Relv the Mysterious encounter in Plane of Storms (@Eldarian)
 * Jaggedpine War Event Villagers will no longer Duplicate spawn themselves during the event (@Eldarian)
 * Rabbit Petamorph wands now make rabbits instead of Dougs
 * Petamorph wand illusions are now permanent
 * Fixed mismatch between displayed cast times and actual cast times for certain spells.
 * Dain is no longer a Doug
 * Jaled Dar's Shade is no longer a Doug
 * Bard songs are no longer affected by any spell focuses.
# Misc
 * Certain Merchants who have items with criteria which hide that item (such as class or level), no longer have a temporary merchant list. Notably, this affects Merchant Aina in the Bazaar
 * Removed slow effect from Prismatic Entropy.
 * Added 'Train All' toggle to AA Window (@voidless)
 * Added 'Map Filters' option window to Map Window (@voidless)
 * Vision of Ayonae's class randomization feature now randomizes all 3 classes.
 * Added XL Gnomish Quadramorphic Combinerator. Combine up to 16 items in any combination of Base and Enchanted to create a Legendary item.
 * Name Changes are now available from the Polymorphist in the Bazaar.
 * Removed Delivery Voucher from all merchants in the Bazaar
 * Added Bundle of Delivery Vouchers (10) to Echo of Memory in the Bazaar. This will unpack into 10 Delivery Vouchers when purchased.
   * Reminder: Delivery Vouchers can be used to purchase items from traders in the Bazaar from any zone with no additional fees, and have that item delivered directly to your inventory.
* Druid and Ranger epic 1.0 quest NPCs in East Karana will now only accept talisman turn-ins in the correct sequence and will reject out of sequence items if the quest is already in progress. Althele will accept any of the quest talismans to restart the line. (@ammordius)
* Commander Zazuzh and Commander Zherozsh in Ssra Temple are now guaranteed to be up in a non-respawning instance with their key piece.
* Box of the Void is now Lore
* Tome Vendors in EC Tunnel are now all labeled correctly
* Added Echo of the Past to numerous zones involved in Epic Quests, all Epics should now have DZ options for all contested stages.
* Reduced AoE Range of Chronostorm
* Spell Casting Subtlety removed.
* Silent Casting has been made available to all casting classes, the recast time reduced to 60 seeconds, and the duration increased to 1 hour (and the buff will now suspend).

---

---

