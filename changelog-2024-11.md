---
title: Changelog - November 2024
description: Changelog entries for November 2024
published: true
date: 2025-06-19T23:04:34.918Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:34.918Z
---

# Changelog - November 2024

[← Back to Recent Updates](/en/Change-log-history) | [← October 2024](/en/changelog-2024-10) | [December 2024 →](/en/changelog-2024-12)

---

*36 updates in November 2024*

<a name="entry-1312479580904362005"></a>

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
- Deep will no longer eat items turned in by non-Monks (@Grek)
```

---

---

<a name="entry-1312210013049061387"></a>

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

<a name="entry-1311563335329779764"></a>

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

<a name="entry-1311249916022100048"></a>

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

<a name="entry-1310692059795034183"></a>

## 2024-11-25 19:42 - Entry 1310692059795034183
**Author:** Aporia

```
- Echo added for Lake Rathe
- Crag spiders look less human and more spider|
- More LoY items tuned down to be between Kunark and Velious loot
```

---

---

<a name="entry-1310651946822013050"></a>

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

<a name="entry-1310448565931474955"></a>

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

<a name="entry-1309678834458562560"></a>

## 2024-11-23 00:36 - Entry 1309678834458562560
**Author:** Catapultam

Deploying
```
- Corrected logical error preventing Base Crit Damage Ratio from applying
- Temporarily disabled 1x/char AA reset on Vision of Aayonae.
```

---

---

<a name="entry-1309582982549602315"></a>

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

<a name="entry-1308919463030165574"></a>

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

<a name="entry-1308440149453049907"></a>

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

<a name="entry-1307944944706650153"></a>

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

<a name="entry-1307724713937862677"></a>

## 2024-11-17 15:11 - Entry 1307724713937862677
**Author:** Catapultam

```
- Pet illusion wands should work as expected. You may need to resummon any necro pets.```

---

---

<a name="entry-1307433633753202742"></a>

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

<a name="entry-1307044028734378104"></a>

## 2024-11-15 18:06 - Entry 1307044028734378104
**Author:** Catapultam

Pending
```
- Fix crash related to additional loot
```

---

---

<a name="entry-1306853645442224129"></a>

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

<a name="entry-1306665076367036507"></a>

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

<a name="entry-1306393344519442453"></a>

## 2024-11-13 23:00 - Entry 1306393344519442453
**Author:** Catapultam

Deployed
```
- ZEM normalized to 2.0 for zones with ZEM below 2.0
```

---

---

<a name="entry-1305993720575037471"></a>

## 2024-11-12 20:32 - Entry 1305993720575037471
**Author:** Catapultam

Deployed
```
- Pets survive death again (frfr)
- Parcel purchases work again
```

---

---

<a name="entry-1305908449619607663"></a>

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

<a name="entry-1305393437985734676"></a>

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

<a name="entry-1305270536628338759"></a>

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

<a name="entry-1304979313254207538"></a>

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

<a name="entry-1304647984100806717"></a>

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

<a name="entry-1303902189189857281"></a>

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

<a name="entry-1303619142045143072"></a>

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

<a name="entry-1303530351636774976"></a>

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

<a name="entry-1303442945671692420"></a>

## 2024-11-05 19:36 - Entry 1303442945671692420
**Author:** Catapultam

@here

```
- Fixed zone crashes
```

---

---

<a name="entry-1303422359621079101"></a>

## 2024-11-05 18:15 - Entry 1303422359621079101
**Author:** Catapultam

Deployed
```
- New global buff system (Thanks @Secrets)
- Fishing can result in Enchanted and Legendary items
```

---

---

<a name="entry-1303013816132440124"></a>

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

<a name="entry-1302710373446586460"></a>

## 2024-11-03 19:05 - Entry 1302710373446586460
**Author:** Catapultam

Pending
```
- Characters who are Rangers will display their Bow as their default weapon instead of their melee weapons.
- Discovery of Enchanted items will no longer trigger a world announcement.
```

---

---

<a name="entry-1302710180533899408"></a>

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

<a name="entry-1302321345014534207"></a>

## 2024-11-02 17:20 - Entry 1302321345014534207
**Author:** Catapultam

Pending on fresh zone servers
```
- Fixed crash related to moving bag contents
```

---

---

<a name="entry-1302291165894152242"></a>

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

<a name="entry-1302287329112756244"></a>

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

<a name="entry-1302047213064683530"></a>

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

