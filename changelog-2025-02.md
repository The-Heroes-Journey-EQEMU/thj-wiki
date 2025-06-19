---
title: Changelog - February 2025
description: Changelog entries for February 2025
published: true
date: 2025-06-19T23:04:23.097Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:23.097Z
---

# Changelog - February 2025

[← Back to Recent Updates](/en/Change-log-history) | [← January 2025](/en/changelog-2025-01) | [March 2025 →](/en/changelog-2025-03)

---

*11 updates in February 2025*

<a name="entry-1341103053197283349"></a>

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

<a name="entry-1339745754541064212"></a>

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

<a name="entry-1339477902109966367"></a>

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

<a name="entry-1338759014258970654"></a>

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

<a name="entry-1338412565780238357"></a>

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

<a name="entry-1338377526820601906"></a>

## 2025-02-10 05:14 - Entry 1338377526820601906
**Author:** Catapultam

```
- Various spells and songs corrected to have haste instead of Slay Undead
- Lord Inquisitor Seru now correctly uses certain abilities if he has the support of any of his Praeserti
- Lord Inquisitor Seru's death reward event will now fire more reliabily
- Many fixes to various encounter scripts (@Trust, @Zimp)
- Removed Fling effect from Battle Leap (@Aporia)
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

<a name="entry-1337893727150014565"></a>

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

<a name="entry-1337209418198286398"></a>

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

<a name="entry-1337208133201690625"></a>

## 2025-02-06 23:47 - Entry 1337208133201690625
**Author:** Catapultam

THIS CHANGELOG IS FOR LUCLIN RELEASE AND IS NOT COMPLETE

```
- Updated to EQEmu 22.62.2
- 'Improved the netcode' (@Akkadius)

Fixes:
- Purify Body should now work as expected (@Fluff)
- BoBs will no longer sell to any merchant regardless of faction
- Players entering or leaving the zone in a Non-Respawning instance with more than 2 members will no longer cause mobs to heal
- Faded Memory should spawn for Zlandikar and the other guy
- Items with slots incorrectly set to only allow one wrist have been corrected to allow both wrists.
- Fix zone crash that could occur when a script not directly attached to an NPC could instruct a recently dead NPC to Move to a new location.
- Various NPCs will no longer flee when kicked.
- Certain tradeskill recipes will no longer return incorrect items via Salvage AA (@Trust)
- Fixed various luclin encounters (thx @Trust, @Zimp, others)
- Gnomes can now acquire Tinkering Mastery AA
- Fixed a number of Haste spells that were actually Slows (Bards, Rejoice!)
- Fixed Reverse DS effects not working
- Doppelgangers will no longer use ranged attacks, they will only cast spells.

Changes:
- Languid Bite and Deep Sleep should now trigger off AA casts (@Zimp)
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

<a name="entry-1336033147346878590"></a>

## 2025-02-03 17:58 - Entry 1336033147346878590
**Author:** Catapultam

Posting this early because it went out early
```
- Updated Default Maps (@Lachadan)
- Added Dark Mode maps option (dropdown menu in map window) (@Lachadan)
```

---

---

<a name="entry-1335823574799224852"></a>

## 2025-02-03 04:05 - Entry 1335823574799224852
**Author:** Aporia

```
- The Echo of the Past for Nagafen's Lair, Permafrost, and Velketor's lab have been moved inside their respective zones.
- If you see an Echo of the Past in Lavastorm or Everfrost, please ignore them and zone in to the respective zone to pull your DZ.
- Great Divide still has an Echo of the Past but it is now at the succor location to the south of the zone and is meant to spawn a DZ for Great Divide itself.
```

---

---

