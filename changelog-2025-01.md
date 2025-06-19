---
title: Changelog - January 2025
description: Changelog entries for January 2025
published: true
date: 2025-06-19T23:04:26.941Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:26.941Z
---

# Changelog - January 2025

[← Back to Recent Updates](/en/Change-log-history) | [← December 2024](/en/changelog-2024-12) | [February 2025 →](/en/changelog-2025-02)

---

*16 updates in January 2025*

<a name="entry-1334900028866826271"></a>

## 2025-01-31 14:56 - Entry 1334900028866826271
**Author:** Catapultam

```
- Peridots are no longer marked NO VALUE
- Fixed Bag of Bartering prompt not displaying in some circumstances.
- Bag of Bartering prompt is now sorted by item stats and value, but may be truncated for large item lists.

- Reduced packet resend aggressiveness - This may help with connection stability for some users (@Akkadius)
```

---

---

<a name="entry-1334259808114839553"></a>

## 2025-01-29 20:32 - Entry 1334259808114839553
**Author:** Catapultam

```
- Updated to EQEmu v22.61.1
```
https://github.com/EQEmu/Server/pull/4617
https://github.com/EQEmu/Server/pull/4627

---

---

<a name="entry-1332857825009078393"></a>

## 2025-01-25 23:41 - Entry 1332857825009078393
**Author:** Catapultam

```
- Fixed Guild Member level display. (Client Patch Required)
```

---

---

<a name="entry-1332759507641827409"></a>

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
- All players with Tracking should now be able to filter track results (@Salty)
- Fixed memory leak in client which caused map to not properly reset spawn lists under some circumstances (@dannuic)
- Reduced the 'merchant multiplier' on most items.
- Fixed several memory leaks (@Akk)
- Re-enabled direct inventory delivery via Delivery Vouchers
- Adjusted client memory map in a speculative fix for out of memory client crashes (@Drake)

Quest Fixes:
- Quests fixes related to Qeynos Badge (@Trust)
- Implemented JFP War (@Trust)
- Cleaned up Shaman Cudgel & Skull quest (@Trust)
  - Added Flags to each step to monitor progress
  - Added faction and level checking per step
  - Added notice of flags being assigned (So they are not "Invisible")
  - Added Dialog to Oxyn "Progress" that will output current progress point.
  - Limited a quest turn-in that can be exploited for fast and unlimited EXP
- Misc Befallen cleanup (@Trust)
- Fixed Faction hits around Giant Scarab quests in Kaladim (@Trust)
- Various Quest fixes in qey2hh1 (@Trust)
- Corrected several quests which rewarded the wrong items.

- Added Mystic Soulbinding Apparatus to Gemcrafter Anuk This reusable device allows you to attune any item, preventing it from being accidentially sold or|| traded.

- Unflinching Resolve and Stalwart Endurance have been removed from the game.
- Any player that has a single point of Unflinching Resolve or Stalwart Endurance will be given Steadfast Will

- The vendor cost of items has increased as the sell value on some has increased.

```

---

---

<a name="entry-1332028783162818775"></a>

## 2025-01-23 16:46 - Entry 1332028783162818775
**Author:** Catapultam

```
- Items should now never be able to be sold for more than they are bought for.
- No-Rent items can not be sold via Bags of Bartering
- Custom Pet Names restored
```

---

---

<a name="entry-1331997123805184092"></a>

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
- Item Previews are now avaiable (alt-rightclick item icon in 'item inspect' window) (@dannuic)
```

---

---

<a name="entry-1331723721295003740"></a>

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

<a name="entry-1329893093335371877"></a>

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
- Instant-Cast clickies can be activated while singing bard songs (@Zimp)
- Improved logic around rune stacking with regard to bard songs (@Zimp)
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

<a name="entry-1329465177497665590"></a>

## 2025-01-16 14:59 - Entry 1329465177497665590
**Author:** Aporia

Pending Reboot:

```
- Typhoon Breath has had its curse counters cut in half and it's cooldown tripled.
```

---

---

<a name="entry-1329263425905229878"></a>

## 2025-01-16 01:38 - Entry 1329263425905229878
**Author:** Catapultam

NINJA CHANGELOG
```
- Polymorphist now properly accepts EoM
```

---

---

<a name="entry-1328936987754889247"></a>

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

<a name="entry-1328923023532752966"></a>

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
- Cycle Pet\Self hotkey will now cycle between all pets (@Salty)
- Removed servers other than THJ from server list (@Splose)

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

<a name="entry-1327449601371934735"></a>

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

<a name="entry-1324929653957328956"></a>

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
- Traders should now be cleaned up if a zone server crashes (@Neckkola)
- Fixed a memory leak in pet bags
- All Handin quests should now work

```

Additionally; it is now possible for us to update quest scripts to allow handing in stacks at a time. This requires reworking the script, however, and so will not be a global change.

We are crowdsourcing quests which would benefit from this treatment -> [Here](https://docs.google.com/document/d/1D-BxDDT6pFQHfxA6dcqdbxU9f2mMFgvtZbTvMomF47E/edit?tab=t.0)

---

---

<a name="entry-1324112534776713266"></a>

## 2025-01-01 20:30 - Entry 1324112534776713266
**Author:** Aporia

Out of respect for player time and expected engagement, the following changes have been made:

```
- Non raid bosses in ToV have had their HP reduced.
- Thifling Focuser's in PoG have had their HP reduced.
```

---

---

<a name="entry-1324047001591091262"></a>

## 2025-01-01 16:10 - Entry 1324047001591091262
**Author:** Catapultam

```
- Implemented limit of 599 total active traders to work around client bug (More comprehensive workaround to come)
```

---

---

