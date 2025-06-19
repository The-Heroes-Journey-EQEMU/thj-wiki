---
title: Changelog - December 2024
description: Changelog entries for December 2024
published: true
date: 2025-06-19T23:04:30.832Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:30.832Z
---

# Changelog - December 2024

[← Back to Recent Updates](/en/Change-log-history) | [← November 2024](/en/changelog-2024-11) | [January 2025 →](/en/changelog-2025-01)

---

*34 updates in December 2024*

<a name="entry-1323716631951577148"></a>

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

<a name="entry-1323713355206234286"></a>

## 2024-12-31 18:04 - Entry 1323713355206234286
**Author:** Catapultam

```
- Experimental change for /baz crash
- Experimental change for crash-on-zone
```

---

---

<a name="entry-1323409018273923123"></a>

## 2024-12-30 21:54 - Entry 1323409018273923123
**Author:** Catapultam

I am a generous god.
```
- The Vision of Ayonae will now allow you to reduce your level, and return to up to your previous maximum level. This service costs 500pp per level changed.
```

---

---

<a name="entry-1323104912036462603"></a>

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
- Turn-ins with multiple identical items will once again function (@Akk)
- Recovering Parcels will no longer require an open top-level inventory slot (Thanks @Neckkola)
- Items with charges will no longer be interpreted as stacked items for quest turnins. (@Akk)
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
- Reworked Tunare encounter (@Trust)
- Reworked Bristlebane encounter (@Trust)
- Reworked TOFS mirrors and keys (@Trust)
- Added DZs for TOFS, CC, Iceclad
```

---

---

<a name="entry-1321688812581027932"></a>

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

<a name="entry-1321237072048033833"></a>

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

<a name="entry-1321019345039790141"></a>

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

<a name="entry-1320912696492691486"></a>

## 2024-12-24 00:35 - Entry 1320912696492691486
**Author:** Catapultam

This is also Deployed.

---

---

<a name="entry-1320638822970687630"></a>

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

<a name="entry-1320539762389422122"></a>

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

<a name="entry-1320263658823221339"></a>

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

<a name="entry-1319751613853859863"></a>

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

<a name="entry-1318262438977736856"></a>

## 2024-12-16 17:04 - Entry 1318262438977736856
**Author:** Catapultam

ROLLING DEPLOYMENT (Will be inconsistent which zones this works on until next reboot. Do not expect bazaar to be effected)
```
- Unattuner should now function again
```

---

---

<a name="entry-1318237038197342208"></a>

## 2024-12-16 15:23 - Entry 1318237038197342208
**Author:** Catapultam

```
- Glamour-Stones now have teal names.
- Added `missingspells` argument to `/outputfile`. Use like `/outputfile missingspells [filename]` (where `filename` is optional) to output a level-sorted list of spells to a file in your EQ directory. File name defaults to `<character>-MissingSpells.txt`. (Thanks @dannuic)
```

---

---

<a name="entry-1317589922177093672"></a>

## 2024-12-14 20:31 - Entry 1317589922177093672
**Author:** Catapultam

```
- Added title for owning a Vial of Prismatic Dye
```

---

---

<a name="entry-1317579139951235225"></a>

## 2024-12-14 19:49 - Entry 1317579139951235225
**Author:** Catapultam

DEPLOYED
```
- Added 10 titles for prolific Gamblers.
```

---

---

<a name="entry-1317508462522925087"></a>

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

<a name="entry-1316571786611261500"></a>

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

<a name="entry-1316438968958455849"></a>

## 2024-12-11 16:18 - Entry 1316438968958455849
**Author:** Catapultam

```
- Removed Class Requirements from all epic quests (Thanks @Prymetyme)
```

---

---

<a name="entry-1316279399741657161"></a>

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

<a name="entry-1315493798641401887"></a>

## 2024-12-09 01:42 - Entry 1315493798641401887
**Author:** Catapultam

Rolling Deploy (Requires new zone server; new DZ does not guarantee this)
```
- Corrected Veterancy scaling formula to correctly function near the end of the scaling range
```

---

---

<a name="entry-1315454822505517128"></a>

## 2024-12-08 23:07 - Entry 1315454822505517128
**Author:** Catapultam

Hotfix
```
- Reduced maximum veterancy bonus from 5x to 3x AAEXP
```

This impact of the change allowing Veterancy to apply AFTER the per-kill cap was significantly greater than appeared in testing. This change will still result in overall higher AAEXP rates than prior to the most recent patch.

---

---

<a name="entry-1315352052188184646"></a>

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

<a name="entry-1315148539457703938"></a>

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

<a name="entry-1314840330230566975"></a>

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

<a name="entry-1314802696938586153"></a>

## 2024-12-07 03:56 - Entry 1314802696938586153
**Author:** Catapultam

Deployed (Client Patch)
```
- ACTUALLY FIXED NOCLIP OBJECTS (Thanks @Bakemono for enormous troubleshooting help)
```

---

---

<a name="entry-1314426106375573516"></a>

## 2024-12-06 03:00 - Entry 1314426106375573516
**Author:** Catapultam

Deployed (-ish)
```
- Fixed 'Spells are 255 until you zone once'
- Possibly fixed some pets poofing on server-down (Sorry, it won't work on the next server-down, probably)
- Disc timers are no longer transferred to new characters when you camp to character select and switch toons
- Spell Procs added by buffs must be unique (@Grek)
- Potentially fixed client memory leak causing collidable objects to no longer be collidable
```

---

---

<a name="entry-1314128377191465030"></a>

## 2024-12-05 07:17 - Entry 1314128377191465030
**Author:** Catapultam

Deployed
```
- Fix for crash-on-zone for some clients
```

---

---

<a name="entry-1313560375739941017"></a>

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

<a name="entry-1313276869738631230"></a>

## 2024-12-02 22:53 - Entry 1313276869738631230
**Author:** Catapultam

```
(Quests, Deployed)
- Re-enabled 'Slayer Titles'
- Various fixes to Toirgan Mines scripts (@Trust)
- Various quest and script fixes (@Grek)
- Various quests and script fixes (@Trust)
```

---

---

<a name="entry-1313142732813766719"></a>

## 2024-12-02 14:00 - Entry 1313142732813766719
**Author:** Catapultam

Deployed
```
- Experimental fix for those crashing on logging\zoning into the Bazaar
```

---

---

<a name="entry-1312932176060223628"></a>

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

<a name="entry-1312645296576135229"></a>

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

<a name="entry-1312621082380992636"></a>

## 2024-12-01 03:27 - Entry 1312621082380992636
**Author:** Aporia

```
Option added to Omat Vastsea's quest script to summon back Natasha to make it easier for players who ran into issues during the Cleric epic to fix their quest state.

By saying "I wish to see Natasha", you can trigger a spawn of Natasha. Who is now immune to player damage.

Thank you Grig
```

---

---

