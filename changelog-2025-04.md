---
title: Changelog - April 2025
description: Changelog entries for April 2025
published: true
date: 2025-06-19T23:04:14.700Z
tags: changelog, automated
editor: markdown
dateCreated: 2025-06-19T23:04:14.700Z
---

# Changelog - April 2025

[← Back to Recent Updates](/en/Change-log-history) | [← March 2025](/en/changelog-2025-03) | [May 2025 →](/en/changelog-2025-05)

---

*8 updates in April 2025*

<a name="entry-1363499720273821706"></a>

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

<a name="entry-1361550724663873648"></a>

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

<a name="entry-1359585216825655307"></a>

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
- Fixed an issue where spawn locations weren't being restored properly after zone state restoration. (@Akk)
- Fixed an issue where restoring an in-progress Plane of Time B instance would sometimes not restore properly. (@Akk)
- Fixed a scenario where sometimes players would not be able to enter certain open world zones while others would not experience said issue. (@Akk)
- Improved Bazaar search performance (@Akk)
- Prismatic Scale of the Elements (Legendary) is now Attunable instead of No Trade.
- Splinters of Time without a proc are now the correct aug type.
- Bard song aggro was incorrectly inflated. Fixed.
- Ranger archery bonus now correctly begins at 50 instead of 51.
- Hand of Ro now stacks with other -Fire Resist debuffs
- Pets can once again be issued commands from the default range.
- Xegony key will now Keyring
- Symbol of Torden will now Keyring
- Prevent pets from being added to mob hate lists if they are on hold (@Zimp)
- 2H Bash & Slam now works with Autoskill (@Duneathor)
- Reduced the Damage Shield component of Blessing of Praesertum Matpa
- Revamped 'Stats' page on Default UI
- /autoskill now supports Taunt
- Fixed inconsistencies around basic stat caps and certain spell effects
- Fixed pets with taunt off still pulling aggro
- Fixed pets with taunt off still eating rampage
- Fixed swarm pets not obeying custom pet restrictions (proc rate etc) (@Grek)
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

<a name="entry-1357601537861615697"></a>

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

<a name="entry-1357428075155165204"></a>

## 2025-04-03 18:54 - Entry 1357428075155165204
**Author:** Catapultam

```
- Re-Enabled Global Buffs
- Various backend performance improvements (@Akk)
- Zebuxoruk now drops minimum of Enchanted quality augments, and can rarely drop additional augments.
- Lord Inquisitor Seru has a higher probability of dropping additional loot based on the number of difficulty-enhancing buffs present on him
```

---

---

<a name="entry-1357226963760316516"></a>

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

<a name="entry-1356802123106357349"></a>

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

<a name="entry-1356635539750650037"></a>

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

