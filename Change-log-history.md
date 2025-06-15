---
title: Change Logs
description: 
published: true
date: 2025-06-15T22:17:14.102Z
tags: change-logs, change, logs, patchnotes, patch, notes, patch-notes, patches
editor: markdown
dateCreated: 2025-06-15T20:03:58.450Z
---

![change-logs.webp](/change-logs.webp){.align-center}
# THJ Change-Logs
(Newest is up top, Oldest is at the bottom.)

## 2025-06-13 21:46 - Entry 1383200966580371556
**Author:** Catapultam

## Jun 13
* Speculative fix for client crashes.

---

---

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
* An Undead Knight in the Temple of Sol Ro now appropriately responds to expected quest text.
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
* Players can now say "return" when killing Berserker's Image and looting their Axe of lost Souls to return.
* Client updates have been made over the last week to reduce the incidence of crashing when zoning or switching characters.
* Necropotence and Shadow Curse will correctly trigger when mobs are killed in melee.
---
## Encounters
* Zebuxoruk will no longer transition to phase 2 time rewinds and accelerations while any summoned echoes (boss adds) remain alive. Defeat them to disrupt his temporal shield.
* His rewinds have decreased in effectiveness and each time Zebuxoruk rewinds time, the amount of health he recovers is reduced, stacking.
---
## Misc
* The Polymorphist in the Bazaar now sends tells instead of using quest::Say. This change was made to avoid players accidentally changing features they didn't intend by clicking say messages while others use the feature.
* A Marquee message will be displayed when a player attempts to leave the Bazaar with a Trader's Satchel
* Detrimental spells no longer use precision buff timers.
* It is no longer possible to claim a title that you already have.
* Crucible of the Elements is now twice as likely to drop from the Elemental Gods.
* The Elemental Gods can now drop both a crucible and their essence instead of one or the other.

---

---

## 2025-05-23 04:21 - Entry 1375327656756908104
**Author:** Catapultam

## Hotfix 05-22-2025 1

* Reduced the number of client crashes when zoning or switching characters
* Removed Map Filter window
* Added Map Filter options to main Map window
* Removed particles from Druzzil's Mystical Familiar

---

---

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
* Mobs automatically riposted via disciplines are now only attacked back once a combat round. All attacks are still blocked.
* Properly increased the base damage of all DoT spells.
* Implemented `/castmode [normal/bard/toggle]` switches between normal and bard-style (click gem during casting to interrupt) for non-Bard spells
* Purge Enchantment is no longer unresistable
* Mind Crash AA no longer bugs out and has a 5 minute CD when hastened AA is maxed out.
* Vision of Ayonae now automatically uses free class and AA resets if available to you.
* Proc-On-Kill effects (Necropotence, Killing Spree, etc) can now trigger when your pets kill mobs.
* Fennin Ro will no longer depop if left up for too long.
* Speculative fix for rare issue causing zone crash on death of Seru
## Encounters
* Zebuxoruk on hard and normal difficulty will drop at least two splinters for groups of 3 or more players.
## Bug Fixes
* Sword of Truth, Reforged - Singing Resonance now works correctly
* Restored all default waypoints for new accounts.
* Fixed issue causing mouse to be unresponsive in some circumstances.
* Trigger-on-DoT tick abilities are no longer triggered on cast of other spells.
## Platform
* Updated to EQEmu 23.7.0

---

---

## 2025-05-18 17:41 - Entry 1373717024785825935
**Author:** Catapultam

## Known Issues
* Critical Hit messages for autoattack do not account for Heroic Strength scaling
* Beeeeeees! should not affect players.
* Staff of Solusek Ro focus should affect AoE spells like other foci of the same type do.
* Doppelganger is underperforming

---

---

## 2025-05-18 14:57 - Entry 1373675756659671040
**Author:** Catapultam

## The Magic Map
  * Interact with the Magic Map in the Bazaar or East Commonlands directly.
  * Tearel can still provide group and expedition feature unlocks
## General Combat Changes
  * Autoattack (not Archery) damage is increased by Heroic Strength.
  * Archery now has a minimum amount of damage per successful hit, determined by Heroic Dexterity.
  * Berserker Snares will no longer consume axes
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
 * Nitram Anizok will respawn if killed during his event.
 * Debuffs cast by the Thought Horror Overfiend have been given a 30s recast timer.
## Items
* Substantially improved the items rewarded from Vortex of the Past
* Removed 'No Drop' from items rewarded by Vortex of the Past
## Bug Fix
* Fixed Theft of Life AA no longer affects heal spells.
* Fixed error related to Mez, Silence, and Charm in debuff logic (This might be what is randomly killing pets)
* Certain messages related to Ranged Attack Mode are now rate-limited.
* It is now possible to sort the tracking window.
* Fixed movement casting with Dimensional Shield.
* Fixed zone crash around Behemoth event in PoI
* Gram Dunnar will now craft figurines for you for your new classes
* Fixes to Brianna Falsrinay quest
* Initiate Symbol of Brell should now be completable
* Non-Bard Song spells can no longer be interrupted by Bards by spam-clicking the spell gem.
* Critical Hit messages for Melee, Skills, and Ranged attacks should now more accurately report the correct damage value
* NPCs are removed from hatelists more consistently on depop and despawn.
* Fixed serveral bugs related to Extended Target
* Different ranks of Cryomancy and Pyromancy no longer stack.
* The Goblin King in Runnyeye can no longer double spawn.
* Fixed over a dozen quests in Classic which could not be completed due to script errors.
## Misc
* Many broken Glamours have been removed from the game and replaced with Token of Shifting Glamour, which can be turned into the Purveyor of Glamour for a new random glamour.
## Platform
  * Updated to [EQEmu 23.6.0](https://github.com/EQEmu/Server/releases/tag/v23.6.0)

---

---

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
 * Revisions to Druzzil Ro event
 * Revisions to Herald of Druzzil Ro event
 * Fixes to Relv the Mysterious event

---

---

## 2025-05-08 03:58 - Entry 1369886137379983400
**Author:** Catapultam

# Hotfix

## Misc
 * Camp timer is skipped when out of combat (OOC Regen active), allowing for instant camp instead
 * Updated Lore Description on XL Combinerator
## Bug Fixes
 * Revisions to Druzzil Ro event
 * Revisions to Herald of Druzzil Ro event
 * Fixes to Relv the Mysterious event

---

---

## 2025-05-07 16:10 - Entry 1369707907456831498
**Author:** Catapultam

# Hotfix

* Reverted 'Songs with a 3 second base cast time have been lowered to 2.5 seconds.'
* Reverted 'Bard songs are no longer affected by any spell focuses.'
* Bard songs can no longer be affected by Improved Damage type focuses, but can be affected by other spell focuses.

---

---

## 2025-05-07 15:40 - Entry 1369700491662987505
**Author:** Catapultam

[This patch has a theme song.](https://www.youtube.com/watch?v=Yps9mkxnHS8)

---

---

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
 * Tracker Azeal will no longer be spawning multiable copies of himself
 * Added Relv the Mysterious encounter in Plane of Storms
 * Jaggedpine War Event Villagers will no longer Duplicate spawn themselves during the event
 * Rabbit Petamorph wands now make rabbits instead of Dougs
 * Petamorph wand illusions are now permanent
 * Fixed mismatch between displayed cast times and actual cast times for certain spells.
 * Dain is no longer a Doug
 * Jaled Dar's Shade is no longer a Doug
 * Bard songs are no longer affected by any spell focuses.
# Misc
 * Certain Merchants who have items with criteria which hide that item (such as class or level), no longer have a temporary merchant list. Notably, this affects Merchant Aina in the Bazaar
 * Removed slow effect from Prismatic Entropy.
 * Added 'Train All' toggle to AA Window
 * Added 'Map Filters' option window to Map Window
 * Vision of Ayonae's class randomization feature now randomizes all 3 classes.
 * Added XL Gnomish Quadramorphic Combinerator. Combine up to 16 items in any combination of Base and Enchanted to create a Legendary item.
 * Name Changes are now available from the Polymorphist in the Bazaar.
 * Removed Delivery Voucher from all merchants in the Bazaar
 * Added Bundle of Delivery Vouchers (10) to Echo of Memory in the Bazaar. This will unpack into 10 Delivery Vouchers when purchased.
   * Reminder: Delivery Vouchers can be used to purchase items from traders in the Bazaar from any zone with no additional fees, and have that item delivered directly to your inventory.
* Druid and Ranger epic 1.0 quest NPCs in East Karana will now only accept talisman turn-ins in the correct sequence and will reject out of sequence items if the quest is already in progress. Althele will accept any of the quest talismans to restart the line.
* Commander Zazuzh and Commander Zherozsh in Ssra Temple are now guaranteed to be up in a non-respawning instance with their key piece.
* Box of the Void is now Lore
* Tome Vendors in EC Tunnel are now all labeled correctly
* Added Echo of the Past to numerous zones involved in Epic Quests, all Epics should now have DZ options for all contested stages.
* Reduced AoE Range of Chronostorm
* Spell Casting Subtlety removed.
* Silent Casting has been made available to all casting classes, the recast time reduced to 60 seeconds, and the duration increased to 1 hour (and the buff will now suspend).

---

---

## 2025-04-20 13:01 - Entry 1363499720273821706
**Author:** Catapultam

## **Spring Event: Easter 2025**
- Easter Eggs may now be discovered throughout the world in various places.
- Will you open them as you find them, or improve their quality first?
- Additional rewards will be granted at the conclusion of the event based on player participation and interaction.

## **Alternate Advancement**
- **Bazaar and Back** AA moved to the **Special** tab.
- **Consume Item** AA moved to the **Special** tab.
- **Consume Experience** AA added:
  - Costs 100 AA to purchase (one-time cost).
  - When activated, consumes unspent AA to progress any equipped Power Source item.
- **Alternately Advanced Firework** AA added for all players. Set your AA ablaze for fun.

## **General Fixes**
- The following buffs are no longer dispellable:
  - Bloodlust
  - Improved Twincast
  - Frenzied Devastation
  - Prolonged Destruction
- Fixed miscellaneous Z-axis spawn issues.
- Resolved Cleric and Paladin spell quest issues in Gunthak.
- Fixed miscellaneous Out of Era (OoE) drop issues.
- Added **Lady Inquisitor** title as counterpart to **Lord Inquisitor**.
- Loot should no longer be removed from mobs on zone shutdown.
- Swarm pets spawned by weapons wielded by pets should now correctly attack.

## **Class Balance Changes**
### **Berserker**
- **Reckless Discipline** cooldown reduced to 30 minutes.
- Improved **Critical Hit** rate calculation for **Devastating Frenzy**.

### **Cleric**
- **Yaulp V+** no longer fades when sitting.

### **Bard**
- **Denon’s Desperate Dirge** base damage and formula adjusted. Still strong for AoE, no longer optimal for single-target.
- Bard songs can no longer be twincast.

### **Druid**
- Now has access to the **Healing Boon** AA.
- **Nature’s Blessing** increased mana cost reduced to 50%.

### **Ranger**
- **Hastened Weapon Shield** is now available. Max rank reduces cooldown to 30 minutes.
- **Burning Arrow** and **Flaming Arrow** now have a 0.5-second cast time.

### **Rogue**
- **Assassin’s Strike** endurance cost reduced to 400 (from 515).
- **Counterattack Discipline** cooldown reduced to 30 minutes.

### **ShadowKnight**
- **Leechcurse Discipline** cooldown reduced to 30 minutes. Duration increased to 5 ticks (from 4).
- **Harmtouch RK XIV** now lasts 12 ticks.

### **Shaman**
- **Spiritual Blessing** increased mana cost reduced to 50%.
- **Spirit of the Leopard** now drops from Emperor Ssra and is usable at level 60. Grants 200% proc rate mod.
- **Rabid Bear** now correctly increases STR and DEX caps.
- **Ancestral Guard** cooldown reduced by 100 seconds per rank and now lasts full duration (no longer caps at 5,000 damage).

### **Warrior**
- **Hastened Furious Discipline** is now available. Max rank reduces cooldown to 30 minutes.

### **Wizard**
- **Mana Burn / Blast / Blaze**:
  - Base cooldown reduced to 66 minutes (from 72).
  - New **Hastened** AA reduces cooldown by 6 minutes per rank.
- **Mind Crash** cooldown reduced to 10 minutes.
- **Strong Root** break chance reduced to 10% at max rank.
- **Hastened Root** brings **Strong Root** cooldown to 2 minutes at max rank.

## **Encounter Adjustments**
- **Inquisitor Lord Seru** stun duration reduced to 7.5 seconds (from 20).
- **Zebuxoruk** minimum damage reduced.
- Zeb's adds now deal reduced minimum damage.

## **Item Adjustments**
- **Prismatic Scale of the Elements (Legendary)**:
  - Augment stats adjusted.
  - **Prismatic Dominance** proc rate increased to 100% (from 10%).
- Luclin and Velious **Ancient** spells renamed to `Spell: Ancient: <name>` to allow right-click scribing.
- Alternate Currency items can no longer be sold to vendors.
- Added over **5,500** new weapon glamours. These are new items; not all have unique graphics.

---

---

## 2025-04-15 03:56 - Entry 1361550724663873648
**Author:** Catapultam

## Changelog April 14 2025

## **Auto Idle and Auto-AFK Updates**

The **Idle** and **AFK** systems have been separated to improve player experience and reduce unnecessary network load.

- In non-combat, players become idle after 1 minute and AFK after 10 minutes.
- In combat, players become idle after 10 minutes and AFK after 30 minutes.

### Key Changes:
- **Idle** now reduces client position updates to improve performance in crowded zones like the Bazaar.
- **AFK** is now fully independent of idle and manual `/afk`. Automatic AFK will not override or be overridden by manual AFK status.
- Manual `/afk` remains active until toggled off and is unaffected by automatic behavior.
- Automatic AFK messages no longer interfere with manual or automatic AFK or idle states.
- The following actions now reset idle and AFK timers:
  - Moving items
  - Casting spells
  - Using `/autoattack`
  - Receiving messages
- **Trade** (start or finish) now forces a position sync for both parties.
- **Wearchange packets** (e.g., armor appearance updates) are now sent even while idle.
- **Buyers** and **Traders** are excluded from automatic AFK entirely.

---

## 💰 **Alternate Currency Improvements**

- **Alternate currency** is now account-wide.
- Currency counts now automatically refresh when:
  - Reclaiming items
  - Creating currency
  - Updating currency values
- The **Reclaim** button now functions correctly with currency items on the cursor.

---

## 🐞 Fixes & Improvements

- Fixed integer underflow on 0-value runes.
- Fixed **Frenzy** so it can now critically hit as intended.
- Fixed **weapon glamours** not appearing on pets.
- Resolved various issues with glamours, illusions, and idle logic in the Bazaar.
- Pets summoned by **Doppelgangers** now correctly belong to their summoner’s owner.
- Fixed a bug where pets could become permanently detached from their owner.
- Fixed bug causing pet aggro to clear whenever taunt command was set, regardless of setting.
- Fixed a bug preventing pets with taunt off from properly gaining the 'Immune to NPC Aggro' flag
- Fixed a bug which caused pets to taunt enemies attacking their owner at unlimited range.

---

---

---

## 2025-04-09 17:46 - Entry 1359585216825655307
**Author:** Catapultam

**Auto AFK**

**Why this Change?** Part of what we see in a critical hub zone such as Bazaar, is extremely high CPU, lag, causing a bad experience for other players trying to zone into the zone and function at all. This change aims to drastically reduce packet spam in the zone, keeping the zone lean and leading to a much better player experience when using the Bazaar. When a player with 4 pets is running in circles in the zone, it sends enormous amounts of position updates to X number of players in the zone, even those who are idle and don't need all of these updates.

When clients go AFK they stop receiving packet updates for movement. When they go un-AFK they get synchronized with all the clients around them.

**Changes**

* When in a non-combat zone (Bazaar) - auto AFK timer is 60 seconds
* When in a combat zone - auto AFK timer is 10 minutes
* When you go AFK, we also toggle the native /afk flag on the client now
* When a client initiates a trade with another client, both clients in the trade get auto-marked as non-AFK
* When a client finishes a trade with another client, both clients in the trade get auto-marked as non-AFK
* Heading now takes part in triggering when a client "moved" to remove them from auto AFK status
* Client messaging is now simply "You are AFK." / "You are no longer AFK."

```
- Fixed an issue where spawn locations weren't being restored properly after zone state restoration.
- Fixed an issue where restoring an in-progress Plane of Time B instance would sometimes not restore properly.
- Fixed a scenario where sometimes players would not be able to enter certain open world zones while others would not experience said issue.
- Improved Bazaar search performance
- Prismatic Scale of the Elements (Legendary) is now Attunable instead of No Trade.
- Splinters of Time without a proc are now the correct aug type.
- Bard song aggro was incorrectly inflated. Fixed.
- Ranger archery bonus now correctly begins at 50 instead of 51.
- Hand of Ro now stacks with other -Fire Resist debuffs
- Pets can once again be issued commands from the default range.
- Xegony key will now Keyring
- Symbol of Torden will now Keyring
- Prevent pets from being added to mob hate lists if they are on hold
- 2H Bash & Slam now works with Autoskill
- Reduced the Damage Shield component of Blessing of Praesertum Matpa
- Revamped 'Stats' page on Default UI
- /autoskill now supports Taunt
- Fixed inconsistencies around basic stat caps and certain spell effects
- Fixed pets with taunt off still pulling aggro
- Fixed pets with taunt off still eating rampage
- Fixed swarm pets not obeying custom pet restrictions (proc rate etc)
- Added the following EQTypes for UI makers.
    ClassAbbrList = 6666,
    TrueEvasion = 6667,
    TrueMitigation = 6668,
    WornATK = 6669,
    ItemExp = 6670,
    SpellCritRate = 6671,
    SpellCritRatio = 6672,
    HealCritRate = 6673,
    HoTCritRate = 6674,
    DoTCritRate = 6675,
    DoTCritRatio = 6676,
    MeleeCritRate = 6677,
    MeleeCritRatio = 6678,
    PetFlurryRate = 6679,
    PetMeleeCritRate = 6680,
    PetAvoidance = 6681,
    PetMeleeMitigation = 6682,
    PrimaryActualDelay = 6683,
    SecondaryActualDelay = 6684,
    Pet0Taunt = 6685,
    Pet1Taunt = 6686,
    Pet2Taunt = 6687,
    Pet0Hold = 6688,
    Pet1Hold = 6689,
    Pet2Hold = 6690,
    Pet0GHold = 6691,
    Pet1GHold = 6692,
    Pet2GHold = 6693,
    Pet0Focus = 6694,
    Pet1Focus = 6695,
    Pet2Focus = 6696,
    Pet0Spellhold = 6697,
    Pet1Spellhold = 6698,
    Pet2Spellhold = 6699,
    Pet0SPO = 6700,
    Pet1SPO = 6701,
    Pet2SPO = 6702,
    CapClairvoyance = 6703,
    CapHealAmount = 6704,
    CapSpellDamage = 6705,
    CapWornATK = 6706,
    ArcheryCritRate = 6707,
    RuneAmount = 6708,
    SpellRuneAmount = 6709
```

Known Issues:
```
- Pets with taunt OFF should be ignored by mobs - This is not working correctly
```

---

---

## 2025-04-04 06:23 - Entry 1357601537861615697
**Author:** Catapultam

Hotfix
```
- Pets which are not taunting should REALLY be immune to rampage now.
- Kerafyrm may now have more than one scale.

- Pets will only resync gear when inventory operations are performed with the pet bag instead of all operations
- Reduced the number of equipment change packets being sent in certain circumstances
```

---

---

## 2025-04-03 18:54 - Entry 1357428075155165204
**Author:** Catapultam

```
- Re-Enabled Global Buffs
- Various backend performance improvements
- Zebuxoruk now drops minimum of Enchanted quality augments, and can rarely drop additional augments.
- Lord Inquisitor Seru has a higher probability of dropping additional loot based on the number of difficulty-enhancing buffs present on him
```

---

---

## 2025-04-03 05:35 - Entry 1357226963760316516
**Author:** Catapultam

Late Night Hotfix
```

- Temporarily disabled global buffs through Apocrypha and the event Signets (Manually extended for 24hrs!)

* Needs new Zone Server (Probably won't work in Bazaar, will be more reliabile as zones cycle out) *
- #commands will be consumed in any channel (the spam should go down)
- attackmode ranged should be less laggy and more reliable for displaying weapons correctly

* Needs CLIENT UPDATE (PATCH) *
- Added the following command aliases
  /pet (#petcmd)
  /attackmode (#attackmode)
  /autoskill (#autoskill)
- #commands should no longer echo in chat (even if nobody could see them when properly consumed)
```

---

---

## 2025-04-02 01:27 - Entry 1356802123106357349
**Author:** Catapultam

4/2/2025 (Yes, this one is real)
```
- Reverted class deletions. Implemented <<# a u t o s k i l l>> instead
  - Initially supports the following Skill attacks
      Backstab
      Bash
      Tiger Claw
      Eagle Strike
      Dragon Punch / Tail Rake
      Flying Kick
      Round Kick
      Kick
      Frenzy
  - Absolutely no timer deconfliction is executed by the command, please only enable skills you want to be used.

- Implemented #attackmode
  - Rangers no longer display their bow by default. Any character can use #attackmode ranged to preferentially use their bow for autoattack and display

- Implemented #petcmd
  - Pet window buttons (and hotkeys created from them, or /pet commands) only send instructions to the 'active pet' (the pet displayed in the window)
  - 'Triple-pet' UI mod is not recommended, as it may be confusing as to which pet is 'active'
  - added #petcmd to send instructions to ANY pets (send commands by class name, etc)
  - Usage: #petcmd [attack, qattack, follow, guard, sit, stop, taunt (on\\off), hold (on\\off), ghold (on\\off), spellhold (on\\off), focus (on\\off), back, regroup (on\\off)] [all, mag, bst, nec, enc, shm, dru, brd, shd].
  - Any number of command and target verbs may be used at the same time, and in any order
  - /pet health and #petcmd health now display inventory for that pet

- Removed access to #mystats. On most servers, the inventory\player profile page is inaccurate and so mystats is needed. On this one, due to the unique nature of our technology, the inverse is true.

- Corrected bug which allowed creation of augmented items that were not usable in any slots.
- Syncrosatchels or equivalents will now consider slotted augments to determine which slot an item can be equipped into
- Splinters of Time which are not PRI\SEC\RANGE no longer require slotting into a weapon
- Dispel-type spells cast by players on players or player pets are no longer resistable.
- Dispel-type spells cast by mobs are now resistable.
- Fixed Monk class names display on Character Select
- Sol Ro Tower respawn timers have been fixed.
- Legends of Norrath cards no longer have a self consume clicky effect and have an updated lore.
- Innoruuk and Rallos Zeks adds no longer leash and assist their god
- Aid Grimmel quest npc should be more responsive now.
- The rztwl event in plane of tactics should behave even more as expected, with failure timers removed.
- The Fennin event in plane of fire should now correctly resume when returning to the zone and no longer fails on timeout.
- Plane of Earth a ring events rewritten to be more resilient to zoning out. (Thanks Pippz)
- Echo added to Splitpaw
- Mortal Coil is no longer blocked by random clickies
- Villagers in HoHA are now tethered and will not run full marathons.
- 61-65 LDoN spells have been added to PoP parchment turn in rewards
- 50-60 LDoN spells have been added to Warders, Ancients, Lords and Ladies in Velious
- Mistakenly remaining GoD and OoW spells have been removed from PoK vendors *and* player spellbooks.
- Lvl 62 BST and lvl 63 Necro pet now correctly scale their level.
- The likelihood of finding weapon augments has increased on the Glamour NPC.
- Aspect of the Reptile duration has been increased.
- /shield now works for Warriors level 30 or greater
- All entities are capped at 35 worn Shielding
- Switched Prismatic Strike to Chromatic resist type
```

---

---

## 2025-04-01 14:25 - Entry 1356635539750650037
**Author:** Catapultam

```
- Implemented the new Player Rendering Overhaul!
This feature, unique to THJ, will provide an unparalleled graphics experience like you have never seen before! Enjoy AAA quality which you had never imagined that you'd see in this game. Please note that this is a REQUIRED feature, and out of date clients will be disconnected automatically, so please remember to patch!

- Nerfed Mnk/Mnk/Mnk
- Removed several redundant player classes; Monks, Rogue, Warrior, Wizard, Berserker are all classes who's roles are better performed by other classes, and so these have been permanently disabled.
- Bard has been removed because it is just too much trouble and causes too many bugs.
```

---

---

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

## 2025-03-22 03:31 - Entry 1352847240527609957
**Author:** Catapultam

Running changelog for Post-PoP hotfixes.
```
- Corrected flagging logic for Aerin`Dar event.
- Corrected flagging logic for Grummus event
- Corrected flagging logic for Hedge event
- Corrected goup port logic for PoJ trials
- Corrected group port logic for Keeper of Souls

- Fixed zone crash related to tradeskills
- Fixed inability to mix enchanted\legendary in standard tradeskill combines
```

---

---

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

## 2025-03-12 21:16 - Entry 1349491176792658022
**Author:** Aporia

This is a changelog post to test the new patcher.

```
Words. Changes. Nerfed monks.
```

---

---

## 2025-03-12 16:55 - Entry 1349425683507708005
**Author:** Catapultam

Hotfix -> Requires new zone zervers to take effect
```
- Fixed pets not correctly calculating spell proc rate
```

---

---

## 2025-03-12 16:03 - Entry 1349412549308842084
**Author:** Catapultam

```
- Doppelgangers now respect spell recast times of spells they inherit from their owner.
- Swarm pets inherit spell modifiers from their owner even when their owner has no other pets
- Zone State restoration is now improved in such a way as to prevent spawning multiple mobs on zone restore.
```

---

---

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

## 2025-03-08 06:48 - Entry 1347823190017052734
**Author:** Catapultam

```
- Re-enabled Zone State Preservation
- Fixed incorrectly calculated stat caps
- Fixed crash that could occur with certain player events
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

## 2025-02-17 17:44 - Entry 1341103053197283349
**Author:** Catapultam

```
- Consolidated Echo of Aegolism, Echo of the Grove, Echo of the Brood, Echo of Focus, and Echo of Koadiac into Echo of Power.
- Replaced Knight's Rebuke with existing AA: Knight's Return Strike
- Fixed several errors with Valentine's Day event scripts
- Prevented Forlorn Follower of Erolisi from replacing certain NPCs
```

Important Information & Errata:

- Forlorn Follower of Erollisi are *still* whatever their base NPC is. They still have the same quests, scripts, etc. If you need them to *die* for some event to work correctly, just kill them, don't use their dialogue to make them depop.
- Echo of Power is not a direct 1:1 comparison to the effects of the old buffs, and may be adjusted in the future. The application of buff scaling makes the consolidated buff scale a little bit differently than the composite buffs.

---

---

## 2025-02-13 23:51 - Entry 1339745754541064212
**Author:** Catapultam

```
- Fixed regression in zone scaling script. Mobs should no longer heal when someone enters or leaves zone
- Worg pets should no longer try to visually hold weapons.
- Speculative fix to make glamour appearances more reliable.
- Adjusted Doppelganger spellcasting priority
- Adjusted Doppelganger spell stacking
- Adjusted pet aggro distribution (pet taunt on\off)
```

---

---

## 2025-02-13 06:06 - Entry 1339477902109966367
**Author:** Aporia

```
Please be aware, Doppelganger is being actively worked on as we try to make it behave more offensively.

We realize that not being able to control what default spells were being used was not an ideal UX and are working toward a more intuitive spell set.

Expect Doppelganger to cast spells from you bar + their original nukes for now.

Thank you!
```

---

---

## 2025-02-11 06:30 - Entry 1338759014258970654
**Author:** Catapultam

```
- Fixed Praesertum Mapta's infinite healing exploit
- Fixed players being immune to stun for a period of time after being stunned.
- Removed several undesirable spells from Doppelgangers
- Doppelgangers no longer use AoE spells of any type from their owner's memorized spell list.
- Lowered the spawn time of A File Cabinet

- Players will become immune to silence for a period of time after becoming silenced.
```

---

---

## 2025-02-10 07:33 - Entry 1338412565780238357
**Author:** Catapultam

Hotfix
```
- Returned Destructive Fury to Wizard AA list.
- Removed Fear, Blind, and Charm spells from Doppelganger spell lists (requires new zone server, may not work in existing instances)
- Removed extra 10 ranks of (unpurchasable) Fury of Magic from some classes (will remain visible in bazaar, also a new zone servers thing)
```

---

---

## 2025-02-10 05:14 - Entry 1338377526820601906
**Author:** Catapultam

```
- Various spells and songs corrected to have haste instead of Slay Undead
- Lord Inquisitor Seru now correctly uses certain abilities if he has the support of any of his Praeserti
- Lord Inquisitor Seru's death reward event will now fire more reliabily
- Many fixes to various encounter scripts (@Trust, @Zimp)
- Removed Fling effect from Battle Leap
- Removed Warders in VT
- Removed depop timer from The Insanity Crawler
- XTC unrooted
- Ssra High Priest unrooted
- Various double-spawns of bosses in ssrratemple have been removed
- Shadowstone idol NO-VALUE tag removed
- Reduced the HP of VT trash by 50%
- Reduced the respawn time of VT trash to match other XP zones.
- Bane Weapons will allow skill attacks (Frenzy, Backstab, Monk attacks, etc) to function.
- A File Cabinet respawn time adjusted to 1 hour, 59 minutes, 59 seconds, making it eligible to spawn in respawning instances.
- Power Source item growth rate increased. We will monitor this for re-evaluation.
- Removed ranks 7-9 of Fury of Magic which were incorrectly made available to hybrid classes.


Doppelganger Rework
- The enchanter AA Doppelganger has been largely reworked.
- Doppelgangers now gain the Equipment, (Long-Duration) Buffs, and Spells of the Enchanter who created them has at time they are created.
- They will use Nukes, Lifetaps, DoTs, Slows, Debuffs, and Snares. They will NOT use any other type of spell, including AoE spells.
```

---

---

## 2025-02-08 21:12 - Entry 1337893727150014565
**Author:** Aporia

Pending Reboot:

```
- Vex Thall Trash HP has been reduced by 50%
- Vex Thall ZEM has been increased.
- All VT mobs are a minimum of level 60
- Fungal Infusion now removes curse counters!
- Silence on Thall Va Xakra, and Diabo Xi Xin Thall now behave like Aten Ha Ra's. For every 12 seconds you are silenced, you will now have a 12 second reprieve.
```

---

---

## 2025-02-06 23:52 - Entry 1337209418198286398
**Author:** Aporia

THIS CHANGELOG IS ALSO FOR LUCLIN RELEASE AND IS NOT COMPLETE/MAY CHANGE BEFORE LAUNCH

```
**Balance**

- Cleric's Divine Avatar has been scaled down, but remains one of the most powerful AA's in the game. Duration reduced to 2 minutes. Melee damage bonus and proc chance reduced to 100.
- Pet's now have a hard cap on how much Flurry, Crit, Crit Damage, and Proc rate they can access (75%/75%/75%/100)
- Wizard AA Improved Familiar no longer gives stacking critical spell damage (Total decrease of 7.8% with all crit damage buffs going.)

- Warrior's Battle Leap AA duration to 12 seconds and increase damage modifier SPA 185 to 25% at RkI. RkII has been added for purchase for a 50% increase.
- Warrior's Fellstrike Discipline duration increased to 1.5 min
- Paladin's Holyforge Discipline now does crit and 50% SPA 185 *instead of crit and crippling blow* but had it's duration reduced to 2 minutes
- Rogue's Lethality increased to 40% SPA 185
- Rogue's Thief's Vengeance Discipline was increased to a 12 second duration
- Rogue only piercers now give additional backstab damage (x3)
- Druid's Spirit of the Bear now adds 75% SPA 185
- Druid's Spirit of the White Wolf now reduces spell cost by 20-25%, increases chance to critical heal by 15% and increases the chance to critical heal on a heal over time by 20%.
- Druid's Spirit of the Black Wolf now reduces spell cost by 20-25%, increases chance to land a critical hit with detrimental spells by 10%, increases critical spell damage by 50%, increases critical DoT chance by 10% and critical DoT damage by 50%
- Shaman's Rabid Bear proc now has a -50 disease resist modifier and a -50 disease resist check on the proc
- Shaman's Rabid Bear can now increase the stat cap of Str and Dex by 25/50/75

**Additional Changes:**

- Named mob spawn chance increased in SSRA basement (Strange Green Metal mobs)
- Bard Hymn of the Last Stand detrimental portion can no longer crit or get modified by spell damage and kill you.
- Aten Ha Ra's Silence of the Shadows now has a 24s recast time. Word of Command now has a 6s recast time.
- Fixed several broken spawns in Sanctus Seru
- Fungal Infusion now gives back 250 endurance in addition to its regular 250 mana
- Divine Hammer of Consternation and it's Corrupted counterpart now proc Divine Shield instead of Divine Aura
- Bixie parts can now drop from Bixies in PoM
- ZEM of Velious zones reduced.
- ZEM of Luclin zones increased.
- Thief's Vengeance Endurance cost lowered to 350
- Mark of Karn now has a -75 resist check and takes only 2 seconds to cast.

**DZs Added**

- Grimling Forest
- Acrylia Caverns
- The Gray
- The Deep
- The Fungus Grove
- Umbral Plains
- Dawnshroud Peaks
- Twilight Sea
- Vex Thel
- Sanctus Seru
- Katta Castellum
- Ssraeshza Temple
- Akheva Ruins
- Grieg's End
- Feerrott
- Lesser Faydark
- Swamp of No Hope

**The 10th Ring War is now working!**
A HUGE thank you to Pippz and the many hands that went in to fixing this!

10th Ring War rewards have had their stats increased:

- (Crown of Narandi, only awarded if Churn stays alive)
- (Eye of Narandi, only awarded if Kurgin stays alive)
- (Earring of the Frozen Skull, only awarded if Corbin stays alive)
- (Faceguard of Bentos the Hero, only awarded if Dobbin stays alive)
- (Choker of the Wretched, only if Garadain stays alive)
- (Ring of Dain Frostreaver IV, always rewarded)

**The Ring of Fire is in for Luclin!**
A HUGE thank you to Trust and the hands that went in to testing this!
```

---

---

## 2025-02-06 23:47 - Entry 1337208133201690625
**Author:** Catapultam

THIS CHANGELOG IS FOR LUCLIN RELEASE AND IS NOT COMPLETE

```
- Updated to EQEmu 22.62.2
- 'Improved the netcode'

Fixes:
- Purify Body should now work as expected
- BoBs will no longer sell to any merchant regardless of faction
- Players entering or leaving the zone in a Non-Respawning instance with more than 2 members will no longer cause mobs to heal
- Faded Memory should spawn for Zlandikar and the other guy
- Items with slots incorrectly set to only allow one wrist have been corrected to allow both wrists.
- Fix zone crash that could occur when a script not directly attached to an NPC could instruct a recently dead NPC to Move to a new location.
- Various NPCs will no longer flee when kicked.
- Certain tradeskill recipes will no longer return incorrect items via Salvage AA
- Fixed various luclin encounters (thx @Trust, @Zimp, others)
- Gnomes can now acquire Tinkering Mastery AA
- Fixed a number of Haste spells that were actually Slows (Bards, Rejoice!)
- Fixed Reverse DS effects not working
- Doppelgangers will no longer use ranged attacks, they will only cast spells.

Changes:
- Languid Bite and Deep Sleep should now trigger off AA casts
- Magicians no longer keep TEMPORARY items unless they have a spell that can summon them (like any other class)
- Added QUEST tag to most items used in any kind of quest Turn-In.
- Ring of the Shissar is now No-Trade
- SPA 185 (SE_DamageModifier) now stacks.
- Adjusted Arx key to only work inside Sanctus Seru, and be instance aware
- Lord Inquisitor Seru will banish any attacker who does not possess an Arx

New:
- Returned Jolum to the Bazaar
  - Jolum will exchange your summoned Grandmaster's Satchel for a permanent, 30-slot Grandmaster's Carry-All. This item is LORE.
  - Grandmaster's Satchel and Grandmaster's Carry-All are now No-Drop.
- Added 15 additional ranks of Mystical Attuning
- Added Knight's Rebuke AA for Paladins
  - Allows Bash on Riposte


```

---

---

## 2025-02-03 17:58 - Entry 1336033147346878590
**Author:** Catapultam

Posting this early because it went out early
```
- Updated Default Maps
- Added Dark Mode maps option (dropdown menu in map window)
```

---

---

## 2025-02-03 04:05 - Entry 1335823574799224852
**Author:** Aporia

```
- The Echo of the Past for Nagafen's Lair, Permafrost, and Velketor's lab have been moved inside their respective zones.
- If you see an Echo of the Past in Lavastorm or Everfrost, please ignore them and zone in to the respective zone to pull your DZ.
- Great Divide still has an Echo of the Past but it is now at the succor location to the south of the zone and is meant to spawn a DZ for Great Divide itself.
```

---

---

## 2025-01-31 14:56 - Entry 1334900028866826271
**Author:** Catapultam

```
- Peridots are no longer marked NO VALUE
- Fixed Bag of Bartering prompt not displaying in some circumstances.
- Bag of Bartering prompt is now sorted by item stats and value, but may be truncated for large item lists.

- Reduced packet resend aggressiveness - This may help with connection stability for some users
```

---

---

## 2025-01-29 20:32 - Entry 1334259808114839553
**Author:** Catapultam

```
- Updated to EQEmu v22.61.1
```
https://github.com/EQEmu/Server/pull/4617
https://github.com/EQEmu/Server/pull/4627

---

---

## 2025-01-25 23:41 - Entry 1332857825009078393
**Author:** Catapultam

```
- Fixed Guild Member level display. (Client Patch Required)
```

---

---

## 2025-01-25 17:10 - Entry 1332759507641827409
**Author:** Aporia

Pending Server Reboot:

```
- Consolidated logic on both populating and executing Bags of Bartering. This should reduce confusion and increase accuracy about which items are actually eligible to be sold.
- Berserker Summoned Axes may no longer be vendored
- No-Rent items may no longer be vendored
- Items with Augments may no longer be auto-vendored
- Removed a bunch of inaccessible NPCs from the Bazaar
- Added NO-VALUE tag to many items given by trivial quest scripts.
- Added NO-VALUE tag to all summoned items
- All players with Tracking should now be able to filter track results
- Fixed memory leak in client which caused map to not properly reset spawn lists under some circumstances
- Reduced the 'merchant multiplier' on most items.
- Fixed several memory leaks
- Re-enabled direct inventory delivery via Delivery Vouchers
- Adjusted client memory map in a speculative fix for out of memory client crashes

Quest Fixes:
- Quests fixes related to Qeynos Badge
- Implemented JFP War
- Cleaned up Shaman Cudgel & Skull quest
  - Added Flags to each step to monitor progress
  - Added faction and level checking per step
  - Added notice of flags being assigned (So they are not "Invisible")
  - Added Dialog to Oxyn "Progress" that will output current progress point.
  - Limited a quest turn-in that can be exploited for fast and unlimited EXP
- Misc Befallen cleanup
- Fixed Faction hits around Giant Scarab quests in Kaladim
- Various Quest fixes in qey2hh1
- Corrected several quests which rewarded the wrong items.

- Added Mystic Soulbinding Apparatus to Gemcrafter Anuk This reusable device allows you to attune any item, preventing it from being accidentially sold or|| traded.

- Unflinching Resolve and Stalwart Endurance have been removed from the game.
- Any player that has a single point of Unflinching Resolve or Stalwart Endurance will be given Steadfast Will

- The vendor cost of items has increased as the sell value on some has increased.

```

---

---

## 2025-01-23 16:46 - Entry 1332028783162818775
**Author:** Catapultam

```
- Items should now never be able to be sold for more than they are bought for.
- No-Rent items can not be sold via Bags of Bartering
- Custom Pet Names restored
```

---

---

## 2025-01-23 14:41 - Entry 1331997123805184092
**Author:** Catapultam

```
- Type 21 Glamour-Stones no longer require item type armor
- Fixed EoM-purchased Gnomish Quadramorphic Combinerator
- Bazaar Parcel Fee removed when inside the Bazaar (any instance)
- Disabled 'Warp to Trader' functionality from Find Trader
- Changing Pal\SK Epic from one form to another will no longer eat augs

- Added Delivery Vouchers & Direct to Inventory Delivery
  - Purchased from Merchant Aina for platinum
  - Purchased from Echo of Memory for EoM
  - Each direct to inventory delivery will consume 1 Delivery Voucher from your Alt Currency.

- Increased standard stack size to 1000
- All items have a sell value based on stats.
- Item Previews are now avaiable (alt-rightclick item icon in 'item inspect' window)
```

---

---

## 2025-01-22 20:34 - Entry 1331723721295003740
**Author:** Aporia

Changes:
```
- Kildrukaun the Ancient's Typhoon Breath now casts once every 45 seconds instead of 15.
- Bladesoul's Spiritual Diadem now correctly classified as armor
- Lvl 50+ Druid and Shaman pets will now benefit from Pet Power 15, 20, and 25.
- Misc item description updates
- A Knight of Luclin now correctly reports the targets needed for Luclin unlock
- Fixed Z-axis of ground spawns in Lake Rathe
- Key of Torsis is now correctly set to a 100% drop rate
- Stun Resist AAs are being squished to prevent overflows. Steadfast Will will now be available for (WAR/PAL/SK/MNK/BER). Dauntless Perseverance has been removed entirely as stun resist > 100 does nothing.
```

Pending Patch:
```
Unflinching Resolve and Stalwart Endurance have been removed from the game.
- Any player that has a single point of Unflinching Resolve or Stalwart Endurance will be given Steadfast Will on next downtime.
```

---

---

## 2025-01-17 19:20 - Entry 1329893093335371877
**Author:** Catapultam

CHANGES

```
- Kerafyrm event adjusted.
  - Typhoon Breath has had its curse counters cut in half and it's cooldown tripled.
  - The Warders have been reintroduced to the pool of potential adds for the ecnounter.
- Fixed missing 'the Naughty' and 'the Grinch' titles
- Fixed Double\Triple attack not working for Throwing
- Rysva To`Biath will now allow completion of the Book of Scale quest
- Instant-Cast clickies can be activated while singing bard songs
- Improved logic around rune stacking with regard to bard songs
- Reverted change that resulted in bags not being able to be sold back to EoM vendor
- Unattuner and Gnomish Quadramorphic Combinerator can only be sold back to EoM vendor if they were purchased with EoM
- Unattuner and GQC is no longer NO-DROP
- Vibrating Gauntlet\Hammer of Infuse will preserve augments when swapping (invalid augs will fall out)
- Characters with a Trader's Satchel in their inventory who find themselves in a zone other than Bazaar will be moved back to Bazaar

- Fixed inspect item not working when outside of the instance containing a Bazaar trader.
- Fixed off-by-1 error with regard to Bazaar Shard numbering

- Added Bag of Bartering and Belt Pouches of Bartering to Echo of Memory in Bazaar
 - These bags will allow you to Sell All or Keep One Per Stack of their contents when interacting with a Merchant
 - Bag of Bartering - 30 slots, Max Size Giant, 100% WR
 - Belt Pouches of Bartering - 100 slots, Max Size Small, 100% WR
   - Pro Tip: Put this one in your LAST inventory slot to act like a 'filter' for preconfigured junk in combination with 'Keep One Per Stack' sell mode
```

KNOWN ISSUES
```
- Traders in Bazaar Shard 1 will show as their name if you are in any open world zone, not just the Bazaar
```

EXTRA
```
An EXPERIMENTAL client configuration change has been added to the 'extra' directory in the patcher. BACK UP and then replace your 'resources/Memory.ini' file with this if you experience frequent crashes while zoning, especially if you have gone to discord for help and been told it was the 'graphics memory crash'.
```

---

---

## 2025-01-16 14:59 - Entry 1329465177497665590
**Author:** Aporia

Pending Reboot:

```
- Typhoon Breath has had its curse counters cut in half and it's cooldown tripled.
```

---

---

## 2025-01-16 01:38 - Entry 1329263425905229878
**Author:** Catapultam

NINJA CHANGELOG
```
- Polymorphist now properly accepts EoM
```

---

---

## 2025-01-15 04:01 - Entry 1328936987754889247
**Author:** Catapultam

BONUS CHANGELOG
```
- Lokar To`Biath in neriakc now accepts stacks of items.
- Lashun Novashine in North Qeynos now accepts stacks of items.
- Captain Tillin in South Qeynos now accepts stacks of items.
- Captain Bosec in Highkeep now accepts stacks of items.
- Trooper Mozo in Cabilis now accepts stacks of items.
- Pandos Flintside in West Freeport now accepts stacks of items.
- Niola Impholder in South Felwithe now accepts stacks of items.
```

---

---

## 2025-01-15 03:05 - Entry 1328923023532752966
**Author:** Catapultam

```
- The Polymorphist now allows you to set custom pet names
  - Default pet names have been reset as part of moving to new pet name system
- All Polymorphist services may now be purchased with platinum.

- Purchasing via Parcel from Bazaar now adds parcel tax once again
- Bazaar trader cap lifted.
- Traders not in-zone will display as 'Bazaar Shard N' where N is the shard where they are located

- Kerafyrm encounter adjusted.
- Wizard Familiar spells no longer spawn a flappy
- Cycle Pet\Self hotkey will now cycle between all pets
- Removed servers other than THJ from server list

- Blinded By Fury is now a short-duration buff that is not suspend-able.
- Frenzy Weapon Scaling is now sum of Primary + Secondary
- Added Tunable to Frenzy Weapon Scaling (default same value as before)
  - FrenzyScaleOnWeaponAmount
- Added Monk Kick\Strike weapon damage scaling and tunable.
  - MonkScaleOnWeaponAmount
- Added Monk Kick\Strike Hand\Foot damage scaling and tunable
 - MonkScaleOnHandFeetQuality
```

---

---

## 2025-01-11 01:30 - Entry 1327449601371934735
**Author:** Aporia

Pending Patch:

```
- Burned Out Lightstone no longer glows so bright
- Echo of the Past should now be findable
- Lioness Matriarch and Lion Patriarch can now drop Lion Skins in addition to pelts. (Fleeting Quiver seekers rejoice)
- Killing Dozekar the Cursed now correctly spawns A Faded Memory
- Killing Kelorek`Dar now correctly spawns A Faded Memory
- Paladins now have access to the Shield Specialist AA
- The Shield Specialist AA has been increased for Warrior and Paladin to increase auto attack damage with your primary weapon by 20/40/60/80/100%
- Paladins now have access to the Holy Shield AA (The Paladin's shield is imbued with holy light increasing the Paladin's chance to proc all effects and allows the Paladin to cloak themselves in a runic shield while fighting. Requires maximum rank in Shield Specialist.)
- The Vicious Smash AA has had its effect doubled.
- A Tribute Master has been added to EC Tunnel
- Certain legendary items have had their missing stats added back.
- The Endless Cookie Platter now let’s you know that you do, indeed, summon a cookie.
- Updated description of Paladin Discipline Holyforge to indicate its effect against *all targets*. (This was always the case, most people just didn’t know.)
- Snarla the Fang now gives the correct faction
- Druid AA Wrath of the Wild tooltip has been updated to reflect its current implementation: “This ability will shield you with a charge based, large damage barrier of thorns. When each charge is consumed there is a chance to grant the player an additional blessing: Protection of the Spirit Wolf.”
- Enchanter AA Hastened Edict of Command has had Rk 1/2/3 added to the game. Rk3 brings the CD of Edict down to 30 minutes.
- Berzerker AA Hastened Savage Spirit is now available with the final rank bringing its CD to 20 minutes.
- Rogue AA Hasty Exit has had ranks added bringing its final CD to 5 minutes.
```

---

---

## 2025-01-04 02:37 - Entry 1324929653957328956
**Author:** Catapultam

```
New:
- The Heroes' Journey patcher will now automatically back up your UI configurations and detect when they have become corrupted. (Thanks @Xackery!)

Adjustments:
- Bristlebane has been rebalanced
- Gaining XP while at AAXP cap no longer sets percentage of XP assigned to AA to 0%.

Bug Fixes:
- Countless script fixes (Thanks @Trust!)
- Traders should now be cleaned up if a zone server crashes
- Fixed a memory leak in pet bags
- All Handin quests should now work

```

Additionally; it is now possible for us to update quest scripts to allow handing in stacks at a time. This requires reworking the script, however, and so will not be a global change.

We are crowdsourcing quests which would benefit from this treatment -> [Here](https://docs.google.com/document/d/1D-BxDDT6pFQHfxA6dcqdbxU9f2mMFgvtZbTvMomF47E/edit?tab=t.0)

---

---

## 2025-01-01 20:30 - Entry 1324112534776713266
**Author:** Aporia

Out of respect for player time and expected engagement, the following changes have been made:

```
- Non raid bosses in ToV have had their HP reduced.
- Thifling Focuser's in PoG have had their HP reduced.
```

---

---

## 2025-01-01 16:10 - Entry 1324047001591091262
**Author:** Catapultam

```
- Implemented limit of 599 total active traders to work around client bug (More comprehensive workaround to come)
```

---

---

## 2024-12-31 18:17 - Entry 1323716631951577148
**Author:** Aporia

```
- Enchanter AA Mana Draw now has a 10 minute CD with Rk3 Hastened Gathering
- The Sleeper will no longer reset his HP to full when he roars.
- The Sleeper will now despawn his adds from phase 4 if a player dies and re-engages at full health.
- Misc Faction fixes (Thanks Trust!)
```

---

---

## 2024-12-31 18:04 - Entry 1323713355206234286
**Author:** Catapultam

```
- Experimental change for /baz crash
- Experimental change for crash-on-zone
```

---

---

## 2024-12-30 21:54 - Entry 1323409018273923123
**Author:** Catapultam

I am a generous god.
```
- The Vision of Ayonae will now allow you to reduce your level, and return to up to your previous maximum level. This service costs 500pp per level changed.
```

---

---

## 2024-12-30 01:46 - Entry 1323104912036462603
**Author:** Catapultam

```
Added:
- Urthron's Ultimate Unattuner has been added for sale from Gemcrafter Anuk
- Gnomish Quadramorphic Combinerator has been added for sale from Gemcrafter Anuk
- Vial of Prismatic Dye has been added for sale from Gemcrafter Anuk

Adjusted:
- Donal's Chestplate of Mourning now casts regular Complete Heal with a 30 second recast
- Melodic Breastplate clicks at level 1.

UX:
- Pets will no longer accept a Syncrosatchel which is traded to them.

Bug Fixes:
- Turn-ins with multiple identical items will once again function
- Recovering Parcels will no longer require an open top-level inventory slot (Thanks @Neckkola)
- Items with charges will no longer be interpreted as stacked items for quest turnins.
- Restored No-Rent\Temporary item timer to 1800 seconds (was set to 1 second for debugging, which made it to prod)
- Non-Mages who can summon an item will find that those items are much more permanent.
- Corrected model for velium spiders in Velketor's Labyrinth
- Corrected model for crystal golems in Velketor's Labyrinth
- Corrected model for gargoyles in Velketor's Labyrinth
- Corrected model for Velketor the Sorcerer
- Corrected model for Snow Cougars
- Corrected a script error in Dain Frostreaver IV
- Thunder Spirit Princess will once again accept 10 gold
- Fixed zone crash on conning mobs in some edge cases
- Fixed zone crash on handing items to pets in some edge cases
- SE_FadingMemories no longer applies to the caster of the effect instead of the target when applied to an NPC.
- Pets are cleaned up on death once more
- Fixed bad plat handling on Purveyor of Glamour and a few other NPCs
- Tradeskill combines will display skill-up messages.
- GM Training will display skill-up messages.
- Custom Helms will now return the correct quality
- Reworked Tunare encounter
- Reworked Bristlebane encounter
- Reworked TOFS mirrors and keys
- Added DZs for TOFS, CC, Iceclad
```

---

---

## 2024-12-26 03:59 - Entry 1321688812581027932
**Author:** Catapultam

Rolling log for *TEST* while I get velious ready.... Final patch notes will be re-posted prior to Velious launch.
```
New:
- Added per-class pet bags. See bag vendor in the Bazaar or Shady Swashbuckler in EC Tunnel. If you choose not to use a pet bag, no item reimbursements will be given for lost items.
- Reworked NPC hand-ins, it should now be impossible to hand an item to an NPC and have it eaten (other than pets without a pet bag).

Removed:
- Charmed pets will no longer hand back items given to them. Use a Syncrosatchel to equip your pet or rely on vanilla charm-gear mechanics.

Bug Fix:
- Corrected bug applying spell damage\crit incorrectly to pets
- Corrected bug preventing heal amount from being applied to pet procs
- Corrected bug preventing spell damage from being applied to pet DoT procs
- Pets using 2h weapons no longer reduce added damage by 1/2
- No-Rent\TEMPORARY bags should now correctly be replaced by their disenchanted versions instead of destroying their contents.
- Pets should no longer be deleted for players who are logged on as the server goes down.
- Berserker Disciplines should no longer be removed when dropping (non-Berserker) classes.
- Spells that you can no longer cast because of deleveling are no longer removed when dropping classes.
- Sympathetic Procs will no longer trigger twice for one of your pets.
- *Most* pets may once again be shrunk. Some are buggy still, working on it.

Adjusted:
- Pets now inherit 50% of their owner's spell damage, heal amount, critical spell damage and critical healing on procs\spells.
- Pets with 2H weapons equipped no longer equip an offhand.
- Pets use equipped weapon delay instead of standard NPC delay.
- Pets base damage is normalized to their new attack delay.
- Pets directly add their equipped weapon damage to their attacks.
- Syncrosatchels increased to 4 slots.
- TEMPORARY items will not expire while logged off if you can summon that item via a spell in your spellbook. (Or, for now, are a Magician)
- All spells should be deletable from spellbook (Requires additional client patch)

Misc:
- Progression targets for Luclin unlock have been finalized; Zlandikar, Klandikar, Wuoshi, Kelorek'Dar, and Dozekar the Cursed
```

---

---

## 2024-12-24 22:04 - Entry 1321237072048033833
**Author:** Catapultam

New **TEST** build
```
New:
- Added per-class pet bags. See bag vendor in the Bazaar. If you choose not to use a pet bag, no item reimbursements will be given for lost items.
- Reworked NPC hand-ins, it should now be impossible to hand an item to an NPC and have it eaten (other than pets without a pet bag).

Removed:
- Charmed pets will no longer hand back items given to them. Use a Syncrosatchel to equip your pet or rely on vanilla charm-gear mechanics.

Bug Fix:
- Corrected bug applying spell damage\crit incorrectly to pets
- Corrected bug preventing heal amount from being applied to pet procs
- Corrected bug preventing spell damage from being applied to pet DoT procs
- Pets using 2h weapons no longer reduce added damage by 1/2
- No-Rent\TEMPORARY bags should now correctly be replaced by their disenchanted versions instead of destroying their contents.

Adjusted:
- Pets now inherit 50% of their owner's spell damage, heal amount, critical spell damage and critical healing on procs\spells.
- Pets with 2H weapons equipped no longer equip an offhand.
- Pets use equipped weapon delay instead of standard NPC delay.
```

---

---

## 2024-12-24 07:39 - Entry 1321019345039790141
**Author:** Catapultam

The below is deployed on THJ Test Server and is available for further testing.

Merry Christmas?

```
New:
- Added per-class pet bags. See bag vendor in the Bazaar. If you choose not to use a pet bag, no item reimbursements will be given for lost items.
- Reworked NPC hand-ins, it should now be impossible to hand an item to an NPC and have it eaten (other than pets without a pet bag).

Removed:
- Enchanter pets will no longer hand back items given to them. Use the Enchanter's Syncrosatchel to equip your pet or rely on vanilla charm-gear mechanics.

Bug Fix:
- Corrected bug applying spell damage\crit incorrectly to pets
- Corrected bug preventing heal amount from being applied to pet procs
- Corrected bug preventing spell damage from being applied to pet DoT procs
- Pets using 2h weapons no longer reduce added damage by 1/2

Adjusted:
- Pets now inherit their owner's spell damage, heal amount, critical spell damage and critical healing on procs\spells, split evenly between all (non-swarm) pets owned by their owner.
- Pets with 2H weapons equipped no longer equip an offhand.
- Pets use equipped weapon delay instead of standard NPC delay.
```

---

---

## 2024-12-24 00:35 - Entry 1320912696492691486
**Author:** Catapultam

This is also Deployed.

---

---

## 2024-12-23 06:27 - Entry 1320638822970687630
**Author:** Catapultam

Deployed
```
- Shadowknight pets now have their own unique spells
 - Each has (SHD) appended to the spell name
 - New scrolls added to Bazaar spell vendors
 - Vision of Ayonae can help you unmem spells (say 'unmem') if you have a now-uncastable spell memorized.
```

---

---

## 2024-12-22 23:53 - Entry 1320539762389422122
**Author:** Aporia

Deployed

```
- Paladin AA Blessing of Life Rk 2 and 3 now available for an increased base heal amount and proc rate.
- Paladin AA Healing Light Rk 2 and 3 now available for an increased proc rate (up to 30%)
```

Deployed
```
All single target Paladin stun spells now have a small damage component to proc Sympathetic Strike.
```

---

---

## 2024-12-22 05:36 - Entry 1320263658823221339
**Author:** Catapultam

Small WIP Changelog...
```
- Reworked Clockwork Banker & Resupply Agent Tools
 - No longer uses a pet slot
 - Summoned for 15 minutes or until owner leaves the zone
 - Can only summon one of each type at a time
```

---

---

## 2024-12-20 19:41 - Entry 1319751613853859863
**Author:** Catapultam

Consolidated Changelog
```
- Unattuner works again
- Added 10 titles for prolific Gamblers.
- Added title for owning a Vial of Prismatic Dye
- Glamour-Stones now have teal names.
- Guild Names and permissions should now propagate to all zone servers correctly.
- Additional perfomance improvements around Bard Songs.
- Pets which you cannot cast no longer survive your death (the same as buffs).


 - Creatures all across Norrath, Luclin, and the Planes have come into possession of Strangely Wrapped Gifts
 - Strange Elves from beyond this world have appeared in the Bazaar and EC Tunnel, seeking these gifts.
 - Do you open them? Or return them?

```

---

---

## 2024-12-16 17:04 - Entry 1318262438977736856
**Author:** Catapultam

ROLLING DEPLOYMENT (Will be inconsistent which zones this works on until next reboot. Do not expect bazaar to be effected)
```
- Unattuner should now function again
```

---

---

## 2024-12-16 15:23 - Entry 1318237038197342208
**Author:** Catapultam

```
- Glamour-Stones now have teal names.
- Added `missingspells` argument to `/outputfile`. Use like `/outputfile missingspells [filename]` (where `filename` is optional) to output a level-sorted list of spells to a file in your EQ directory. File name defaults to `<character>-MissingSpells.txt`. (Thanks @dannuic)
```

---

---

## 2024-12-14 20:31 - Entry 1317589922177093672
**Author:** Catapultam

```
- Added title for owning a Vial of Prismatic Dye
```

---

---

## 2024-12-14 19:49 - Entry 1317579139951235225
**Author:** Catapultam

DEPLOYED
```
- Added 10 titles for prolific Gamblers.
```

---

---

## 2024-12-14 15:08 - Entry 1317508462522925087
**Author:** Catapultam

12/14/24

Bug Fixes
```
- Implemented experimental change to fix the 'no cast bar' bug. This MAY reintroduce a worse bug, but looks good in brief testing. Please report any instances of randomly not being able to cast or perform certain other activities.
- All starting AA now cost 0 points; this may cause your current 'spent' AA total to decrease when it is next updated.
- Significantly reduced the complexity of checking for bard song auto-refresh
- Poisons are no longer equippable.
- Removed several remaining class checks on epics.
```

New Features
```
- The Purveyor of Glamour will create Glamour-Stones (Transmog Ornaments) for Armor!
  - NOT Hero's Forge.
  - Works with modern & legacy player models
  - 5Kpp + sacrificial item
  - Not Dyable

- Removed tradeskill recipe for Vial of Prismatic Dye
- Added Vial of Prismatic Dye to Augs merchant in Bazaar
- Adjusted Vial of Prismatic Dye pricing (Sell from vendor @ 50k, Buy from vendor @ 100p)

- The Purveyor of Glamour will now create 'Hero's Forge' style Armor Glamour-Stones!
  - Generated through 'custom work' randomization system
  - 2 EoM each, tradable.

- The Vision of Ayonae can now reset your AA!
  - Each character gets one free reset
  - Subsequent resets cost 10 EoM and incur a stacking 7 day cooldown (identical to dropping a class)

- Added Petamorph Wands: Wrulon, Phoenix (Red, Blue), Telmira, Stoneworker, Giant Ant, Gorilla, Crushbone Orc, Lightning Dervish, Lava Dervish, Stone Dervish
- Pets will spawn using the appearance of any equipped Petamorph Wands
```

The Vial of Prismatic Dye changes are likely going to be something that many people disagree with. We are choosing the take a different experience for armor appearance customization on this server vs official or other emulated servers. I feel that armor dyes are a 'quick and dirty' solution that allows getting whatever appearance you want quickly and easily, and removes a lot of the fun in finding the exact combination of gear to achieve the look you want. Transmog accomplishes this better, and serves as a plat sink that we definitely need. However, I am leaving Dyes in-game, for those who do want to use that shortcut, with an additional plat sink component.


Additionally, for those who do not want to deal with Heros' Forge armor appearances, please remember they can be disabled in the Options menu.

---

---

## 2024-12-12 01:06 - Entry 1316571786611261500
**Author:** Catapultam

Consolidated Changelog

```
- Corrected Veterancy scaling formula to correctly function near the end of the scaling range
- Fixed SE_GiveDoubleRiposte (Knave's Return Stab, Furious Refrain, Return Kick, etc)
- Probably fixed UCS problems again (thanks @Akk)
- Removing a class no longer removes spells you can still use due to other classes
- Removing a class unequips items which are no longer usable
- Removed Class Requirements from all epic quests (Thanks @Prymetyme)
```

Rolling Deploy (Requires new zone server; new DZ does not guarantee this)
```
- Detrimental Sympathetic procs should no longer target their caster under any circumstance
```

---

---

## 2024-12-11 16:18 - Entry 1316438968958455849
**Author:** Catapultam

```
- Removed Class Requirements from all epic quests (Thanks @Prymetyme)
```

---

---

## 2024-12-11 05:44 - Entry 1316279399741657161
**Author:** Catapultam

Rolling Deploy (Requires new zone server; new DZ does not guarantee this)
```
- Fixed SE_GiveDoubleRiposte (Knave's Return Stab, Furious Refrain, Return Kick, etc)
- Probably fixed UCS problems again (thanks @Akk)
- Removing a class no longer removes spells you can still use due to other classes
- Removing a class unequips items which are no longer usable
```

---

---

## 2024-12-09 01:42 - Entry 1315493798641401887
**Author:** Catapultam

Rolling Deploy (Requires new zone server; new DZ does not guarantee this)
```
- Corrected Veterancy scaling formula to correctly function near the end of the scaling range
```

---

---

## 2024-12-08 23:07 - Entry 1315454822505517128
**Author:** Catapultam

Hotfix
```
- Reduced maximum veterancy bonus from 5x to 3x AAEXP
```

This impact of the change allowing Veterancy to apply AFTER the per-kill cap was significantly greater than appeared in testing. This change will still result in overall higher AAEXP rates than prior to the most recent patch.

---

---

## 2024-12-08 16:19 - Entry 1315352052188184646
**Author:** Catapultam

Deployed
```
Quests
- Revamp of 'Thieves Aboard the Ship' event (Thanks @Trust)
- Plane of Sky keys are no longer removed from inventory when leaving the zone (Thanks @Trust)

Bug Fixes
- Apply MeleeLifeTap to Archery damage
- Temporary Stun Immunity after being stunned now correctly applies to non-spell stuns.
- Flags should be consistent between different zones.
- Worn ATK is no longer double-counted under certain circumstances.

Misc
- Bonus AAEXP from Veterancy will now give feedback indicating when the bonus will end.
- Bonus AAEXP from Veterancy is now applied after the per-kill AAEXP cap.
- Revamped Healing messages
- Revamped Rune messages
```

---

---

## 2024-12-08 02:50 - Entry 1315148539457703938
**Author:** Aporia

Deployed:

```
- Extended Ingenuity AA has been enabled for Bards
- Bladed Song is now unresistable and has had a second rank added.
- Dance of Blades, Bladewhirl Proc now has a -100 chromatic check on landing. It's AC shred and resist debuff now scales with level.
- Funeral Dirge now increases physical damage taken by 10/15/20% and has had its duration doubled
- Hastened Funeral Dirge AA is now available (5 Rks) putting Funeral Dirge down to 10 minutes at max level
- Song of Stone has had its pet stats increased significantly and its cooldown reduced significantly

These changes were made to reinforce the support nature of the Bard and its viability across multiple builds.

Thank you for your patience as we continue to try navigate player feedback!
```

---

---

## 2024-12-07 06:26 - Entry 1314840330230566975
**Author:** Catapultam

Rolling Deployment (Will show up in zones other than the bazaar as time goes on, after reboot will be effective everywhere)
```
- Adjusted spell damage messages to show spell, and pet owners.
- Adjusted DoT damage messages to be normal non-melee hits
- Potentially fixed Explorer path progression quests not unlocking flags reliabily
```

---

---

## 2024-12-07 03:56 - Entry 1314802696938586153
**Author:** Catapultam

Deployed (Client Patch)
```
- ACTUALLY FIXED NOCLIP OBJECTS (Thanks @Bakemono for enormous troubleshooting help)
```

---

---

## 2024-12-06 03:00 - Entry 1314426106375573516
**Author:** Catapultam

Deployed (-ish)
```
- Fixed 'Spells are 255 until you zone once'
- Possibly fixed some pets poofing on server-down (Sorry, it won't work on the next server-down, probably)
- Disc timers are no longer transferred to new characters when you camp to character select and switch toons
- Spell Procs added by buffs must be unique
- Potentially fixed client memory leak causing collidable objects to no longer be collidable
```

---

---

## 2024-12-05 07:17 - Entry 1314128377191465030
**Author:** Catapultam

Deployed
```
- Fix for crash-on-zone for some clients
```

---

---

## 2024-12-03 17:39 - Entry 1313560375739941017
**Author:** Catapultam

12/3/24

Pending Reboot & Patch
```
- Corrected Hoshkar AoE to apply a sane slow effect, instead of a negative attack speed
- Para Dar's Slow AoE is now curable.
- Corpse decay time will never be longer than the respawn time of the mob.
- Hunter's Fury should no longer block Trueshot Discipline
```

---

---

## 2024-12-02 22:53 - Entry 1313276869738631230
**Author:** Catapultam

```
(Quests, Deployed)
- Re-enabled 'Slayer Titles'
- Various fixes to Toirgan Mines scripts
- Various quest and script fixes
- Various quests and script fixes
```

---

---

## 2024-12-02 14:00 - Entry 1313142732813766719
**Author:** Catapultam

Deployed
```
- Experimental fix for those crashing on logging\zoning into the Bazaar
```

---

---

## 2024-12-02 00:03 - Entry 1312932176060223628
**Author:** Catapultam

Deployed
```
- Combat Skill activation should no longer impose a 1-second cooldown on other skills.
- Adjusted Map targeting range again
- Doubled Tracking\Situational Awareness range for mobs that you have LoS on
- Cleaned up parsed spell information for SPA relevant to Sympathetic Healing
(If you are interested in helping to clean up the spell parser in general, and are comfortable working with C-Strings, hit me up! There's a pile of EOM)
```

---

---

## 2024-12-01 05:03 - Entry 1312645296576135229
**Author:** Aporia

```
Rejoice.
- /friend works correctly again

Rejoice harder.
- /ignore works correctly again

(Thanks Akk!)
```

---

---

## 2024-12-01 03:27 - Entry 1312621082380992636
**Author:** Aporia

```
Option added to Omat Vastsea's quest script to summon back Natasha to make it easier for players who ran into issues during the Cleric epic to fix their quest state.

By saying "I wish to see Natasha", you can trigger a spawn of Natasha. Who is now immune to player damage.

Thank you Grig
```

---

---

## 2024-11-30 18:05 - Entry 1312479580904362005
**Author:** Catapultam

Deployed
```
(Client Update, DEPLOYED)
- Experimental Fix for 'You can't use that command right now...` while spamming Disciplines
- Even Better fix for 'You can't use that command right now...` while spamming Disciplines
- Doubled Target Range on Map.
- Improved Map performance.

(Server Update, DEPLOYED)
- Prevent slow effects from causing uninitialized skill timers to be set to ~80 years in the future
- Situational Awareness AA adjusted to provide effective skill instead of actual 'skill points'.
- Haste now displays on a scale starting at 0%.
- Haste is no longer over-applied to activated Melee skills (Kick, Bash, Backstab, Frenzy, etc).
- Moved several previously unfilterable combat messages (Master Wu, Strikethrough, Stun) to Skills chat-window filter. Options filter window is unchanged.
- Dispel should no longer trigger a lag spike for some players.
- Pets will prioritize equipping items in their primary and secondary slots ahead of any other slots.

(Quests, DEPLOYED)
- The Polymorphist will now allow you to change Deity.
- The Polymorphist will now allow you to 'reset' a pet name, so a new random static will be generated the next time you summon that pet type.
- Solomen will now respond to his linked prompt.
- Tomekeeper Dahl will no longer eat items turned in by non-Monks.
- Deep will no longer eat items turned in by non-Monks
```

---

---

## 2024-11-30 00:14 - Entry 1312210013049061387
**Author:** Aporia

```
- Scale armor and other chain like armor with missing graphics should now be fixed
- Hastened Celestial hammer has had its pre-requisites removed
- Many AA descriptions updated (thank you Alebrije)
- Misc quest fixes
- Echo added to Kaesora
- The Tangrin respawn time reduced
- Account actions taken around custom Macro Quest sources.
- Turkeys are no longer lore, but are now no-drop
- Pumpkin Spice Latte is now no-drop
- Turkeys and Pumpkin Spiced Lattes now have a rare chance to drop from enemies until Sunday night
- Echo added to Highpass (I couldn't trust rogues to play nice...)
- Quest EXP temporarily disabled
```

---

---

## 2024-11-28 05:24 - Entry 1311563335329779764
**Author:** Aporia

Pending Reboot/Patch:

```
- Vessel Drozlin respawn lowered to 1hr.
- Hastened Celestial Hammer AA adjusted and re-enabled.
- Rogue/Monk Strikethrough AA display bug fixed
- Echo added to OoT
- Echo added to Droga
- Echo added to Nurga
- A Mischievous Halfling now has Thanksgiving food and drink!
```

---

---

## 2024-11-27 08:39 - Entry 1311249916022100048
**Author:** Catapultam

Deployed
```
Client Plugin:
- Fixed client memory leak in map
- Targeting mobs from map is limited distance (50 units) or Line of Sight.
- /mapfilter custom will only show mobs you can see the names of
- You now use the highest tracking skill of anyone in your group to evaluate mobs-on-map name visibility

Epics:
- Added 2H versions of Innoruuk's Curse and Fiery Avenger.
- Added 'Change Stance' click effect on Innoruuk's Curse and Fiery Avenger to shift between 1H and 2H forms.
```

---

---

## 2024-11-25 19:42 - Entry 1310692059795034183
**Author:** Aporia

```
- Echo added for Lake Rathe
- Crag spiders look less human and more spider|
- More LoY items tuned down to be between Kunark and Velious loot
```

---

---

## 2024-11-25 17:02 - Entry 1310651946822013050
**Author:** Catapultam

Deployed (Client Patch)
```
- Increased zoom-out distance (thanks @iamclint)
- Implemented /fov command to adjust field-of-view; 45 (default) - 90 (thanks @iamclint)
- Potentially fixed Crash-on-Zone into certain zones such as HateplaneB and Bazaar
```

---

---

## 2024-11-25 03:34 - Entry 1310448565931474955
**Author:** Aporia

Deployed
```
- Several instantly spawnable quest NPCs are no longer attackable.
- Cleric epic returned to primary only. This is a tradeoff for having the same proc as the level 50 summoned hammer
- Berserker epic had stats rebalanced for Kunark/Velious era.
- Fixed edge cases where group heals wouldn't heal pets.
- Echo for Chardok moved inside of Chardok
- Echo added for Warslik Woods
- Echo added for Burning Wood
- Echo added for Lake of Ill Omen - Echo added for Overthere
- Echo added for South Karana
- Respawn time reduced on a sleeping ogre
- Respawn time reduced on Verina Tomb
```

---

---

## 2024-11-23 00:36 - Entry 1309678834458562560
**Author:** Catapultam

Deploying
```
- Corrected logical error preventing Base Crit Damage Ratio from applying
- Temporarily disabled 1x/char AA reset on Vision of Aayonae.
```

---

---

## 2024-11-22 18:15 - Entry 1309582982549602315
**Author:** Catapultam

Deployed
```

- Adjusted SPA 294 (SE_CriticalSpellChance) to no longer stack its critical damage modifier, as originally intended)
- Adjusted AA "Destructive Fury" to use SPA 155 (SE_SpellCritDmgIncrease) to increase critical damage directly.
- Added AA "Destructive Fury" to Wizards
- Adjusted AA "Arcane Destructive Fury to use SPA 155 (SE_SpellCritDmgIncrease) to increase critical damage directly.
- Reduced Crit Damage Bonus from "Arcane Destructive Fury" to 10% per rank
- Adjusted Spell "Improved Familiar" to use SPA 155 (SE_SpellCritDmgIncrease) to increase critical damage directly.
- Adjusted Spell "Spirit of the Black Wolf" to use SPA 155 (SE_SpellCritDmgIncrease) to increase critical damage directly.

- Implemented 1x/char AA reset on Vision of Aayonae.
- Implemented 1x/char free class change on Vision of Aayonae.

- Fixed error preventing Melee Damage Bonus spell effects from working.
- Being over-cap on unused AA no longer results in AA loss, only the inability to earn additional AA
- SE_MeleeLifetap now works with Ranged and Throwing attacks

- All Expedition locks have been reset.
```

---

---

## 2024-11-20 22:18 - Entry 1308919463030165574
**Author:** Aporia

Implemented:
```
- Many AA descriptions have been updated to provide more information (thank you Alebrije!)
- Bard aggro from songs has had its aggro reduced to 25% of its former cap.
- Extended EXP bonus turned off.
- Grand Master Lozz no longer speaks of Apocryphal things.
- Kurn's Tower DZ no longer drops you in the middle of the zone (lol sorry)

```

Pending Patch/Reboot:
```
- Wizard AA Improved Familiar now correctly summons a drake instead of a baby skeleton on rank 3 and 4
- Form of the Black wolf illusion now matches Spirit of the Black Wolf duration.
- ENC AA Mana Draw recast set on spell to match AA to avoid odd CD interactions.
- Several Legendary items missing Heroic stats have been fixed.
- All NPCs with a spawn time of > 1 hour, that don't have their own DZ, and are needed for epic quests have had their spawn time reduced to 1 hour.
- The following starting cities have had these NPCs receive Parcel training!

- Antonica
(West) Freeport: Lindie Rains
Grobb: Grallvek
Halas: Grots
Neriak - Commons: Lynsalai
Oggok: Klob Pulp
Rathe Mountains: Zok Malka
Rivervale: Teelie Meegles
South Qeynos: Ren Pinemyer
Surefall Glade: Grathin Nilm

- Faydwer
AkAnon: Zenrel Ottonoggin
Greater Faydark: Merchant Vaelias
Northern Felwithe: Laernian Caelael
North Kaladim: Marsha Stonepenner

- Odus
The Erudin Palace: Sparlus Penfold
Paineel: Henly Nictropus

- Kunark
East Cabilis: Klok Faziz

- Luclin
Shar Vahl: Laanas Sejiir

- All Soulbinders are now immune to player damage
- Important NPCs in EC tunnel are now immune to player damage
```

We are planning on a reboot tomorrow morning or afternoon to bring live pending and new changes.

Many good things in the works!

---

---

## 2024-11-19 14:34 - Entry 1308440149453049907
**Author:** Aporia

```
- Cazel now always drops his spoon.
- Echo of the Past now available in Kithicor.
- Echo of the Past now available in Rathe Mountains.
- Significantly increased performance in zones over time.
- Sending plat via the parcel is working again! (Thank you Neckkola!)
```

---

---

## 2024-11-18 05:46 - Entry 1307944944706650153
**Author:** Aporia

```
- Pets can once again be summoned in PoSky
- Ranger AA Precision of the Pathfinder description updated.
- Veteran's Wrath AA description, updated.
- Formula changed on Cinda's Charismatic Carillon and negative resist mod added
- Echo's learn to spell better
- Sirran will now accept key items regardless of what island he is on.
- Spiroc Lord will now stay dead if Guardian is dead
- Bags can now be sent through parcel (money still cannot).
```

---

---

## 2024-11-17 15:11 - Entry 1307724713937862677
**Author:** Catapultam

```
- Pet illusion wands should work as expected. You may need to resummon any necro pets.```

---

---

## 2024-11-16 19:54 - Entry 1307433633753202742
**Author:** Aporia

Pending reboot/patch
```
- Monk AA Grappling Strike description corrected.
- Monk AA Destructive Force should now work correctly.
- Putrid Skeletons once again drop Putride Rib Bone for Monk Sash quest
- Cazic Quill and Jagged Diamond Dagger can now be quested above their base version
- Many misc item fixes
- Highpass safe location no longer puts you outside the map (fixes evac in zone).
- Wizard AA Cryomancy and Pyromancy buffs should now stack. Only one can trigger at a time.
- Malka Rale should now spawn more often for Rogue Epic
- Monk AA Way of Steel description corrected.
- Greenmist SK armor has been added back to loot tables in PoFear.
- Druid AA Nature's Guardian HP and AC increased.
- Denise Songweaver in PoSky now expects the correct items for the Bard Test of Tone
- Warrior AA Battle Leap description corrected
- Grandmaster H'Qilm has had their spawn rate increased to match the rest of Hate named.
- All Echo of the Past are now immune to all player damage.
```

---

---

## 2024-11-15 18:06 - Entry 1307044028734378104
**Author:** Catapultam

Pending
```
- Fix crash related to additional loot
```

---

---

## 2024-11-15 05:29 - Entry 1306853645442224129
**Author:** Catapultam

Deployed
```
- Attempt to fix pet illusion targeting (Cannot duplicate on test, theoretical edge case fix)

- Group Incentive Program
 - In the interest of promoting sharing instances for the health of server resources...
 - Respawning Instances are now subject to the same scaling rules as Non-Respawning instances (3+ players adds to mob difficulty)
 - For each expedition member past the second;
   - 25% stronger mobs
   - 25% more XP
   - 25% more AAXP
   - 25% more item Exp
   - 25% chance for each mob to drop an additional set of loot
   - increased chance of legendary rolls
```

---

---

## 2024-11-14 17:00 - Entry 1306665076367036507
**Author:** Catapultam

Deployed
```
- Update to EQEmu v22.59.1
- Fix invisible mobs (Thanks @Akkadius - you are the real MVP!)
- Sweaty Bird Farmers rejoice - ported WFH Spiroc Island script (Thanks @Trust)
- Added Secondary usability to Thornstinger
```

---

---

## 2024-11-13 23:00 - Entry 1306393344519442453
**Author:** Catapultam

Deployed
```
- ZEM normalized to 2.0 for zones with ZEM below 2.0
```

---

---

## 2024-11-12 20:32 - Entry 1305993720575037471
**Author:** Catapultam

Deployed
```
- Pets survive death again (frfr)
- Parcel purchases work again
```

---

---

## 2024-11-12 14:53 - Entry 1305908449619607663
**Author:** Aporia

Deployed:
```
- Noble Dojorn and Overseer of Air now correctly drop Efreeti War Maul
- Bryn Fynndel now correctly accepts the Shadow Coded Book
- Geometry updated across many zones to fix mobs falling through the world ie Fear - Thank you Trust!
- The frequency of charm pets breaking and aggroing other mobs reduced (faction wars)
- Players now informed why they can't pull a dz when they aren't the leader (because they aren't the leader)
- Charm can *actually* be refreshed in combat now
- Sanguine Mind Crystal and Azure Mind Crystal now behave well with implied targeting
- Mojax can no longer spawn infinite Duggin Scumbers
- Previously non-resizable windows are now resizable by default
- Glidara Myllar now accepts Warning to Glidara
```

Pending Patch/Reboot:
```
- Warrior AA Gut Punch description fixed
- Certain items that had incorrect stats for their legendary versions have been fixed
- Cleric AA Turn Undead description fixed
```

---

---

## 2024-11-11 04:47 - Entry 1305393437985734676
**Author:** Catapultam

Deployed
```
- Disabled Anti-AFK script in the Bazaar
- Fixed Ride-Along bazaar and back targets
- Charm spells should no longer inappropriately redirect as implied targets.
- ZEM is applied to per-kill aaxp cap
```

---

---

## 2024-11-10 20:39 - Entry 1305270536628338759
**Author:** Catapultam

Deployed 11/10/24
```
- Additional fixes for 'Invisible Mobs' issue
- Deployed sharding system for Bazaar (Thanks @Akkadius)
- Misc unstream fixes

- Windstriker has had its proc changed to Lightning Bolt
- Rain Caller has had its click removed and replaced with the same spell (Firestrike) as a proc
```

Notable Known Issues
```
- Using the 'ride along' feature of Bazaar and Back for a group member with a different target zone will result in undefined behavior
```

---

---

## 2024-11-10 01:21 - Entry 1304979313254207538
**Author:** Catapultam

Hotfix 11/8/24  - This requires a fresh zone server until reboot, so only zones which have been closed for 5 mins or longer.
```
- Attempt to fix 'Invisible Mobs' issue
```

Deployed 11/9/24
```
- Tearal and Son of Tearal can now attune your Bazaar and Back ability to either Bazaar or East Commonlands, respectively.
- Plane of Sky scripts should all work now.
```

---

---

## 2024-11-09 03:25 - Entry 1304647984100806717
**Author:** Catapultam

Hotfix 11/8/24 - This requires a fresh zone server until reboot, so only zones which have been closed for 5 mins or longer.
```
- Attempt to fix pet buffs causing periodic frame skips for some users
```

Deployed 11/9/24
```
- Respawning instance lockout lowered to 2 hours.
- Mobs with respawn times longer than 2 hours will not spawn inside Respawning instances.
- Lowered Non-respawning instance lockout to 16 hours.
```

---

---

## 2024-11-07 02:01 - Entry 1303902189189857281
**Author:** Catapultam

Deployed 11/7/24
```
- Added Disenchanted Bags
- Charm pets will not clear inventory on refreshing charm
- Fixed clicking off pet buffs
- Shrink\Grow works on pets
- Rabid Bear moved to song window
- Clean up pets on charm break a little better, hopefully resolving intermittent issues with hostile npc seeming to be a friendly
- Marl Kastane should spawn for Shadowknights who need him upon entering Kerra Ridge
- Removed Deity from all items
- Adjusted negative stats on edge case upgraded items
- Pets & Suspended buffs persist through death
- Added more descriptive text to instance offer dialogue
```

---

---

## 2024-11-06 07:17 - Entry 1303619142045143072
**Author:** Catapultam

Deployed 11/6/24

```
- Updated to EQEmu v22.57.1
- Mages no longer lose TEMPORARY items when logged off
- More than 4 proc buffs can simultaneously apply (but no more than 4 will proc in any combat round)
- Necromancers get full damage from Vampiric Embrace
- Dragons are no longer tiny
- Crocodiles are no longer huge
- Spoot remains an asshole
- Shrink and Grow, except specifically pet-targeted, no longer affects NPCs or Pets.
- Echo of Luck works correctly for quest turn-ins.
- Charm can be refreshed?
```

---

---

## 2024-11-06 01:24 - Entry 1303530351636774976
**Author:** Aporia

```
- Oracle of K`arnon respawn lowered to 1 hour with a 30 minute variance.
- Sir Lucan D`Lere respawn lowered to 1 hour with a 30 minute variance.
- Marl Kastane respawn lowered to 1 hour with a 30 minute variance.
- Lost Iksar quest text now makes sense.
- Cryomancy and Pyromancy description now correctly reflects that it can be used on spells below level 60.
- Bosses once again correctly spawn inside of non-respawning instances
- Geometry updated for several problematic zones (thanks Trust!)
- Black Block of Ore no longer looks like a book
- Druid spell Protection of Rock now correctly scales again
- Enchanter spell Weakness now correctly stronger than Insipid Weakness
- Necro AA Death Bloom had its health cost and mana regen halved per tick
- Shaman AA Spiritual Blessing is now marked as non dispellable
- Bard AA Funeral Dirge can no longer be resisted
- Warrior AA Warlord’s Resurgence has had its description corrected
- Enchanter spell Boon of the Clear Mind is now correctly tuned between C1 and C2
- EoM Haste once again grants haste V1 and is now correctly applying
- Echo for hate removed from Oasis
- Apothic Kilt (Legendar) now gives correct stats
- Echo for Runnyeye now works correctly
- Echo added to Cazic Thule
- BST AA Gelid Rending can now proc with any weapon
- Cazic Thule no longer despawns under certain unintended conditions
```

Some of these are live, some of these are pending. Trying to iterate quickly to get all your reports addressed.

For a little background, things like this are not necessarily fixed in order of importance- beyond server stability and playability, every report is important.

So, when we have small amounts of time or limited capacity, we bite off little things.

Rest assured, our OCD will guarantee every report gets looked at 🙂

---

---

## 2024-11-05 19:36 - Entry 1303442945671692420
**Author:** Catapultam

@here

```
- Fixed zone crashes
```

---

---

## 2024-11-05 18:15 - Entry 1303422359621079101
**Author:** Catapultam

Deployed
```
- New global buff system (Thanks @Secrets)
- Fishing can result in Enchanted and Legendary items
```

---

---

## 2024-11-04 15:11 - Entry 1303013816132440124
**Author:** Catapultam

Immediate effect
```
- Reduced Exp from Spirocs in Plane of Sky
- Terror, Fear, Dread, and Dracoliche no longer spawn in respawning Plane of Fear instances
- Respawning Instances now have the same lockout DURATION as Static instances

- Parcel purchase from /baz window is now free.
```

---

---

## 2024-11-03 19:05 - Entry 1302710373446586460
**Author:** Catapultam

Pending
```
- Characters who are Rangers will display their Bow as their default weapon instead of their melee weapons.
- Discovery of Enchanted items will no longer trigger a world announcement.
```

---

---

## 2024-11-03 19:05 - Entry 1302710180533899408
**Author:** Catapultam

Deployed over last two days, sorry has been crazy;
```
- Updated Gambling Halfling text
- Cryomancy and and Pyromancy are no longer level restricted
- Bow Mastery fixed frfr
- Mobs should flee when feared now
- Charm spells should overwrite any other Charm spell cast by the same caster on the same mob.
- Adjusted item experience gain
  - clamped exp gain based on tier
  - adjusted exp gain calculation

- Fixed crash related to activating AAs while in a group
- Way of Steel should now display correctly to all monk combos (please remember to patch).
- Halfling Rogue GM text corrected.
- Incorrectly scaled legendary items fixed (improved).
- Certain unusable poison crafting components removed from Bazaar vendor.
- Berserker starting weapon now *actually* a 2hander.
- Compensating measure implemented for bugged starting quests. If you have a bugged starting quest from last night, please remove the quest, relog, go to the fading memory in bazaar, and say "note", then proceed with the quest.
- EoM buffs disappearing under certain circumstances has been resolved.
- Item leveling appearing to pause at certain points has been resolved.
- Fixed crash related to moving bag contents

- Fixed memory leak related to loading AA information
```

Known major issues
```
- Item leveling does not work as anticipated via kill-exp. Consuming does work as expected.
- Bazaar is VERY slow when local population over 100
```

---

---

## 2024-11-02 17:20 - Entry 1302321345014534207
**Author:** Catapultam

Pending on fresh zone servers
```
- Fixed crash related to moving bag contents
```

---

---

## 2024-11-02 15:20 - Entry 1302291165894152242
**Author:** Aporia

Deployed

```
- Way of Steel should now display correctly to all monk combos (please remember to patch).
- Halfling Rogue GM text corrected.
- Incorrectly scaled legendary items fixed (improved).
- Certain unusable poison crafting components removed from Bazaar vendor.
- Berserker starting weapon now *actually* a 2hander.
- Compensating measure implemented for bugged starting quests. If you have a bugged starting quest from last night, please remove the quest, relog, go to the fading memory in bazaar, and say "note", then proceed with the quest.
- EoM buffs disappearing under certain circumstances has been resolved.
- Item leveling appearing to pause at certain points has been resolved.
```

---

---

## 2024-11-02 15:04 - Entry 1302287329112756244
**Author:** Catapultam

Pending
```
- Updated Gambling Halfling text
- Cryomancy and and Pyromancy are no longer level restricted
- Bow Mastery fixed frfr
- Mobs should flee when feared now
- Charm spells should overwrite any other Charm spell cast by the same caster on the same mob.
- Adjusted item experience gain
  - clamped exp gain based on tier
  - adjusted exp gain calculation

- Fixed crash related to activating AAs while in a group
```

---

---

## 2024-11-01 23:10 - Entry 1302047213064683530
**Author:** Catapultam

Deployed 11/1/24.

Welcome to Release.

```
- Added #tim (Toggle Improved Models). Use this command to disable upgraded NPC models if you hate fun.
- Non-Bards can no longer interrupt spell casting by clicking the gem multiple times.

Class Removal
- Vision of Ayonae now requires EoM to remove a class, and has a 7-day initial cooldown. This cooldown will increase by 7 days, permanently, each time it is used on a character.
- When removing a class, invalid skills are also removed.

Abilities
- Improved Frenzy damage scaling based on Primary Weapon
- Improved damage from Way of Steel
- Druid AA Nature's Guardian has had its CD reduced for ranks 5 and 6.
- Ranger AA Bow Mastery works as intended again.
- Lifetap spells can once again crit heal

Misc
- Re-Introduced and fixed 'Hunter' titles
- Item Discovery Broadcasts should filter under 'Experience Messages'
- Custom bazaar NPCs can no longer be mistakenly attacked.
- Fear now causes NPCs to flee again
- Megosh Thistlethorn is back in game but with OoE scripts stripped
- Some quests have had their components/items made lore again.
```

---

---

## 2024-10-31 17:09 - Entry 1301593922492956733
**Author:** Catapultam

Deployed

```
- Removing class correctly removes spells
- AAXP settings preserved on zone
- Project Illusion works on all pets
- EoM cost reduced from 5 to 2 for The Mischievous Halfling and the Purveyor of Glamour.
- Death tip now correctly reflects gameplay on THJ.
- New friends added to the campfire.
- Updated website.
- Dragon Trigger in Skyfire no longer incorrectly attacks players
- AA cap for white mobs increased to 6%
- AA scale blue, light blue, and green mobs slightly increased
- Fixes for memory leaks around item improvement and pets
```

---

---

## 2024-10-30 19:55 - Entry 1301273391797506099
**Author:** Aporia

Deployed
```
- EoM cost reduced from 5 to 2 for The Mischievous Halfling and the Purveyor of Glamour.
- Death tip now correctly reflects gameplay on THJ.
- New friends added to the campfire.
- Updated website.
- Dragon Trigger in Skyfire no longer incorrectly attacks players
- AA cap for white mobs increased to 6%
- AA scale blue, light blue, and green mobs slightly increased
```

---

---

## 2024-10-30 18:44 - Entry 1301255542051831931
**Author:** Catapultam

Pending
```
- Removing class correctly removes spells
- AAXP settings preserved on zone
- Project Illusion works on all pets
```

---

---

## 2024-10-29 21:10 - Entry 1300929901423231056
**Author:** Catapultam

Deployed
```
- Fixed some NPC quest text
- Fixed charm breaks
- Fixed Way of Steel (Nerfed Monks)
- Added additional starting port locations
- Charm spells can be refreshed
- Reduced some annoying noises (REMOVED)
- Autofire\throw can be used while casting bard songs
- Guild Management Window now shows correct classes
- Lifetaps can once again critically heal
```

---

---

## 2024-10-28 23:43 - Entry 1300605985504624640
**Author:** Catapultam

Deployed
```
- Implemented per-kill AAEXP cap which is informed by: con of mob, level of player. Exp Rate buffs increase this cap.
- Decreased amount of exp needed to improve items to (Enchanted)
- Pet inventory and buffs no longer fade on zone
- Marsingers 3\4 require Kunark to be unlocked
- Removing classes should now correctly store changes to player profile
- Echo of the Brood now has a small spell haste component
- All auto granted starting AA now have an AA cost of 0 to allow players to progress total AA count at the same rate.
- Cleric now starts with Purify Soul AA instead of Twincast AA
- Purify Soul is now a 15 minute CD
- Druid now starts with Entrap instead of Paralytic Spores
- Druid and Necromancer no longer start with Critical Affliction AA
- Druid, Necromancer, Enchanter, and Shaman now begin with an innate 3% chance to crit with DoTs
- Enchanter and Shaman now also start with the Destructive Cascade AA
- Shooting a bow/throwing things now levels Offense (thank you Carolus)
- Spell crit chance and bonus now stack correctly (thank you Grek)
- Players no longer autojoin deprecated channels. General, OOC, and AUC are now the preferred global channels (thank you Trust)
- Support, Bug, and LFG channels are now available to new players that join Discord by default
- Warrior and Berserker starting quest item adjusted.
- Bard Discipline Deftdance has had its base CD reduced and now has Hastened AA available
- Updated Consume Item AA description
```

---

---

## 2024-10-27 18:52 - Entry 1300170230915534848
**Author:** Aporia

Deployed
```
- All auto granted starting AA now have an AA cost of 0 to allow players to progress total AA count at the same rate.
- Cleric now starts with Purify Soul AA instead of Twincast AA
- Purify Soul is now a 15 minute CD
- Druid now starts with Entrap instead of Paralytic Spores
- Druid and Necromancer no longer start with Critical Affliction AA
- Druid, Necromancer, Enchanter, and Shaman now begin with an innate 3% chance to crit with DoTs
- Enchanter and Shaman now also start with the Destructive Cascade AA
- Shooting a bow/throwing things now levels Offense (thank you Carolus)
- Spell crit chance and bonus now stack correctly (thank you Grek)
- Players no longer autojoin deprecated channels. General, OOC, and AUC are now the preferred global channels (thank you Trust)
- Support, Bug, and LFG channels are now available to new players that join Discord by default
- Warrior and Berserker starting quest item adjusted.
- Bard Discipline Deftdance has had its base CD reduced and now has Hastened AA available
- Updated Consume Item AA description
```

---

---

## 2024-10-26 05:45 - Entry 1299609834563440670
**Author:** Aporia

Deployed

```
- Assassinate can now trigger at level 50
- Buffs that effect spell critical damage should now stack
- Hitting level 50 will now automatically grant one class AA
- Main task updated to require level 50 instead of 51
- Weirdness fixed around Echo of the Brood server buff
- Dreadlands Echo is no longer... in places other than Dreadlands <_<
- Fists of Steel renamed to Way of Steel. Way of Steel procs off kicks/strikes and also increases the damage of kicks and strikes the same way Fists of Steel increased h2h damage. Way of Steel does not increase h2h damage.
```

---

---

## 2024-10-24 18:17 - Entry 1299074291568082975
**Author:** Catapultam

working log; all pending
```
- Added a short lockout to Respawning instances (1 hour)
- Added Hand of the Gods proc to cleric epic
- Power Source item improvement rate calculation is now always based on the top-tier version of the item, then scaled down for lower tiers.
- Fixed Rage Volley casting animation
- Discs now correctly start their timers when activated while casting.
- Fixed spell haste display
- Fixed melee mitigation effect on pets
- Enabled AAEXP at level 1
- Reduced max level during classic to 50
- Echo buffs now scale by level more appropriately.
```

---

---

## 2024-10-24 17:53 - Entry 1299068357512790077
**Author:** Aporia

```
- Frenzied Burnout AA cost reduced to 3/6/9/12/12/12
- Elemental Earth AA no longer exploitable for massive HoT
- NPC Melee Interrupts reduced
- Sarkis Ebonblade now talks to Shadowknights as intended
```

---

---

## 2024-10-23 07:41 - Entry 1298551768585605191
**Author:** Catapultam

```
- Removed all lockouts from respawning instances
- Raid\Flag bosses no longer spawn in respawning instances
- Non-Respawning instances will become more difficult based on the number of players above 2 in an expedition.
- Players may no longer be added to an expedition once the progression flag mob spawns.
```

---

---

## 2024-10-22 17:52 - Entry 1298343309261013104
**Author:** Aporia

Deployed

```
- Many Hate 2.0 and OoE items available in classic have been reduced to bring them in line with progression expectations.
- Many LoY and OoE items available in Kunark have been reduced to bring them in line with progression expectations.
- More AA/Spell description corrections.
- Backstab damage from non-1hp sources has been reduced.
- Corrected map files for Hate, The Hole, Gunthak, Nadox, Veksar, and Sebilis have been added to the patcher.

```

---

---

## 2024-10-19 20:52 - Entry 1297301475860414606
**Author:** Aporia

```
- Pet buffs that include mitigation can no longer be dispelled.
- Blur of Axes base damage increase has been reduced.
- Tearel can now interact with players that are invis/hidden/SoS.
- Prince Selrach Di'zok has had his stun component removed. Blind lasts up to 24 seconds.
- Sneak Attack description fixed.
- RoRZ description fixed.
- Notlav the Scalekeeper no longer spawns.
- Minor VP 1.0 fixes.
- Trickster's Calling reduced to 10s
```
**Important Note:**

Innoruuk in Hate has been changed similarly to the Dragons in VP 2.0.

Loot has been changed to the original (Post Revamp) version 1.5. His difficulty has been reduced in kind. All of his revamped loot can now be worn by any race.

---

---

## 2024-10-16 02:20 - Entry 1295934257541283881
**Author:** Retribution EQ #change-log

```
- Scout Malom now correctly spawns The Spirit of Torment.
```

---

---

## 2024-10-13 20:12 - Entry 1295116943312818217
**Author:** Aporia

```
- Glidara Myllar script fixed.
- Bryn Fynndel script fixed.
- Orc Impaler quest should now be completable.
- Mojax Hikspin script fixed.
- Enchanter slow cast times reduced to match comparable Shaman slow cast times. This effects: Tepid Deeds, Shiftless Deeds, Forlorn Deeds, Dreary Deeds, and Desolate Deeds.
- Echo of the Past added to Crushbone
- Echo of the Past added to Befallen
- Echo of the Past added to Kurn's Tower
- Echo of the Past added to Runnyeye
- Echo of the Past added to The Warrens
- Echo of the Past added to Blackburrow
- Echo of the Past added to Sol A
- Echo of the Past added to Upper Guk
- Monk Disciplines Voiddance and Whirlwind have had their base CD reduced to 28 minutes from 40.
- Echo of the Past for Dreadlands has been moved to its port in spot.

```

**Important Note:**

It has been decided that VP 2.0 launching with Kunark is a poor overall experience for a number of reasons.

VP moving forward will drop 1.0 loot and its bosses will be scaled back to fit in between Kunark progression targets and Velious dragons. They will keep most of their mechanics but the effects and stats have been reduced by about 60%.

This should make it feel like an end game Kunark experience, and with the availability of Enchanted/Legendary gear, still worth doing in era.

The mobs and abilities may be adjusted further.

---

---

## 2024-10-12 22:24 - Entry 1294787699277959189
**Author:** Aporia

Pending Reboot

```
- Waypoint added to Lake Rathe
- Black Insanity and Dark Courage weapons have had their bane damage increased on each version.
- Inscribable Words ground spawn fixed in Nagafen's Lair.
- Spawn location of Avisiris has been corrected.
- Gliblixl Rocktok now sells starter Bard Instruments in the bazaar.
- Philter of Translocation now properly labeled Philter of Major Translocation
```

---

---

## 2024-10-11 18:42 - Entry 1294369641543762014
**Author:** Catapultam

```
- Experimental fix for the noloot\nocast bug
- Misc bug fixes
```

---

---

## 2024-10-09 23:18 - Entry 1293714261134278699
**Author:** Catapultam

```
* Vision of Ayonae added to Bazaar
 - For characters with exactly 1 class, the Vision can add two random classes.
 - For characters with more than 1 class, the Vision can remove a class. This removal has a cost in EOM and a cooldown.
   - Cooldown set to 1 day and EoM cost to 0 for Beta
   - All skills, spells, disciplines, and AA which are unusable after the class drop are deleted.
```

---

---

## 2024-10-09 15:33 - Entry 1293597206405840899
**Author:** Catapultam

```
* Players are immune to stun for a short time after being Stunned
* Increased the amount of allowed movement while casting spells
* Instant-cast Disciplines can be used while casting
* Disciplines with casting time will interrupt spellcasting.
* Fixed pet buffs randomly not working based on resummoning pets, etc
```

---

---

## 2024-10-09 15:13 - Entry 1293592147341082697
**Author:** Retribution EQ #change-log

```
* Lowered Damage on Sympathetic Strike I-III
* Sacrificial Dagger adjusted to Sympathetic Strike II
* Black Tome with Silver Runes adjusted to Sympathetic Strike III

* Twincast will no longer apply to most procs
* Calliav\Prism Skin type runes provide immunity to DS while active, and DS hits do not burn their charges.
```

---

---

## 2024-10-08 22:55 - Entry 1293346133531430913
**Author:** Catapultam

```
* Classes eligible to buy an AA are now listed in the AA Description
* Removed low-level bonus to item leveling, now solely based on con of kill and stats on item
```

---

---

## 2024-10-08 05:05 - Entry 1293076847604535327
**Author:** Catapultam

```
* Item Exp actually takes item stats into account.
* Ranged Attacks can skill up DA\TA
```

---

---

## 2024-10-08 02:28 - Entry 1293037243723939890
**Author:** Catapultam

```
* DD spell cast times reduced to 3 seconds if above 3 seconds, Any time reduced this way added to recast times.
* Cast times on spell inspect window are now correct, and correctly account for Spell Haste.
* Spell Cast bar will still end 'early' when Spell Haste is in effect.
* Archery and Throwing weapons now check Double and Triple Attack skills
* Fixed PBAoE being limited to 4 targets
* Adjusted item leveling so that item stats is weighted over character level
* EoM Exp AND Loot buffs apply to item leveling rate
```

---

---

## 2024-10-06 04:09 - Entry 1292338022649561121
**Author:** Retribution EQ #change-log

```Cabilis, Lake of Ill Omen, Warsliks Woods, Swamp of No Hope, Field of Bone, Kurn's Tower, Shar Vahl, Shadeweaver's Thicket, Hollowshade Moor, and Paludal Caverns are all now available in classic.```

---

---

## 2024-10-06 01:33 - Entry 1292298737808445541
**Author:** Catapultam

```
- Added Tutorial Popups for; Welcome, Buff Suspending, Power Source\Upgraded Items, Sympathetic Procs
- Added two newbie tasks that helps guide the player from level 1->51, introduce key concepts and faciliate Kunark unlock
```

---

---

## 2024-10-02 20:55 - Entry 1291141623316615188
**Author:** Catapultam

```
- Swarm pets created by pets now belong to that pet's owner.
- Items upgraded via power source can no longer trigger Discovery events.
- Items upgrading via power source will no longer gain any significant exp while in a raid.
- #mystats now dumps all pet info at once, regardless of target
- default UI elements for Player and Group windows are now non-resizable, and can be moved more intuitively.
- Pet Commands other than /pet attack and /pet back are issued ONLY to your focused pet (the one which has the pet window)
- Added additional stages to Power Source exp reports.
```

---

---

## 2024-10-01 15:19 - Entry 1290694483100569703
**Author:** Catapultam

```
- Restored vanilla timers to discs
- Discs assigned to multiple classes use original timer IDs
- Discs assigned to individual classes use a class-unique set of timer IDs
```

---

---

## 2024-10-01 07:27 - Entry 1290575831361523777
**Author:** Catapultam

```
- Added support for up to 500 disc timers
- All discs on seperate timers (This will change!)
- Reworked custom skill timers to reduce packet traffic by at least 100x
- Static instances are now generated dynamicly
- All of the above patch
```

---

---

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

## 2024-09-25 00:58 - Entry 1288303500970692668
**Author:** Catapultam

```
* Fixed infinity buff stacking from non-class sources
* Fixed crash bug
* Fixed attune-on-exp bouncing
```

---

---

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

## 2024-09-21 20:22 - Entry 1287147068732997703
**Author:** Catapultam

```
* Only Must-Equip clickies will become attuned when clicking from inventory
* Numerous quest script fixes
* Honey, I shrunk the bats.
```

---

---

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

## 2024-09-17 16:58 - Entry 1285646038744567849
**Author:** Catapultam

```
* Hopefully fixed power source dupe (again again)
* Removed Fury of Magic AA from Hybrids again
```

---

---

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

## 2024-09-15 08:43 - Entry 1284796823336259585
**Author:** Retribution EQ #change-log

```
* Hole door is now 'click to enter' instead of being a literal door
```

---

---

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

## 2024-09-14 22:57 - Entry 1284649224260292678
**Author:** Aporia

```
Hell levels removed for real this time.
```

---

---

## 2024-09-14 22:11 - Entry 1284637798019633182
**Author:** Retribution EQ #change-log

Pending Patch

```
Enchanter AA Phantasmic Reflex has been changed. ALL SPELLS cast by an enchanter, now have a SMALL chance to grant the caster SMALL rune.

Legendary Staff of Writhing and Legendary Ancient Prismatic Staff now have had their proc restored in addition to their click.
```

---

---

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

## 2024-09-05 23:33 - Entry 1281396861147676696
**Author:** Retribution EQ #change-log

```
Spirit of the Howler Pet level increased.
Nature Walker's Behest Pet HP reduced.
Torturing Winds Debuff reduced to 2 minutes from 2 hours.
```

---

---

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

## 2024-08-30 14:44 - Entry 1279089267922178139
**Author:** Retribution EQ #change-log

Effective on reboot:

```
Lockpicking requirement from SSRA doors has been removed.
Key items are still required.
Certain bags have had their capacity slightly increased on RC/Apoc versions
Zerker AA Tireless Sprint now correctly increases movement rank by 10% for RKII and RKIII
Rangers once again have access to the Shield Block AA
Veteran's Wrath AA once again effects all weapon types (certain weapon types were not benefitting from this AA as intended since the normalization- this has been fixed).
Ranger spells Flaming Arrow and Burning Arrow now correctly proc Symp Strikes. Their base damage has been decreased but now act as short DoTs.
Monks now have access to three ranks of the Hastened Destructive Force AA
Monks now have access to four ranks of the Hastened Defensive Poses AA
Gliblixl Rocktok no longer spawns in the Bazaar
```

---

---

## 2024-08-28 23:47 - Entry 1278501238148960351
**Author:** Catapultam

```
- Can consume higher-tier items (reg in PS, consume enchanted).
- attempt to fix pet taunt
```

---

---

## 2024-08-28 05:38 - Entry 1278227086808715314
**Author:** Catapultam

```
Item Experience Rework (Again)
- Using your Power Source slot to progress an item no longer carries an experience penalty.
- Any item which receives experience becomes no-drop immediately.
- Reworked scaling rates;
  - Rates vary based on item tier, con-level of kill, current level, and total stats of the item.
  - Higher con differences = more item progression
  - Lower current level = more item progression
  - Normal -> Enchanted = less progression required
  - Enchanted -> Legendary = MUCH more progression required
  - More total stats = more progression required
 - Re-implemented Consume Item
  - Still maps to the 4x for normal->enchanted, 4/8x for enchanted -> legendary.
  - No-Drop items MAY NOT be consumed (It was this or break the ratio above to prevent cheese).
```

---

---

## 2024-08-26 06:14 - Entry 1277511372816519231
**Author:** Catapultam

```
Reworked Item Experience
- Not sharing a lot here, figure this one out yourselves.
- This one is way better.
- Items become no-drop as soon as you feed them XP.
- Ok, fine. It's con and level based, totally independent of item stats. Relatively easy to get to enchanted, significantly harder to get legendary.
- Harder at higher levels, but you can kill faster, so... evaluate that how you want.
- Removed exact % feedback for leveling rate.
```

---

---

## 2024-08-24 03:33 - Entry 1276746251861229568
**Author:** Catapultam

8/23 - Pending Reboot
```
* Items which gain a click upon being upgraded to Legendary no longer have 0 charges.
* Charmed pets no longer consume a pet slot after charm breaks
* Glyph AAs can no longer be purchased.
* Skill reuse times fixed (finally), Thanks @Carolus
* Familiars no longer spawn a pet.
* Spell Procs (Poison, buffs, AA, etc) work with ranged and throwing attacks
```

---

---

## 2024-08-23 15:40 - Entry 1276566684332851331
**Author:** Catapultam

```
* Autoinventory now skips Power Source and Ammo
* Refromatted /who results
* Updated Description and names of Dire Charm variants to distinguish allowed targets.
* Updates/Fixes to Melee Skill reuse timers
* Knight's Advantage stacks now
```

---

---

## 2024-08-22 18:15 - Entry 1276243407290761216
**Author:** Catapultam

```
* Implemented Client<->Server handshaking. You will be disconnected after a short period of time if you are not using the client modification plugin.
* Implemented improved MQ2 detection.
```

---

---

## 2024-08-22 15:02 - Entry 1276194813896822829
**Author:** Retribution EQ #change-log

```
Effective on reboot, some effective immediately:

- Banded armor can be combined again.
- Every quest in Jaggedpine now gives the correct faction.
- Klandicar now gives the correct faction.
- Phara Dar now heals to full if disengaged and depops his adds.
- Ella Foodcrafter now lets players know she has [two tasks].
- Circlet of the Falinkan quest now requires correct level to complete (kindly down from ally).
```

---

---

## 2024-08-22 08:52 - Entry 1276101765921509417
**Author:** Catapultam

```
* Lots of progress on cleaning up /who. Apparently I don't remember exactly how /rol and /anon work. More to come
```

---

---

## 2024-08-22 05:37 - Entry 1276052667470188625
**Author:** Catapultam

Running changelog for next patch
```
* Items upgraded via Power Source will retain charges.
* Fixed skillcaps problems, including 2HP
* Level 1 Skills set to cap for that level (Except tradeskills, etc). Skills displayed at level 1 are fucked, don't try to make sense of them.
* First point in new skills is automatically assigned at level-up.
* Revert to vanilla stacking logic, hopefully clears up weird song stacking stuff.
* Fixed not being able to trade your pets no-drop items.
* Fixed typos
```

---

---

## 2024-08-21 04:51 - Entry 1275678617942228993
**Author:** Catapultam

Round 2!
```
* Dimensional Armory will selectively equip mage pets.
* Pets can be traded items again
* Fixed invulnerable monks
* FoS limited to H2H again
```

---

---

## 2024-08-21 02:07 - Entry 1275637372138295417
**Author:** Catapultam

Consolidated Patch.
```
* Cleric summoned hammers are no-drop.
* Pets no longer accept no-drop items given to them by anyone other than their owner.
* Add sliding cap on how much exp can be earned per kill; variable on both player level and con color
* Fixed Fists of Steel
* Multipet Version 2:
 - Primary\Secondary pet distinction is gone
 - Summon or Charm in any order
 - One pet per originating class;
   - One Mage summon or charm
   - One Enchanter summon or charm
   - One Necromancer summon or charm
   - etc
 - Targeting pet switches pet window
 - Pet commands with a pet targeted send command only to that pet
 - /pet qattack - sends one pet at a time
 - Pets will be forced into Ext Target slots 18, 19, 20
* Death no longer results in exp loss.
* Lowered base Exp rate by a moderate amount
* Increased group size exp penalty
* Increased Item Exp rates by a moderate amount
* Hell Levels removed

Hot-Fix (may need new zone server!)
* Tab\F8 should no longer target pets.
* Reverted H2H-only limit on FoS for now.
```

---

---

## 2024-08-21 01:31 - Entry 1275628398600785940
**Author:** Aporia

```
Effective immediately:

- With the decrease of overall exp gain, hell levels have been removed.

- Exp loss on death has also now been removed.
```

---

---

## 2024-08-20 02:19 - Entry 1275278018083815468
**Author:** Catapultam

```
Next Patch:
* Cleric summoned hammers are no-drop.
* Pets no longer accept no-drop items given to them by anyone other than their owner.
* Add sliding cap on how much exp can be earned per kill; variable on both player level and con color
* Fixed Fists of Steel
* Multipet Version 2:
 - Primary\Secondary pet distinction is gone
 - Summon or Charm in any order
 - One per per originating class;
   - One Mage summon or charm
   - One Enchanter summon or charm
   - One Necromancer summon or charm
   - etc
 - Targeting pet switches pet window
 - Pet commands with a pet targeted send command only to that pet
 - /pet qattack - sends one pet at a time
 - Pets will be forced into Ext Target slots 18, 19, 20
* Death no longer results in exp loss.

Hotfix:
* Lowered base Exp rate by a moderate amount
* Increased group size exp penalty
* Increased Item Exp rates by a moderate amount
```

---

---

## 2024-08-20 02:09 - Entry 1275275502965362720
**Author:** Retribution EQ #change-log

```
Next Patch:
* Mage Summoned items modified as follows;
  - Staff of Tracing: Symp Strike I -> Burn (1s/30s)
  - Staff of Warding: Symp Strike II -> Cancel Magic (1s/30s)
  - Staff of Runes: Symp Strike III -> Symp Strike I (1s/30s)
  - Staff of Symbols: Symp Strike IV -> Ward of Calliav (1s/30s)

  - Dagger: Burn -> Burst of Flame
  - Snake Fang: Poison -> Weak Poison
  - Spear of Warding: Rune I (unchanged)
  - Sword of Runes: Rune II (Unchanged)
  - Dagger of Symbols: Shock of Flame -> Shock of Blades

* Apocryphal Fire Crystal Staff: Sympathetic Strike V -> Sympathetic Strike III
* Blur of Axes damage is now scaled based on level.
```

---

---

## 2024-08-18 22:19 - Entry 1274855094273310810
**Author:** Catapultam

```
Hateplaneb is now fixed
```

---

---

## 2024-08-18 17:14 - Entry 1274778415710470184
**Author:** Retribution EQ #change-log

```
Hotfix:

Vulak is no longer rooted in place. It is highly recommended you pull him off his platform before engaging. Unless, of course, you enjoy lava.
```

---

---

## 2024-08-17 20:32 - Entry 1274465896978448579
**Author:** Retribution EQ #change-log

```
Hotfix:
* Haste now applies to combat skills again. (Should fix timer bugs)
```

---

---

## 2024-08-16 15:13 - Entry 1274023304469942294
**Author:** Catapultam

```
* Fury of Magic is no longer available to hybrids
* Fists of Steel no longer applies to 1HB weapons
```

---

---

## 2024-08-16 06:28 - Entry 1273891017434726481
**Author:** Retribution EQ #change-log

```
* Combat Fury normalized for all classes which normally obtain it. Now applies to all weapon skills (Rangers, it now works for archery).
* Veteran's Wrath normalized for all classes
* Mastery of the Past is now fully available to all spellcasting classes
* Shield Block is fully available to all classes able to equip shields
* Spell Casting Subtlety is now fully available to call spellcasting classes

Hotfix:
* Fixed bug preventing rogue from using SoS (Only effective in reloaded zones until reboot)
* Fixed bug around combat fury being a pre-req for other AA
```

---

---

## 2024-08-14 20:28 - Entry 1273377641671430257
**Author:** Retribution EQ #change-log

```
* Bazaar and Back will now place you in a semi-random place in the Bazaar
* Bazaar and Back will now prompt nearby group members if they want to travel with you. (beepboops can use /yes to accept it) (thanks @Chroma)
* Pets should no longer be unshrinkable monstrosities
* Pet names are now static (Parsers rejoice)
* Revamped pet names
```

---

---

## 2024-08-14 05:34 - Entry 1273152817099706388
**Author:** Retribution EQ #change-log

```
Tearel Overhaul

Tearel now allows you to attune the map to any destination you have previously discovered.
He can now also attune the map to your current expedition, but like group ports it takes special reagents (EoM).
Unlocking group ports or expedition attunements will unlock both.
If you already unlocked group ports, you may now use Tearel to return to your active expedition.
```

---

---

## 2024-08-13 17:34 - Entry 1272971478454898777
**Author:** Retribution EQ #change-log

**Consolidated Change Log**
*Note:* Some of these changes already went live, but all of them will be live on reboot.

```
- Mage Epic now correctly impacted by Pet Power 15
- Monster Summoning III now impacted by Pet Power 15
- Zumaik's Animation  now impacted by Pet Power 15
- Spirit of Khurenz stats increased to be in line with Pet Power 15 pets of other classes.
- Emissary of Thule now has an appropriate Pet Power 15 pet.
- Throwing Axes now stack to 100
- Sentry Badain now lets you know the 10th ring war is being worked on and returns your items.
- Enchanter Epic NPC Nadia Starfeast now summons the Enchanter's Sack on turn-in as well as a phrase for those following different guides.
- Bristlebane's Mischievous Mayhem should now be correctly casting every 48 seconds (up from 30).
- GoD quests accidentally enabled by allowing VP 2.0 have had their rewards scaled down instead of removed. If you paid plat for these items and no longer want them, DM me for a refund (Hoshkar and Xygoz quests).
- All Manastone qualities have been set back to a 1-second cast for this season. This may change in future seasons.
- Throw Stone no longer shares a CD with other major skills.
- Explosion of Spite, Beacon of the Righteous, and Area Taunt have had their range increased to 60. This is an increase of 10, 30, and 20 range respectively.
- Group leadership AA requires 100 Dark Blue kills per point.
- Raid leadership AA requires 50 Dark Blue kills per point.
- All poison vendors in the bazaar have had their faction removed.
- Progression NPCs "A Faded Memory" now see through invis, hide, and improved invis.
- Many item stat changes from the king-me channel.
- Ranger AA Frost Arrows has had its damage increased to match Flaming Arrows. Its mana cost per tick has been removed.
- Ranger AA Flaming Arrows has had its mana cost removed.
- Ranger spells Flaming Arrow (Not the AA) and Burning Arrow now apply a called shots effect, increasing archery damage taken by 10 and 20% for 3 ticks.
- Ranger AA Trick Shot occurrence increased to 5% per rank.
- Spell: Trickster's Calling has had it's duration reduced to 20 seconds.
- Crown of Rile has had its original click effect restored - Extinguish Fatigue, restoring Endurance instead of Stamina.
- Druid spell Nature Walker's Behest has had the durability of its pet increased (not its damage).

```

---

---

## 2024-08-10 02:42 - Entry 1271660020295270425
**Author:** Catapultam

```
* Tinkering is available to any race
* Shamans can perform Alchemy
* Rogues can perform Poison Making
* Rogue Sneak\Hide now functions as anticipated
* Melee Combat Skills (Kick, Bash, Kick(s), Strike(s), Frenzy) are all on seperate cooldowns
* Human and Iksar Monks will correctly display Cured Silk type armors.
* Fixed HoTT showing incorrect HP for yourself.
* AA abilities with recasts shorter than their duration will now suspend
* Item EXP to powersource now consumes a portion instead of all exp.
```

---

---

## 2024-08-09 16:03 - Entry 1271499064210362481
**Author:** Catapultam

```
* Added the ability to consume items to add exp to the item in your power source.
  - Must be from the same upgrade series at a lower stage
  - Same step are worth 25% exp
  - One step lower are worth 6.25% exp
* Secondary pets now accept equipment traded to them
* Secondary pets now respond to pet commands
  - /pet qattack now sends pet attack command to one pet at a time, in a cycle
* 4 ranks of Mnemonic Retention are granted on character creation.
```

---

---

## 2024-08-08 13:59 - Entry 1271105399537537064
**Author:** Retribution EQ #change-log

Hot-Fix
```
* Fixed zone server crash when handing items to charmed pets.
* Attempt at fixing certain mobs from summoning you under the world.
```

---

---

## 2024-08-06 17:10 - Entry 1270428849955405916
**Author:** Retribution EQ #change-log

8/06/2024
Consolidated Changelog - Deploying
```
Retribution has migrated to new server infrastructure, located centrally in a Chicago datacenter.

Bug Fixes:
* Improved Implied Targeting - Characters should no longer nuke themselves when a mob dies before their spell lands
* Bard Spellbars should lock\unlock as anticipated
* Experimental fix for spellbar remaining locked under unknown condition
* Both Players and Pets should display Ornaments as anticipated
* IP limit checkks are once again ignored in the Bazaar. Reminder; you are expected to only play a maximum of 3 characters at a time. The hard limit is not enforced at 3, but please do not abuse this grace.
* Vulak should now reliabily spawn. In addition, Thylex of Veeshan will occasionally shout a hint as to which trigger mobs remain up.
* Jaled Dar's Shade should now stop Douging.
* Magician epic pet should now be affected by pet foci again.
* Experimental fix for hotbars occasionally being rearranged

Improvements:
* First Orb of Retribution now also scales based on the farthest progression stage which this account has unlocked this season.
* Rod of Mystical Transvergence conversion ratio enhanced
* Azure Mind Crystals are now a targeted summon
* Sanguine Mind Crysals are now a targeted summon
* Bazaar vendor Augments are now all\all and pri\sec\range
* Removed need for locking on doors to Chardok Royals.

EoM Services:
* The Polymorphist in the Bazaar now has Drakkin as a race-change option.
* The Purveyor of Glamour has a SIGNIFICANTLY higher chance of awarding an 'interesting' random augment
```

Post-Patch
```
* Allaclone and CharBrowser now function correctly.
```

---

---

## 2024-08-05 17:19 - Entry 1270068579076935785
**Author:** Retribution EQ #change-log

8/05/2024
```
* Reworked NTOV script to spawn Vulak
* Removed lockpicking requirement from Chardok Royals
```

---

---

## 2024-08-04 21:07 - Entry 1269763708481962027
**Author:** Retribution EQ #change-log

08/04/2024

All of this probably needs a reboot to be fully effective. Next reboot scheduled for DT on Tuesday.
```
* Reverted anti-idle script in Bazaar
* Azure Mind Crystal is now a targeted summon (target receives item)
* Sanguine Mind Crystal is now a targeted summon (target receives item)
* Bazaar vendor weapon augments are now all/all pri/sec/range
* Sympathetic Procs should no longer reflect back at their owner
```

---

---

## 2024-08-04 00:23 - Entry 1269450676338167808
**Author:** Retribution EQ #change-log

08/03/2024
Immediate or Immediate-ish (new zone servers)
```
* Characters who are AFK\Idle for more than 10 minutes in the Bazaar and not Traders will be phased into a private instance. They will return to the public instance once they are no longer idle.
* Improved Implied Targeting
* Improved Bard spellbar refresh handling (maybe not perfect still)
* Aggressively unlock spellbar for classes other than Bard (Working on action-lock bug)
* First Orb of Retribution now has extra scaling based on progression stages unlocked.
* Pets use Ornaments again
* The Polymorphist will now help you become a Drakkin
* The Purveyor of Glamour has a significantly higher chance of giving you a random ornament that is cool, for some definition of cool.
* Player Ornaments work without re-equipping gear.
```

Next Reboot:
```
* Characters in the Bazaar are once again immune to IP limit checks
* Modulating Rod and Rod of Mystical Transvergence conversion rate increased
```

---

---

## 2024-08-02 22:52 - Entry 1269065307331493943
**Author:** Retribution EQ #change-log

**Adventurers**, *the time has come to brace yourselves for the icy challenges that lie ahead! The mystic land of Velious, long shrouded in legend and mystery, now calls to the bravest of Norrath's heroes.

Velious, the frozen continent, is a land of ancient secrets and formidable foes. Here, the towering ice-bound peaks and treacherous glaciers conceal forgotten dungeons, majestic dragon lairs, and the remnants of the great Coldain dwarves. The legendary giants of Kael Drakkel, the enigmatic dragons of the Temple of Veeshan, and the resilient Coldain dwarves await those bold enough to explore this frigid frontier.

Prepare your weapons, gather your allies, and steel your hearts against the biting cold. The journey through Velious will test your strength, courage, and resolve like never before. Will you rise to the challenge and uncover the hidden treasures and untold stories of this icy realm? The fate of Velious lies in your hands!

Welcome to Velious, where glory and peril are but a heartbeat away. Step forth, and let the adventure begin!*

**Patch Notes:**
```
When the server comes back up, all pending changes will come live, and addition to:

- Pets will now move behind mobs when not tanking
- Adjusted pet follow behavior
- Spells against Pets will now use their owner's resists in addition to their own
- Removed door to Plane of Mischief in Great Divide
- Manifest Elements is no longer granted as part of Mage Epic quest, and is removed from spellbooks
- Dire Charm now calculates 'light blue' correctly.
- Bard Song, Jonthan's Inspiration now has a self only proc component.
- Our beloved magic map is back with new functionality coming soon!
- LoY now releasing with Velious...
```

A HUGE thank you to all our donators, contributors, and active community members! We are having a blast and love that you are too!

We prepared a special treat for you... **LoY launches with Velious launch today!**

Additionally, as we continue to grow, we have decided to normalize non emergency downtime to Tuesdays. So that everyone can better plan 👍

Thanks to your contributions, this Tuesday we will be migrating to new hardware in a more centralized location!

Every week, Retribution gets better, thank you for being here!

Have fun tonight!

---

---

## 2024-08-01 19:14 - Entry 1268648098918567937
**Author:** Retribution EQ #change-log

```
Pending Patch/Reboot
- BST pets Zehkes, Khurenz, and Khati Sha have had their levels and HP adjusted
- BRD Epic can now be equipped in the range slot
- Echo of Memory added to Plane of Mischief ahead of Velious launch
- More Gods now give The God Slayer title.
```

---

---

## 2024-08-01 14:39 - Entry 1268578766473527470
**Author:** Catapultam

```
* Added Multiple Pet functionality
 - First pet Summoned or Charmed is 'Primary Pet' and is controlled via Pet Window
 - Subsequent pets may be Summoned as Secondary Pets
   - Up to 2 Secondary pets may be Summoned
   - Charmed pets may not be Secondary Pets
   - Secondary Pets do not get their own pet control windows, but will obey the following commands
     - /pet attack
     - /pet back off
     - /pet hold
     - /pet ghold
   - Beneficial spells affecting the Primary Pet will mirrored on any Secondary Pets
   - Secondary Pets Cannot:
    - Utilize a pet bag
    - Zone with their owner
 - Only one Pet per class may be summoned. (ie, a SHM/NEC/WAR may summon a Shaman spirit and a Necromancer pet, but not two Necromancer Pets)
```

---

---

## 2024-08-01 14:33 - Entry 1268577273339056153
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

## 2024-08-01 14:32 - Entry 1268576992429605067
**Author:** Catapultam

Retribution EQ #change-log

---

---

## 2024-07-22 04:54 - Entry 1264807693298962432
**Author:** Retribution EQ #change-log

```
Pending Patch:

All World Buffs now correctly count down when in Bazaar.
Holy Elixir once again stacks with other HoTs
```

---

---

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

## 2024-07-20 19:07 - Entry 1264297691672743948
**Author:** Retribution EQ #change-log

```
- Actually, for sure, definitely, REALLY fixed Eejag this time
- Phara Dar's adds should now aggro correctly.
```

---

---

## 2024-07-19 17:35 - Entry 1263912204261134387
**Author:** Retribution EQ #change-log

Immediate Effect:
```
- Low-AA bonus increased to 400%. At 0AA, you will recieve a 4x bonus to AAXP, decreasing linearly until a total of 300AA have been earned
```

---

---

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

## 2024-07-18 20:38 - Entry 1263595829432946698
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

## 2024-07-18 15:53 - Entry 1263523992602546348
**Author:** Retribution EQ #change-log

Pending Reboot:
```
* Fixed and re-enabled AAXP Scaling based on total earned AA
* Symp proc durations reduced to 16h from Permanent
```

---

---

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

## 2024-07-17 01:22 - Entry 1262942533567250433
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

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

## 2024-07-16 14:06 - Entry 1262772314844565504
**Author:** Retribution EQ #change-log

(Next Reboot)
```
- Heroic Charisma is now applied as a direct resist adjustment to spells. (ie; 67 HCha is -67 additional resist check to all spells)
- Improved mob pathfinding
```

---

---

## 2024-07-16 05:16 - Entry 1262638983905804308
**Author:** Retribution EQ #change-log

```
Pending Patch:
Rage of Rallos Zek AA - Endurance Cost Reduced by 1/4

Key requirements in Seb have been removed
```

---

---

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

## 2024-07-11 14:20 - Entry 1260963856692285571
**Author:** Retribution EQ #change-log

```
- Mobs will no longer respawn at 22hr in Non-Respawning instances (to coincide with increased dz lifetimes)
```

---

---

## 2024-07-11 06:09 - Entry 1260840422658277490
**Author:** Retribution EQ #change-log

```
- Temporary pet combat messages should now be visible.
- Pet names for temporary pets, familiars, etc are a bit more descriptive
```

---

---

## 2024-07-11 03:01 - Entry 1260793098468986932
**Author:** Retribution EQ #change-log

```
- 'Unlocking' (Even if still time-locked) Velious now allows bypass of key requirement for Veeshan's Peak.
- 'Unlocking' (Even if still time-locked) Planes of Power now allows bypass of key requirement for Vex Thal.
```

---

---

## 2024-07-11 03:01 - Entry 1260793093314183179
**Author:** Retribution EQ #change-log

```
- Sage of Anachronism can now expand your hole(s)
- Sage of Anachronism will replace lost First Orb of Retribution
```

---

---

## 2024-07-11 03:01 - Entry 1260793044303613973
**Author:** Retribution EQ #change-log

```
- Pet taunt will now enable them to peel off of players.
- Pets will now taunt any mob attacking their owner during their taunt cycle, even if that is not the mob they are currently attacking.
```

---

---

## 2024-07-09 02:16 - Entry 1260056954194366534
**Author:** Retribution EQ #change-log

```
- You will now recieve a notification when Echo of Luck or Seasonal status upgrades a quest reward.
- You will now recieve an upgrade when Seasonal status upgrades a loot reward.
- Really fixed Staff of Forbidden Rites charges.
```

---

---

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

## 2024-07-08 21:40 - Entry 1259987424134565927
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

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

## 2024-07-05 02:38 - Entry 1258612926680531044
**Author:** Catapultam

```
- Removed 'Expanded Pet Affinity' (for now, might do something with this concept later)
```

---

---

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

## 2024-06-27 16:06 - Entry 1255917133528039464
**Author:** Retribution EQ #change-log

Pending Reboot:
`
- Hate 2.0 items are being scaled down to ensure future content isn't completely negated. Most will still be/be close to BiS for Classic. Thank you for your understanding.
- Manastone now has a 1 second cast time but has 10x the effectiveness. Please update your scripts accordingly.
- Consumable requirement removed from Enchanter runes. Casting times have been reduced.
- King-me channel caught up
- Misc quest and bug fixes (see bug/suggestion forum for details)
- Daily DZ/Lockout timers reduced to allow people with a static play schedule to have access at the beginning of their play session each day.
- SHM/BST healing spell, Spirit Salve, now available in bazaar.
- RNG spell, Falcon Eye, now available in bazaar.
`

---

---

## 2024-06-26 13:31 - Entry 1255515686550114346
**Author:** Retribution EQ #change-log

`
- BST Now correctly get Feral Swipe before Frenzied Swipes as their seasonal AA
- Pending reboot, Drelzna now has a chance to drop Jboots
- Najena getting DZ to accommodate JBoot fanbois
`

---

---

## 2024-06-25 04:10 - Entry 1255012117665550440
**Author:** Catapultam

```
- Implemented Implied Targeting for pet attack command
```

---

---

## 2024-06-23 19:02 - Entry 1254511871969726614
**Author:** Retribution EQ #change-log

```
6-23-24

Vah Shir, Iksar, Beastlords and Berserkers are now available for ALL players regardless of expansion unlock.
Progress with who you want!

Rogue Epic no longer completable in Classic. Congratulations on the feat and thank you for being so agreeable Pointz the Assassin! His Epic will be returned to him as soon as Kunark launches.

SK 51 AA was pointing to the wrong spell file. It was doing too much up front mana regen and was missing its recourse. Fixed on next patch.
```

---

---

## 2024-06-22 19:57 - Entry 1254163331300986880
**Author:** Retribution EQ #change-log

Welcome to Season 1!

With all the hype, I forgot to actually post this!

```**Seasonal Characters**

 - New characters created during a Season will be flagged as 'Seasonal'
 - You may opt-out of seasonal play by using the command #disable_seasonal confirm
     - YOU MAY NOT GO BACK TO BEING SEASONAL AFTER OPTING OUT. NO EXCEPTIONS.

 - Seasonal Characters receive the following bonuses:
   - (Season 1 Specific) Start with 'First Orb of Retribution', an augment which will grow in power as you participate in the Season
   - (Season 1 Specific) Start with 'Portable Hole', an upgradable 20-slot bag which you will be able to upgrade as you progress
   - Greatly increased chance to recieve Apocryphal and Rose-Colored drops
   - Certain other rewards for defeating progression challenges!

 - Seasonal Characters may NOT...
   - Group with non-Seasonal characters
   - Trade with non-Seasonal characters
   - Buy from non-Seasonal traders
   - Buy ANYTHING from NPC vendors which was sold by players
   - Pick up items off the ground that were placed by players
   - Cast spells on non-Seasonal characters.
   - Be cast upon by non-Seasonal characters
   - Loot kills that they did not receive XP for
   - Enter DZs with non-Seasonal characters
   - Use the Bazaar Buff-bot for standard buffs
   - May not have more than 6 players in a DZ

* General Changes
 - Everything previously mentioned in the changelog that didn't actually go live due to technical issues.
 - NPCs, except for player Pets, no longer keep items handed by players, they are immediately destroyed.
 - Charmed Pets will hand the item back, while also equipping a copy. The equipped copy is destroyed when the charm breaks.
 - Agents of Retribution renamed to Echo of the Past and will now offer two types of instances; Respawning and non-Respawning
  - Each instance type is on a different replay timer
 - Dire Charm now works on any mob up to light blue to the caster.

* Bug Fixes
 - The Polymorphist now works correctly again!
 - The Purveyor of Glamour now works correctly again!

* Donation Rewards (Echo of Memory)
 - Merchant added in the Bazaar which sells items for Echo of Memory alt currency.
  - This alt currency is awarded to players as a 'Thank You' for donations to server costs
 - 20, 30, 40 slot, No Drop bags now available on this merchant in 10 different colors
 - Unattuners added to this merchant
 - No stat Illusion clickies added to this merchant
 - Anything purchased from this merchant may be sold back to them for a small loss```

---

---

## 2024-06-19 19:15 - Entry 1253065709374930956
**Author:** Retribution EQ #change-log

Pending reboot/patch etc.

```
LGuk DZ fixed
Ghoulbane now drops from Shin Lord again
Infused by rage display error fixed (maybe)
Note for Janam quest has been fixed in E/W Freeport
Incorrect item IDs fixed on drop tables for 6th Necro Skullcap quest
Remaining LoY noob quest NPCs removed.
Skyshrine key no longer required to go to CS
Duplicate Chardok agents removed, remaining one fixed.
Zlandicar becomes a dragon again
Chardok, Great Divide, Fungus Grove, and Tenebrous now have Waypoints
Donation Vendor Added (Will accept EoM for goods soon)
Improved Damage I and II are now working again on 20+ broken items.
Enchanter Doppelganger AA works once again, has adjusted stats, and casts a DD according to its level/rank.
Enchanter AA Deep Sleep now has a 20/40/60/80/100% chance to proc based on rank.
Druid spells with AC debuffs now scale with level again

Necromancer and Mage Pet Buff lines have been normalized so that benefits scale throughout all levels and not one big chunk at the end. (Focus Death and Burnout Lines). Melee mitigation, Accuracy, STR, Haste, ATK, AC, Strikethrough now incrementally increase with each rank of the spell- addressing many performance questions at different level brackets.

Mistmoore, LGuk, Unrest, and CoM now have DZs available.
The shared bank will not longer accept plat.

Dire Charm now works on any light blue mobs that CAN be charmed and is no longer hard capped by level.

Veksar now unlocks with Luclin

Necro AA Cascade of Decay can now be up the same time as sympathetic strike buffs.

Fabled Nagafen can now only be reached by hailing the Sage of Anachronism in the Bazaar

```

---

---

## 2024-06-04 06:49 - Entry 1247442094872858644
**Author:** Catapultam

```
* experimental fix for Artifacts not having persistent ItemIDs
```

---

---

## 2024-06-03 01:16 - Entry 1246995837700018248
**Author:** Retribution EQ #change-log

```
Pending Patch:

A number of small but effective changes have been made to allow for a more diverse spread in the three man set up for early progression.

Calliav Line available to MAG, NEC, and BST- Mana cost halved. Casting time halved. Cooldown halved.
Magician Sol Ro pet items (Pet Power 5) now effect level 29-49 pets in a more noticeable way.
Magician Planar pet items (Pet Power 10) now effect level 49-60 pets in a more noticeable way.
Necromancer Epic and Encyclopedia Necrotheurgia added Minion of Hate effect now has a more noticeable effect on Emissary of Thule and Invoke Death

ALL MAGE PETS from level 29+ can benefit from Pet Power in a similar way of the custom epic pet does.
Earth pets will have the same HP and AC as the epic pet while the fire pet will match the epic pets damage (matches at each pet power rank while using the appropriate pet). Water and Air will be between both but keep their unique procs/abilities/casts.

This reduces the necessity of completing the mage epic and compensates for pet power draughts.

Velious drop Essence of Nature (Tunare) now has the Summoner's Boon focus (Pet Power 15). This change serves to fill the gap in pet power between Kunark and Luclin for Necromancers and Magicians as both can now be effected by Pet Power 15.

BST Pet Spirit of Omakin has been put on Vocarate Water drop table.
BST Pet Spirit of Zehkes put on Greater Vocaration Water drop table.
BST Pet Spirit of Khurenz put on Klandicar, Zlandicar, Wuoshi, Velketor, Kelorek, Sontalak, Master of the Guard, Tormax, and Dain
BST Pet Spirit of Khati Sha stays in Luclin

All of these four pets have had stats adjusted based on Mage/Necro pet power updates.

BST AA Bite of the Asp RK1 now does 25 damage per tick base, but scales 1 damage per level.
BST AA Chameleon Strike RK1 now does 25 base damage, but now has RK2 available at 51 for an increased base damage.

MNK AA Imitate Death now has a base 12minute CD with each rank of Hastened Death removing 2 minutes from the CD, max rank resulting in no CD. It now costs 50 Endurance.

Chloroblast level requirement changed for RNG/BST to 59.

Stacking issues with Warrior AA Infused by Rage fixed.
Blood of Ssra is now a unique spawn and should no longer double spawn sometimes.
Items no longer delete from your cursor when zoning
Urthron's Ultimate Unattuner now works again.

Minotaurs in Steamfont no longer hoard gems.

```

---

---

## 2024-05-18 23:47 - Entry 1241537691439333516
**Author:** Retribution EQ #change-log

```
Pending Patch:

Enchanter AA Illusions of Grandeur now gives 200% Crit DoT damage up from 110%
Enchanter AA Illusions of Grandeur now gives 200% Crit Nuke damage down from 250%
Enchanter AA Doppelganger has had it's Rk I and II pets adjusted to match the changes made to Rk III that were somehow reverted.
Enchanter AA Eldritch Rune is now castable on others.
Enchanter Spell Cajoling Whispers can now be found on Illusionist Jerup in the Bazaar

All Disciplines that DO NOT have a hastened AA have had their Cooldowns reduced to 15 minutes.
All AA that DO NOT have a hastened AA have had their Cooldowns reduced to 15 minutes.

Warrior AA Infused by Rage is now an active AA that applies a permanent buff that can be clicked off by the player.

Tearel's Waypoint list is now sorted properly.

```

We are also bringing live Retribution's Wiki ahead of seasonal launch!

A huge thank you to @ashrem2159 and @Shin Noir (Xackery)

Check out https://retributioneq.com/ for the link!

Please let us know if you think anything should be added/edited.

---

---

## 2024-05-14 11:02 - Entry 1239895622669172778
**Author:** Community Updates

##
👀  What's that tag?

Hey Admins and Mods! Starting May 15, it's possible you might notice something new next to some of your members' usernames: ✨ **Guild Tags **✨

See a cute little tag next to a member's username or profile? That's a **Guild Tag**, which indicates someone's membership to a chosen Guild. You can click on this tag to see the Guild profile, and even apply for membership there as well. What this means for you, beloved Admins and Mods, is that if your server's AutoMod is on, it will also check for Guild Tags ☑️

**What's a Guild?** It's a small, exclusive server that members can apply to join. These servers are tight-knit communities where members can relish in shared identities, hobbies, play styles, and more!
> Please note that Guilds are only available to a small number of servers at this time, so not every server has access to this experiment. Additionally, our support team cannot manually add servers to this experiment.

Much love,
The Discord Team

---

---

## 2024-05-12 20:52 - Entry 1239319403347181588
**Author:** Catapultam

```
- Artifacts no longer become no-drop if you zone with them equipped
- Augments can no longer be dynamic items (Artifacts)
- Discovery tag on Artifacts now refers to the person who discovered the Legendary variant
- Artifacts of items with charged activated abilities now have unlimited charges, must be equipped to use, and have a cast time of either 5 seconds or the cast time of the actual spell, whichever is greater
```

---

---

## 2024-05-12 18:32 - Entry 1239283962421968940
**Author:** Retribution EQ #change-log

```
- Fixed Gram Dunnar giving Intricate Wooden Figurine
- You should no longer be able to complete the Tome of New Beginnings quest multiple times
- Fixed several Paladin class checks in quests
- Fixed many Monk class checks across quest scripts
- Quarm awards GoD flag if you don't have it already somehow
```

---

---

## 2024-05-11 06:37 - Entry 1238741761338118144
**Author:** Catapultam

```
- Maybe fixed sleeping ogre!
```

---

---

## 2024-05-03 07:18 - Entry 1235853048107241472
**Author:** Catapultam

```
* Re-wrote implied targeting again
* fixed expanded pet affinity killing some pets
* combat procs only trigger on damage or healing spells
```

---

---

## 2024-05-02 17:11 - Entry 1235639942298861588
**Author:** Catapultam

```
* Fixed feedback for item XP gain
* Adjusted item XP rate
* Combat effects on items can trigger on spell casts
* Spell Damage and Heal Amount is limited to doubling the initial value of a spell
* Fixed discovery message spam
* Reduced spellproc rate for bard songs
* Artifacts should be explicitly droppable
* Fixed artifact discovery from itemxp
* Fixed LoS on combat abilities
* Ranged attacks can proc bows
```

---

---

## 2024-05-01 04:13 - Entry 1235081630373122109
**Author:** Catapultam

```
* Auto-looting items will no longer place items in the Power Source slot. /autoinventory or use of the auto-inventory area of your inventory screen will continue to do so (for now!)
* Added feedback for how much item XP you are gaining.
```

---

---

## 2024-05-01 02:47 - Entry 1235060114998956103
**Author:** Catapultam

```
* Leveling up an item will now produce a Discovery event
* Leveling up an item to Legendary can now produce an Artifact
* Fixed some logic around discoveries and artifacts
```

---

---

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

## 2024-04-28 23:18 - Entry 1234282565913804800
**Author:** Retribution EQ #change-log

```
Bazaar NPC overhaul.

Bazaar NPCs have been moved to give the Bazaar a more natural feel.

Check the back stalls for GMs, Spell Vendors, and Tomes.
```

---

---

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

## 2024-04-16 01:52 - Entry 1229610384810577930
**Author:** Catapultam

```
- THJ is now officially running entirely off of Retribution's database.
- More iteration to come in terms of scripts and content!
```

---

---

## 2024-03-30 16:33 - Entry 1223671331258892388
**Author:** Catapultam

Pending Reboot\Luck in getting a fresh zs
```
- Buff stacking adjusted
  - Short Buffs (Songs) and Long Buffs no longer have stacking conflicts between categories.
  - Detrimental and Beneficial spells no longer have stacking conflicts between categories.
  - The EFFECTS of the buffs may not stack (mostly between Detrimental and Beneficial), but the buff icons themselves won't block or overwrite. This mostly applies to certain effects like haste\slow.
- Casting skills can only increase from spells cast from spellgems
- Bard Songs will no longer fade just because they ran out of Rune capacity
- Re-introduced Extended Pet Affinity.
  - Now applies to instant-duration (ie heals, cures) as well. Pets need a little bit of love in terms of survivability.
- Instrument modifiers no longer scale effects inappropriately.
```

---

---

## 2024-03-30 15:20 - Entry 1223653123919184135
**Author:** Catapultam

* Forgot to add earlier
```
- Faction checks now use the best modifier amongst your unlocked classes
```

---

---

## 2024-03-29 18:41 - Entry 1223341400129540257
**Author:** Catapultam

* Pending Reboot
```
- Focus effects now work
- Spell Damage\Heal Amount is limited so that it will no more than double the base effect of a spell
- Sympathetic procs are now scaled based off of the cast time and mana cost of the spell which triggered them.
```

---

---

## 2024-03-29 15:35 - Entry 1223294443701014601
**Author:** Catapultam

```
- Corrected /who formatting
- Out-of-Range mobs no longer show up as 'Mob' on map.
  - This is to correct the memory leak in the client during long play sessions
- Cast time is now displayed on spell inspect window
```

---

---

## 2024-03-28 03:29 - Entry 1222749347314405427
**Author:** Aporia

```
Pending reboot

- Emperor SSRA is now a Unique Spawn
- Monk FoS AA is now H2H only
- Bard song cap to correctly mimic Ret
```

---

---

## 2024-03-21 03:41 - Entry 1220215612547141632
**Author:** Catapultam

```
- Sympathetic Procs no longer trigger for anything except spell casts (from Gems)
- Sympathetic Procs no longer trigger for bard songs
```

---

---

## 2024-03-15 22:55 - Entry 1218331890960826460
**Author:** Catapultam

```
- Focus Effects should now work
- Monks should be able to DW empty-handed
- Monk epic should now affect base stats of empty hand h2h attacks
- Group Buffs should work on charmed pets
```

---

---

## 2024-03-15 07:24 - Entry 1218097434379419658
**Author:** Catapultam

```
- Fixed Lavastorm zone lines - you will need to delete lavastorm.eqg from your game directory manually.
```

---

---

## 2024-03-15 03:10 - Entry 1218033525576433674
**Author:** Catapultam

```
- AA cast time is 0 again
- Adventurer's pack increased to 18 slots (will go back to 12 on next server wipe)
```

---

---

## 2024-03-15 02:43 - Entry 1218026683962101780
**Author:** Catapultam

```
- Content DB is now more closely aligned with Retribution
```

---

---

## 2024-03-09 17:21 - Entry 1216073319342673990
**Author:** Catapultam

```
- Delay on debuffs on target applied removed
- Pet spell messages should be working now
- Added pet resist and DoT messages
- Applying a charm spell no longer strips your debuffs
```

---

---

## 2024-03-08 20:12 - Entry 1215754000574582916
**Author:** Unbrella

RIP

---

---

## 2024-03-08 20:12 - Entry 1215753990982078604
**Author:** Unbrella

This was my favorite door

---

---

## 2024-03-08 19:33 - Entry 1215744343210459296
**Author:** Catapultam

``` - Deleted this door.```

---

---

## 2024-03-08 19:33 - Entry 1215744114260443226
**Author:** Catapultam

```
- Slightly increased base XP rate
- Greatly increased AAXP rate
- Increased modifiers for Red\Yellow
- Decreased modifiers for Blue\LBlue\Green
```

---

---

## 2024-03-06 23:57 - Entry 1215085856986103918
**Author:** Catapultam

```
- Progression flags can be acquired from any version of Naggy\Vox\Phinny```

---

---

## 2024-03-06 19:35 - Entry 1215020038755713165
**Author:** Catapultam

```
- Added Pet Discipline to starting AA for Mages, Necromancers, Beastlord, Enchanter, Shaman
- Added Advanced Pet Discipline to starting AA for Mages & Necromancers
- Starting AA are now properly reapplied on zone if you are missing any
```

---

---

## 2024-03-06 18:26 - Entry 1215002506032320612
**Author:** Catapultam

```
- Non-Weapon Instruments that can be equipped in Primary or Secondary can now be equipped in range and ammo slots (Ammo currently does nothing).
```

---

---

## 2024-03-06 02:25 - Entry 1214760643895238697
**Author:** Catapultam

```
- Added /mapfilter to map (Thanks, @Voidless)
- Added click-to-target on map for mobs who you can detect

- Updated patcher to recognize LAA eqgame.exe (may ned to manually download new patcher at https://github.com/The-Heroes-Journey-EQEMU/eqemupatcher/releases/download/1.0.6.49/heroesjourneyeq.exe)
```

---

---

## 2024-03-05 01:42 - Entry 1214387592389328927
**Author:** Catapultam

```
- Mixed Latent\Awakened\Untagged quest turn ins now REALLY work
- You can no longer zone into DoN or OoW zones
```

---

---

## 2024-03-04 05:50 - Entry 1214087621375168573
**Author:** Carolus Rex

You should probably change this channel so that not everyone can post here

---

---

## 2024-03-03 10:47 - Entry 1213799949716819978
**Author:** Catapultam

```
- Added Latent\Awakened bags (next reboot)

- SolB instances are now available.
- Permafrost instances are now available.
- Kedge instances are now available

- Instancing on The Heroes' Journey:
  - Seek out 'A Servant of the Journey' outside, near, or inside raid zones.
  - You will be offered up to two types of instances; Challenge or Opportunity
  - All instances are limited to 6 characters and last 24hours.
  - Challenge instances are available to anyone who have either
     1) Not completed the progression flag associated with this zone
     2) Not exceeded the recommended maximum level for this zone
  - Challenge instances are non-respawning, objective-based tasks, and will reward both 'Accolades of Heroism' and progression flags.
  - If an ineligible person joins a Challenge instance, it will immediately fail.
  - Challenge instances lock immediately upon starting, and have a 20 hour lockout upon completion.
  - Accolades of Heroism will be used to buy equipment in the Bazaar, and will be fully tradable.
  - Opportunity instances have a 20 hour lockout upon request.
  - Opportunity instances are direct copies of the relevant zone, with full repops, etc.
  - Opportunity instances are available to anyone who both meets the level minimum for the instance and has completed the Challenge mode on any character.
```

---

---

## 2024-03-03 09:12 - Entry 1213776104800653393
**Author:** Catapultam

```
- Augments are now All\All
```

---

---

## 2024-03-03 03:41 - Entry 1213692673970675772
**Author:** Catapultam

```
- Increased the rate at which upgraded versions of items will drop
```

---

---

## 2024-03-02 04:36 - Entry 1213344196212031572
**Author:** Catapultam

```
- Tradeskills can now be done with any mix of untagged\latent\awakened components```

---

---

## 2024-03-01 07:01 - Entry 1213018140976357377
**Author:** Catapultam

```
- Characters in the Bazaar are exempt from IP box limits
```

---

---

## 2024-03-01 00:59 - Entry 1212927236416475156
**Author:** Catapultam

```
- Added a large number of waypoints in Classic
- Added a large number of waypoints in Kunark
- Adjusted respawn frequency of all mobs
```

---

---

## 2024-02-29 23:17 - Entry 1212901460459659356
**Author:** Catapultam

```
- Tradeskills will always return (Awakened) items.
` Removed (Latent) tag from normal-quality gear. Henceforth 'untagged' tier.
- Renamed (Potent) tag to (Latent)
```

---

---

## 2024-02-29 22:23 - Entry 1212887837637091349
**Author:** Catapultam

```
- Added MIT and AVG stats to inventory; These show ACTUAL mitigation and avoidance AC after softcap are taken into account
```

---

---

## 2024-02-29 21:54 - Entry 1212880650231750686
**Author:** Catapultam

```
- Improved merchant filtering (patch needed)
- All activated are now instant-cast (patch + reboot)
- Augments no longer require distillers to remove (reboot)
```

---

---

## 2024-02-29 19:24 - Entry 1212842973805420665
**Author:** Catapultam

```
- Soulbinders will also offer gates to bazaar and bind
```

---

---

## 2024-02-29 18:03 - Entry 1212822578775855125
**Author:** Catapultam

```
- reverted 'humans look like monk thing' for now
- restored original UI
- custom UI can be loaded with /loadskin thj_ui
```

---

---

## 2024-02-29 01:59 - Entry 1212579951899836436
**Author:** Catapultam

```
- Switching base class should no longer be required for any class combinations
- Please report any problems with spellcasting as high-priority bugs
- Humans and Iksar with Monk in their composition will look like Monks
```

---

---

## 2024-02-28 20:45 - Entry 1212500743593001070
**Author:** Catapultam

```
(Patch Required)
- Merchantlist filter now properly accounts for your classes
- Levels displayed on spell scrolls is no longer wonky for shared spells
```

---

---

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

## 2024-02-27 07:56 - Entry 1211944847376777226
**Author:** Catapultam

```
- Disciplines should now no longer cause crash on zone
- Implied targeting should be much improved (corpses, procs)
- Pet buffs & heals no longer force change target to pet
```

---

---

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

## 2024-02-24 09:21 - Entry 1210879145433628741
**Author:** Catapultam

```
- Disabled corpses for now to work around a crash bug
```

---

---

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

