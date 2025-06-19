---
title: Changelog - August 2024
description: Changelog entries for August 2024
published: true
date: 2025-06-19T23:04:47.720Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:47.720Z
---

# Changelog - August 2024

[← Back to Recent Updates](/en/Change-log-history) | [← July 2024](/en/changelog-2024-07) | [September 2024 →](/en/changelog-2024-09)

---

*35 updates in August 2024*

<a name="entry-1279089267922178139"></a>

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

<a name="entry-1278501238148960351"></a>

## 2024-08-28 23:47 - Entry 1278501238148960351
**Author:** Catapultam

```
- Can consume higher-tier items (reg in PS, consume enchanted).
- attempt to fix pet taunt
```

---

---

<a name="entry-1278227086808715314"></a>

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

<a name="entry-1277511372816519231"></a>

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

<a name="entry-1276746251861229568"></a>

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

<a name="entry-1276566684332851331"></a>

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

<a name="entry-1276243407290761216"></a>

## 2024-08-22 18:15 - Entry 1276243407290761216
**Author:** Catapultam

```
* Implemented Client<->Server handshaking. You will be disconnected after a short period of time if you are not using the client modification plugin.
* Implemented improved MQ2 detection.
```

---

---

<a name="entry-1276194813896822829"></a>

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

<a name="entry-1276101765921509417"></a>

## 2024-08-22 08:52 - Entry 1276101765921509417
**Author:** Catapultam

```
* Lots of progress on cleaning up /who. Apparently I don't remember exactly how /rol and /anon work. More to come
```

---

---

<a name="entry-1276052667470188625"></a>

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

<a name="entry-1275678617942228993"></a>

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

<a name="entry-1275637372138295417"></a>

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

<a name="entry-1275628398600785940"></a>

## 2024-08-21 01:31 - Entry 1275628398600785940
**Author:** Aporia

```
Effective immediately:

- With the decrease of overall exp gain, hell levels have been removed.

- Exp loss on death has also now been removed.
```

---

---

<a name="entry-1275278018083815468"></a>

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

<a name="entry-1275275502965362720"></a>

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

<a name="entry-1274855094273310810"></a>

## 2024-08-18 22:19 - Entry 1274855094273310810
**Author:** Catapultam

```
Hateplaneb is now fixed
```

---

---

<a name="entry-1274778415710470184"></a>

## 2024-08-18 17:14 - Entry 1274778415710470184
**Author:** Retribution EQ #change-log

```
Hotfix:

Vulak is no longer rooted in place. It is highly recommended you pull him off his platform before engaging. Unless, of course, you enjoy lava.
```

---

---

<a name="entry-1274465896978448579"></a>

## 2024-08-17 20:32 - Entry 1274465896978448579
**Author:** Retribution EQ #change-log

```
Hotfix:
* Haste now applies to combat skills again. (Should fix timer bugs)
```

---

---

<a name="entry-1274023304469942294"></a>

## 2024-08-16 15:13 - Entry 1274023304469942294
**Author:** Catapultam

```
* Fury of Magic is no longer available to hybrids
* Fists of Steel no longer applies to 1HB weapons
```

---

---

<a name="entry-1273891017434726481"></a>

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

<a name="entry-1273377641671430257"></a>

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

<a name="entry-1273152817099706388"></a>

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

<a name="entry-1272971478454898777"></a>

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

<a name="entry-1271660020295270425"></a>

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

<a name="entry-1271499064210362481"></a>

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

<a name="entry-1271105399537537064"></a>

## 2024-08-08 13:59 - Entry 1271105399537537064
**Author:** Retribution EQ #change-log

Hot-Fix
```
* Fixed zone server crash when handing items to charmed pets.
* Attempt at fixing certain mobs from summoning you under the world.
```

---

---

<a name="entry-1270428849955405916"></a>

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

<a name="entry-1270068579076935785"></a>

## 2024-08-05 17:19 - Entry 1270068579076935785
**Author:** Retribution EQ #change-log

8/05/2024
```
* Reworked NTOV script to spawn Vulak
* Removed lockpicking requirement from Chardok Royals
```

---

---

<a name="entry-1269763708481962027"></a>

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

<a name="entry-1269450676338167808"></a>

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

<a name="entry-1269065307331493943"></a>

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

<a name="entry-1268648098918567937"></a>

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

<a name="entry-1268578766473527470"></a>

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

<a name="entry-1268577273339056153"></a>

## 2024-08-01 14:33 - Entry 1268577273339056153
**Author:** Retribution EQ #change-log

[Original Message Deleted]

---

---

<a name="entry-1268576992429605067"></a>

## 2024-08-01 14:32 - Entry 1268576992429605067
**Author:** Catapultam

Retribution EQ #change-log

---

---

