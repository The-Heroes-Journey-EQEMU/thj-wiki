---
title: Change Log History
description: History of THJ Change Logs
published: true
date: 2025-03-06T20:51:25.764Z
tags: changelog, changes, patch notes
editor: markdown
dateCreated: 2025-02-28T01:34:47.144Z
---

![change-logs.webp](/change-logs.webp){.align-center}
# Change-Log
(Feb 23, 2024 – Mar 6, 2025)


> Updated last at second date on title above.



## The Heroes' Journey Change-log (Oldest to Latest)

[Jump to Bottom for latest updates](#bottom)


## (oldest) Fri Feb 23 2024 — Posted by: catapultam\_habeo

-   Hello!
-   Fixed the No-XP bug
-   Fixed base mana regen
-   Fixed crash on interacting with GM

## Sat Feb 24 2024 — Posted by: catapultam\_habeo

-   Disabled corpses for now to work around a crash bug

## Sun Feb 25 2024 — Posted by: catapultam\_habeo

-   Re-enabled corpses
-   Disabled quests from checking corpses for items (lag fix)
-   You can now zone out of the Bazaar using a means other than the zone line
    -   Expected behavior: zone lines take you to your portal source. If none, you go to nexus (if Luclin unlocked) or your bind point otherwise.
    -   Leaving the zone by any method other than a zone line resets your saved portal source.
-   Corrected zoning into Highpass (New version for now)
-   Implemented Faded Writ quest
-   Removed all Fabled mobs from spawn lists

## Tue Feb 27 2024 — Posted by: catapultam\_habeo

-   Disciplines no longer cause crash on zone
-   Implied targeting improved (corpses, procs)
-   Pet buffs & heals no longer force change target to pet

## Wed Feb 28 2024 (02:13:39) — Posted by: catapultam\_habeo

-   Fixed Lavastorm (repatch needed)
-   Fixed patcher weirdness
-   Abysmal Sea is accessible
-   Added LoY, DoN, OoW, GoD zones to progression lockouts
-   Any tag (Latent, Potent, Awakened) can be used for quest turn-ins
-   All AA are instant-cast
-   Fading Memories now uses mana
-   Added Phinigel Autropos to Kunark unlock targets
-   Attempting to zone to a disallowed zone drops you in the nexus
-   Several bug fixes
-   Neriak waypoint fixed
-   Fixed pet buffs suspending after zoning
-   Fixed detrimental spells suspending

## Wed Feb 28 2024 (12:51:31) — Posted by: catapultam\_habeo

**Pending Reboot**

-   Added:RULE\_INT(Spells, DOTsScaleWithSpellDmgPerTickPercent, 0, ...) RULE\_INT(Spells, HOTsScaleWithHealAmtPerTickPercent, 0, ...) RULE\_INT(Spells, PetsScaleWithOwnerPercent, 0, ...)    

## Wed Feb 28 2024 (15:45:04) — Posted by: catapultam\_habeo

**Patch Required**

-   Merchantlist filter now accounts for your classes
-   Spell scroll levels no longer wonky for shared spells

## Wed Feb 28 2024 (20:59:49) — Posted by: catapultam\_habeo

-   Switching base class no longer required for any class combos
-   Please report spellcasting problems as high priority
-   Humans/Iksar with Monk in their composition appear as Monks

## Thu Feb 29 2024 (13:03:55) — Posted by: catapultam\_habeo

-   Reverted “humans look like Monk” for now
-   Restored original UI
-   Custom UI can be loaded with `/loadskin thj_ui`

## Thu Feb 29 2024 (14:24:58) — Posted by: catapultam\_habeo

-   Soulbinders also offer gates to Bazaar and bind

## Thu Feb 29 2024 (16:54:41) — Posted by: catapultam\_habeo

-   Improved merchant filtering (patch needed)
-   All activated abilities are instant-cast (patch + reboot)
-   Augments no longer require distillers to remove (reboot)

## Thu Feb 29 2024 (17:23:14) — Posted by: catapultam\_habeo

-   Added MIT and AVG stats to inventory (actual mitigation/avoidance AC after softcap)

## Thu Feb 29 2024 (18:17:22) — Posted by: catapultam\_habeo

-   Tradeskills always return (Awakened) items
-   Removed (Latent) tag from normal-quality gear (now untagged)
-   Renamed (Potent) tag to (Latent)

## Thu Feb 29 2024 (19:59:48) — Posted by: catapultam\_habeo

-   Added a large number of waypoints in Classic & Kunark
-   Adjusted respawn frequency of all mobs

## Fri Mar 01 2024 (02:01:01) — Posted by: catapultam\_habeo

-   Characters in the Bazaar are exempt from IP box limits

## Fri Mar 01 2024 (23:36:39) — Posted by: catapultam\_habeo

-   Tradeskills can now be done with any mix of untagged/latent/awakened components

## Sat Mar 02 2024 (22:41:22) — Posted by: catapultam\_habeo

-   Increased the rate of upgraded versions of items dropping

## Sun Mar 03 2024 (04:12:54) — Posted by: catapultam\_habeo

-   Augments are now All/All

## Sun Mar 03 2024 (05:47:39) — Posted by: catapultam\_habeo

-   Added Latent/Awakened bags (next reboot)
-   SolB, Permafrost, Kedge instances available
-   **Instancing (Heroes’ Journey):**
    -   “A Servant of the Journey” near or inside raid zones
    -   Two instance types: Challenge (non-respawning) or Opportunity (respawning)
    -   Each instance limited to 6 characters, lasts 24 hours
    -   Challenge: for players without the progression flag or below recommended level; rewards “Accolades of Heroism”; 20-hour lockout
    -   Opportunity: 20-hour lockout, direct copy of zone, available after completing Challenge at least once

## Mon Mar 04 2024 (20:42:44) — Posted by: catapultam\_habeo

-   Mixed Latent/Awakened/Untagged quest turn-ins now REALLY work
-   You can no longer zone into DoN or OoW zones

## Tue Mar 05 2024 (21:25:06) — Posted by: catapultam\_habeo

-   Added `/mapfilter` (thanks @Voidless)
-   Added click-to-target on map for mobs you can detect
-   Updated patcher to recognize LAA eqgame.exe

## Wed Mar 06 2024 (13:26:11) — Posted by: catapultam\_habeo

-   Non-Weapon Instruments that can be Primary/Secondary can also be equipped in range/ammo (ammo does nothing)

## Wed Mar 06 2024 (14:35:51) — Posted by: catapultam\_habeo

-   Added Pet Discipline to starting AAs for Mages, Necros, Beastlords, Enchanters, Shamans
-   Added Advanced Pet Discipline for Mages & Necros
-   Starting AAs reapplied on zone if missing

## Wed Mar 06 2024 (18:57:23) — Posted by: catapultam\_habeo

-   Progression flags can be acquired from any version of Naggy/Vox/Phinny

## Fri Mar 08 2024 (14:33:04) — Posted by: catapultam\_habeo

-   Slightly increased base XP rate
-   Greatly increased AAXP rate
-   Increased modifiers for Red/Yellow
-   Decreased modifiers for Blue/Light Blue/Green

## Fri Mar 08 2024 (14:33:58) — Posted by: catapultam\_habeo

-   Deleted a door

## Sat Mar 09 2024 (12:21:12) — Posted by: catapultam\_habeo

-   Delay on debuffs removed
-   Pet spell messages working
-   Added pet resist and DoT messages
-   Applying charm no longer strips your debuffs

## Thu Mar 14 2024 (22:43:11) — Posted by: catapultam\_habeo

-   Content DB more closely aligned with Retribution

## Thu Mar 14 2024 (23:10:22) — Posted by: catapultam\_habeo

-   AA cast time is 0 again
-   Adventurer’s pack increased to 18 slots (will revert to 12 on next server wipe)

## Fri Mar 15 2024 (03:24:19) — Posted by: catapultam\_habeo

-   Fixed Lavastorm zone lines (must delete `lavastorm.eqg` manually)

## Fri Mar 15 2024 (18:55:58) — Posted by: catapultam\_habeo

-   Focus Effects should now work
-   Monks can dual-wield empty-handed
-   Monk epic affects empty-hand H2H
-   Group Buffs affect charmed pets

## Wed Mar 20 2024 (23:41:12) — Posted by: catapultam\_habeo

-   Sympathetic Procs no longer trigger except from spell gems
-   Sympathetic Procs do not trigger from bard songs

## Wed Mar 27 2024 (23:29:21) — Posted by: apor1a

**Pending Reboot**

-   Emperor SSRA is now a Unique Spawn
-   Monk FoS AA is now H2H only
-   Bard song cap corrected to mimic Ret

## Fri Mar 29 2024 (11:35:23) — Posted by: catapultam\_habeo

-   Corrected `/who` formatting
-   Out-of-range mobs no longer labeled “Mob” on map (memory leak fix)
-   Spell inspect window displays cast time

## Fri Mar 29 2024 (14:41:58) — Posted by: catapultam\_habeo

**Pending Reboot**

-   Focus effects now work
-   Spell Damage/Heal Amount limited so as not to exceed double base
-   Sympathetic procs scale with cast time + mana cost

## Sat Mar 30 2024 (11:20:39) — Posted by: catapultam\_habeo

-   Faction checks now use the best modifier among your unlocked classes

## Sat Mar 30 2024 (12:33:00) — Posted by: catapultam\_habeo

**Pending Reboot**

-   Buff stacking adjusted: short vs. long buffs no longer conflict
-   Detrimental vs. Beneficial no longer conflict
-   Casting skills only increase from spells cast via spell gems
-   Bard Songs no longer fade if they run out of Rune capacity
-   Re-introduced Extended Pet Affinity (instant heals/cures included)
-   Instrument modifiers no longer scale incorrectly

## Mon Apr 15 2024 (21:52:40) — Posted by: catapultam\_habeo

-   THJ now officially running entirely off Retribution’s database

## Tue Apr 23 2024 (02:58:11) — Posted by: catapultam\_habeo

**PENDING REBOOT**

**Bugfixes:**

-   Fixed Saryrn & Quarm (GoD, Fabled Naggy) flags
-   Ancient Cragbeast Matriarch no longer causes disconnects
-   Several misc bugfixes
-   Pet bag no longer endlessly upgrades
-   AA instant-cast again
-   All versions of Intricate Wooden Figurine awarded if eligible

**New Features:**

-   Bazaar Portal returns you to last used location if used in Bazaar
-   Items may be Parceled
-   Apocrypha in Bazaar can “buff” the drop-upgrade rate globally for 4 hours

## Tue Apr 23 2024 (09:13:56) — Posted by: Retribution EQ #change-log

**Bugfixes:**

-   Fixed Saryrn & Quarm (GoD, Fabled Naggy) flags
-   Ancient Cragbeast Matriarch fix
-   Misc bugfixes
-   Muzzle of Mardu no longer usable by players

**New Features:**

-   Bazaar Portal returns you to last location if used in Bazaar
-   Items may be Parceled
-   Apocrypha can buff upgrade rate for 4 hours (world-wide effect)

## Wed Apr 24 2024 (23:11:13) — Posted by: Retribution EQ #change-log

-   AoR for Yxxta moved
-   Enchanter pets >55 have increased damage
-   Necro AA Death Bloom at 51
-   Classic Rogue poisons truly have 50 charges
-   Rathe Council banishes are instance-aware
-   Removed backstab damage from weapons (now uses weapon base damage)
-   Monks start with Rk I Techniques of Master Wu (was Stonewall)
-   All pet classes start with Pet Discipline
-   Tendrils of Fire hits for 450 with -450 resist mod
-   Vrabbit Xloren instance aware for ports
-   Ranger AA Trickshot Rk I: 5% (was 2%), +2% per rank
-   All RC & Apoc weapons have correct +10%/+20% proc mods
-   There is now only one Vacto

## Sun Apr 28 2024 (19:18:15) — Posted by: Retribution EQ #change-log

-   Bazaar NPC overhaul (more natural arrangement)
-   Check the back stalls for GMs, Spell Vendors, and Tomes

## Tue Apr 30 2024 (16:01:07) — Posted by: catapultam\_habeo

**Beta branch**

-   Renamed Latent → “Enchanted” and Awakened → “Legendary”
-   Implemented Dynamic Items (runtime-created, not sellable to NPC, etc.)
-   Implemented Artifacts (chance when receiving Legendary via loot/tradeskill/quest)
-   Implemented “Leveling” items in Power Source slot (blocks player XP, item upgrades from Normal → Tier1 → Tier2)

## Tue Apr 30 2024 (22:47:57) — Posted by: catapultam\_habeo

-   Leveling up an item triggers a Discovery event
-   Leveling to Legendary can produce an Artifact
-   Fixed logic around discoveries/artifacts

## Wed May 01 2024 (00:13:27) — Posted by: catapultam\_habeo

-   Auto-looting no longer places items in the Power Source slot
-   Added feedback for how much item XP you gain

## Thu May 02 2024 (13:11:59) — Posted by: catapultam\_habeo

-   Fixed feedback for item XP gain
-   Adjusted item XP rate
-   Combat effects on items can trigger on spell casts
-   Spell Damage/Heal Amount limited to 2× base value
-   Fixed discovery message spam
-   Reduced bard song proc rate
-   Artifacts are explicitly droppable
-   Fixed artifact discovery from item XP
-   Fixed LoS on combat abilities (@Maze)
-   Ranged attacks can proc bows (@Maze)

## Fri May 03 2024 (03:18:47) — Posted by: catapultam\_habeo

-   Rewrote implied targeting again
-   Fixed expanded pet affinity killing some pets
-   Combat procs only trigger on damage/healing spells

## Sat May 11 2024 (02:37:30) — Posted by: catapultam\_habeo

-   Maybe fixed “sleeping ogre” bug

## Sun May 12 2024 (14:32:01) — Posted by: Retribution EQ #change-log

**Pending reboot**

-   Fixed Gram Dunnar giving Intricate Wooden Figurine
-   No more multiple completions of Tome of New Beginnings
-   Fixed Paladin checks in quests
-   Fixed Monk checks in many quests
-   Quarm awards GoD flag if you lack it

## Sun May 12 2024 (16:52:51) — Posted by: catapultam\_habeo

-   Artifacts no longer become no-drop if you zone with them equipped
-   Augments can no longer be dynamic items (Artifacts)
-   Discovery tag on Artifacts references the person who discovered the Legendary variant
-   Artifacts of items with charged abilities have unlimited charges, must be equipped; cast time is max(5s, actual)

## Sat May 18 2024 (19:47:32) — Posted by: Retribution EQ #change-log

**Pending Patch**

-   Enchanter AA Illusions of Grandeur: Crit DoT = 200% (was 110%), Crit Nuke = 200% (was 250%)
-   Enchanter AA Doppelganger Rk I/II stats corrected
-   Enchanter AA Eldritch Rune now castable on others
-   Enchanter spell Cajoling Whispers sold by Illusionist Jerup in Bazaar
-   All Disciplines lacking hastened AA have 15min CD
-   All AA lacking hastened AA have 15min CD
-   Warrior AA Infused by Rage is active & permanent until clicked off
-   Tearel’s Waypoint list is now sorted properly

## Sun Jun 02 2024 (21:16:15) — Posted by: Retribution EQ #change-log

**Pending Patch**

-   Halved mana/cast time/CD for Calliav line (MAG, NEC, BST)
-   Magician Sol Ro pet items (Pet Power 5) & Planar (Pet Power 10) bigger effect
-   Necro Epic & Encyclopedia Necrotheurgia’s Minion of Hate more noticeable
-   All Mage pets (≥29) benefit from Pet Power similar to epic
-   Velious drop Essence of Nature has Summoner’s Boon (Pet Power 15)
-   BST Pet Spirit spells rearranged
-   BST AA Bite of the Asp Rk I = 25 dmg/tick +1/level; Chameleon Strike Rk I base 25 dmg
-   MNK AA Imitate Death: 12min CD minus 2 each rank, 50 End, can be 0
-   Chloroblast level req = 59 for RNG/BST
-   Warrior AA Infused by Rage stacking fix attempt
-   Blood of Ssra is unique spawn
-   Items no longer vanish from cursor when zoning
-   Urthron’s Ultimate Unattuner works again
-   Steamfont minotaurs no longer hoard gems

## Tue Jun 04 2024 (02:49:31) — Posted by: catapultam\_habeo

-   Experimental fix for Artifacts not retaining persistent ItemIDs

## Wed Jun 19 2024 (15:15:45) — Posted by: Retribution EQ #change-log

**Pending reboot/patch**

-   LGuk DZ fixed
-   Ghoulbane drops from Shin Lord again
-   Infused by Rage display error maybe fixed
-   Note for Janam quest in E/W Freeport fixed
-   Item ID fixes for 6th Necro Skullcap quest
-   Removed LoY noob quest NPCs
-   Skyshrine key no longer required to reach Cobalt Scar
-   Removed duplicate Chardok agents
-   Zlandicar is a dragon again
-   Waypoints added: Chardok, Great Divide, Fungus Grove, Tenebrous
-   Donation Vendor added (will accept EoM soon)
-   Improved Damage I/II reactivated on ~20 items
-   Enchanter Doppelganger AA working, adjusted stats, casts a DD
-   Enchanter AA Deep Sleep 20/40/60/80/100% chance per rank
-   Druid AC-debuff spells now scale with level
-   Necro/Mage pet buff lines scale properly
-   Mistmoore, LGuk, Unrest, CoM now have DZs
-   Shared bank does not accept plat
-   Dire Charm works on any light blue that can be charmed
-   Veksar unlocks with Luclin
-   Necro AA Cascade of Decay coexists with sympathetic strike buffs
-   Fabled Naggy only reached by Sage of Anachronism in Bazaar

## Sat Jun 22 2024 (15:57:19) — Posted by: Retribution EQ #change-log

**Welcome to Season 1!**

-   Seasonal Characters (#disable\_seasonal confirm to opt out)
    -   (Season 1) Start with First Orb of Retribution & Portable Hole (growable 20-slot bag)
    -   Greatly increased chance for Apocryphal/Rose-Colored drops
    -   Additional progression rewards
    -   Cannot group/trade/spell with non-Seasonal, limit 6 in DZ, etc.

**General Changes**

-   All prior pending changes now active
-   NPCs do not retain items handed to them (destroyed), except charmed pets equip a copy and return item
-   Agents of Retribution → Echo of the Past with two instance types (respawning/non-respawning)
-   Dire Charm works on any mob up to light blue

**Bug Fixes**

-   Polymorphist & Purveyor of Glamour fixed

**Donation Rewards**

-   New Bazaar merchant for Echo of Memory (EoM) currency
-   Sells 20/30/40-slot no-drop bags in 10 colors, unattuners, illusions
-   Items can be sold back for a small loss

## Sun Jun 23 2024 (15:02:17) — Posted by: Retribution EQ #change-log

-   Vah Shir, Iksar, Beastlords, Berserkers now available from start
-   Rogue Epic no longer completable in Classic (will return in Kunark)
-   SK 51 AA was pointing to wrong file, fixed next patch

## Tue Jun 25 2024 (00:10:05) — Posted by: catapultam\_habeo

-   Implemented Implied Targeting for `/pet attack`

## Wed Jun 26 2024 (09:31:06) — Posted by: Retribution EQ #change-log

-   Beastlords now correctly get Feral Swipe before Frenzied Swipes as seasonal AA
-   **Pending reboot**: Drelzna can drop Jboots
-   Najena getting DZ for JBoot fans

## Thu Jun 27 2024 (12:06:18) — Posted by: Retribution EQ #change-log

**Pending Reboot**

-   Hate 2.0 items scaled slightly lower so future content not trivial
-   Manastone cast time = 1s but 10× effectiveness
-   Reagent requirement removed from Enchanter runes; cast times reduced

## Wed Aug 14 2024 (01:34:45) — Posted by: Retribution EQ #change-log

-   Tearel Overhaul:
    -   Can attune map to any discovered destination
    -   Can attune to your expedition using EoM
    -   If you previously unlocked group ports, Tearel can do expedition returns

## Wed Aug 14 2024 (16:28:07) — Posted by: Retribution EQ #change-log

-   “Bazaar and Back” puts you at a semi-random spot in Bazaar
-   “Bazaar and Back” can prompt group members to join you
-   Pets no longer become giant/unshrinkable
-   Pet names are now static & reorganized

## Fri Aug 16 2024 (02:28:06) — Posted by: Retribution EQ #change-log

-   Combat Fury normalized for all classes that get it
-   Veteran’s Wrath normalized for all relevant classes
-   Mastery of the Past fully available to all casters
-   Shield Block fully available to all shield-using classes
-   Spell Casting Subtlety fully available to all casting classes

## Wed Sep 19 2024 (04:03:05) — Posted by: Retribution EQ #change-log

**Pending Patch**

-   Instruments show correct Resonance for item tier
-   Tier1/Tier2 items always “Magical”
-   Bard Epic instrument effect corrected
-   Bash reuse timer respects haste
-   Fixed clockwork summons
-   Fixed wizard swords/cleric hammers
-   Beastlords, Berserkers added to old-world items missing them
-   Reduced cooldown of Bestial Alignment
-   SE\_MeleeLifetap applies to SpecialAttackDamage
-   Fixed container slots for Strike of Shissar N poisons

## Thu Sep 19 2024 (16:35:18) — Posted by: catapultam\_habeo

-   Fixed Disc timers
-   Removed references to LDON camps
-   Misc bug fixes
-   FD no longer cures debuffs
-   Pet debuffs removed on resting (except from owner for charm)
-   Pet bag + multiple pets improved
-   Project Illusion works on pets
-   Non-1hp backstab damage fixed
-   Power Source no longer applies stats
-   Improved stacking for multi-class procs
-   DS stacking improved across classes

## Sat Sep 21 2024 (16:22:55) — Posted by: catapultam\_habeo

-   Only must-equip clickies become attuned if used from inventory
-   Multiple quest script fixes
-   “Honey, I shrunk the bats.”

## Wed Oct 09 2024 (19:18:35) — Posted by: catapultam\_habeo

-   Vision of Ayonae added to Bazaar:
    -   If exactly 1 class, you can add 2 random classes
    -   If more than 1 class, you can remove one (cost in EoM, 1-day cooldown)
    -   Any skills/spells/discs/AA from removed class are wiped

## Fri Oct 11 2024 (14:42:50) — Posted by: catapultam\_habeo

-   Experimental fix for “noloot/nocast” bug
-   Misc bug fixes

## Sat Oct 12 2024 (18:24:03) — Posted by: apor1a

**Pending Reboot**

-   Fixed random pet buff issues on resummon

## Wed Oct 23 2024 (03:41:07) — Posted by: catapultam\_habeo

-   Removed lockouts from respawning instances
-   Raid/Flag bosses do not spawn in respawning instances
-   Non-Respawning instance difficulty scales if more than 2 players
-   No adding players once progression flag mob spawns

## Thu Oct 24 2024 (13:53:51) — Posted by: apor1a

-   Frenzied Burnout AA cost reduced
-   Elemental Earth AA exploit fix
-   NPC melee interrupt rate reduced
-   Sarkis Ebonblade now talks to SK properly

## Thu Oct 24 2024 (14:17:26) — Posted by: catapultam\_habeo

**(In progress)**

-   1-hour lockout on respawning instances
-   Added Hand of the Gods proc to cleric epic
-   Power Source improvement rate adjusted
-   Fixed Rage Volley casting animation
-   Disciplines properly start timers if used while casting
-   Spell haste display fix
-   Pet melee mitigation fix
-   AAEXP at level 1
-   Max level = 50 during Classic
-   Echo buffs scale by level more suitably

## Sat Oct 26 2024 (01:45:30) — Posted by: apor1a

-   Assassinate can trigger at level 50
-   Buffs that affect spell crit damage now stack
-   Reaching level 50 auto-grants one class AA
-   Main task now requires level 50 (was 51)
-   Echo of the Brood server buff glitch fixed
-   Dreadlands Echo limited to Dreadlands only
-   Fists of Steel renamed “Way of Steel”; procs off kicks/strikes, no longer boosts H2H

## Sun Oct 27 2024 (14:52:19) — Posted by: apor1a

-   All auto-granted starting AAs have cost 0 so total AA count matches
-   Cleric starts with Purify Soul AA (15m CD) instead of Twincast
-   Druid starts with Entrap, no Paralytic Spores
-   Druid/Necro no longer begin with Critical Affliction
-   Druid/Necro/Ench/Shaman get innate 3% DoT crit
-   Ench/Shaman start with Destructive Cascade
-   Bow/throw skill raises Offense
-   Spell crit chance & bonus stack properly
-   Deprecated channels removed (Support, Bug, LFG remain default)
-   Warrior/Berserker starting quest item adjusted
-   Bard Discipline Deftdance CD reduced, new Hastened AA
-   Consume Item AA description updated

## Mon Oct 28 2024 (19:43:51) — Posted by: catapultam\_habeo

-   Per-kill AAEXP cap by con/level; rate buffs can raise cap
-   Reduced XP needed to improve items to (Enchanted)
-   Pet gear/buffs no longer fade when zoning
-   Marsingers 3/4 require Kunark
-   Removing classes updates player profile properly
-   Echo of the Brood adds small spell haste
-   All auto-granted AAs cost 0
-   Cleric has Purify Soul (15m), no Twincast
-   Druid has Entrap, no Paralytic Spores
-   No initial Crit Affliction for Druid/Necro
-   Druid/Nec/Ench/Shm have 3% DoT crit
-   Ench/Shm have Destructive Cascade
-   Bow/throw raises Offense
-   Crit chance + bonus stack
-   Removed old channels
-   Warrior/Berserker starting item adjusted

## Tue Oct 29 2024 (17:10:58) — Posted by: catapultam\_habeo

-   Deployed fixes: some NPC quest text, charm breaks, Way of Steel (Monk tweak)
-   Added more starting port locations
-   Charm spells can be refreshed
-   Removed certain ambient noises
-   Can use autofire/throw while Bard songs cast
-   Guild Management window shows correct classes
-   Lifetaps can crit heal again

## Wed Oct 30 2024 (14:44:57) — Posted by: catapultam\_habeo

**Pending**

-   Removing a class also removes spells only if truly invalid
-   AAXP settings preserved on zone
-   Project Illusion works on all pets

## Wed Oct 30 2024 (15:55:53) — Posted by: apor1a

-   EoM cost reduced from 5 to 2 for The Mischievous Halfling & Purveyor of Glamour
-   Death tip matches THJ gameplay
-   New “friends” at the campfire
-   Website updated

## Wed Nov 20 2024 (17:18:38) — Posted by: apor1a

-   Many AA descriptions updated (thanks Alebrije)
-   Bard song aggro reduced to 25% of old cap
-   Extended EXP bonus turned off
-   Grand Master Lozz no longer references Apocrypha
-   Kurn’s Tower DZ doesn’t drop you in the middle of the zone

**Pending Patch/Reboot**

-   Wizard AA Improved Familiar uses correct drake rank 3/4 (not skeleton)
-   Form of Black Wolf matches Spirit of Black Wolf duration
-   Enchanter AA Mana Draw recast fix
-   Legendary items missing heroics are fixed
-   NPCs >1h spawn time needed for epics but no personal DZ are reduced to 1h
-   Parcel NPCs added to more city zones
-   All Soulbinders immune to damage
-   Important EC tunnel NPCs immune to damage

## Fri Nov 29 2024 (19:14:06) — Posted by: apor1a

-   Scale/Chain armor with missing graphics fixed
-   Hastened Celestial Hammer prereqs removed
-   More AA descriptions updated
-   Misc quest fixes
-   Echo added to Kaesora
-   Tangrin respawn lowered
-   Account actions re: custom MacroQuest usage
-   Turkeys no longer lore; now no-drop
-   Pumpkin Spice Latte no-drop
-   Turkeys/Pumpkin Spice from mobs til Sunday night
-   Echo added to Highpass
-   Quest EXP temporarily disabled

## Sat Nov 30 2024 (13:05:16) — Posted by: catapultam\_habeo

**Deployed: Client + Server updates**

-   Fix for “You can’t use that command right now…” while spamming Disciplines
-   Another fix for that same error
-   Doubled target range on map
-   Improved map performance
-   Prevent slow effects from setting skill timers >80 years
-   Situational Awareness AA → effective skill (not skill points)
-   Haste displays from 0% up
-   Haste no longer over-applies to Kick/Bash/Backstab
-   Master Wu / Strikethrough / Stun messages → “Skills” filter
-   Dispel no longer lags certain players
-   Pets prefer primary/secondary equip
-   Polymorphist allows changing Deity or resetting pet name
-   Solomen responds properly
-   Tomekeeper Dahl no longer eats items from non-Monks
-   Deep no longer eats items from non-Monks

## Sat Nov 30 2024 (22:27:33) — Posted by: apor1a

-   Omat Vastsea quest can re-summon Natasha for Cleric epic fix
-   Natasha is now immune to player damage
-   Thanks Grig

## Sun Dec 01 2024 (00:03:46) — Posted by: apor1a

-   `/friend` works again
-   `/ignore` works again
-   Thanks @Akk

## Sat Dec 07 2024 (01:26:03) — Posted by: catapultam\_habeo

**Rolling Deployment**

-   Spell damage messages show spell & pet owners
-   DoT damage uses normal non-melee hits
-   Possibly fixed Explorer path progression not unlocking flags

## Sat Dec 07 2024 (21:50:46) — Posted by: apor1a

**Deployed**

-   Extended Ingenuity AA enabled for Bards
-   Bladed Song is unresistable, new Rank II added
-   Dance of Blades → Bladewhirl proc has -100 chromatic, AC/resist debuff scales w/ level
-   Funeral Dirge → +10/15/20% physical dmg, duration doubled
-   Hastened Funeral Dirge (5 ranks) lowers CD to 10 min
-   Song of Stone pet stats & CD improved
-   Overall buffs to Bard support viability

## Sun Dec 08 2024 (11:19:27) — Posted by: catapultam\_habeo

**Deployed**

### Quests

-   Revamp of “Thieves Aboard the Ship” (thanks @Trust)
-   Plane of Sky keys no longer removed on zone exit

### Bug Fixes

-   Apply MeleeLifeTap to Archery damage
-   Temporary stun immunity after being stunned applies to non-spell stuns
-   Flags consistent across zones
-   Worn ATK no longer double-counted
-   All DS from different classes stack properly

## Sun Dec 08 2024 (20:42:42) — Posted by: catapultam\_habeo

**Rolling Deploy**

-   Corrected Veterancy scaling formula near its max range

## Wed Dec 11 2024 (00:44:24) — Posted by: catapultam\_habeo

**Rolling Deploy**

-   Fixed SE\_GiveDoubleRiposte (Knave's Return Stab, Furious Refrain, Return Kick, etc.)
-   Probably fixed UCS issues again (@Akk)
-   Removing a class no longer removes spells if they remain valid via another class
-   Removing a class unequips items no longer usable

## Wed Dec 11 2024 (11:18:28) — Posted by: catapultam\_habeo

-   Removed Class Requirements from all epic quests (thanks @Prymetyme)

## Wed Dec 11 2024 (20:06:14) — Posted by: catapultam\_habeo

**Rolling Deploy**

-   Detrimental Sympathetic procs should no longer target the caster

## Mon Dec 30 2024 (16:54:57) — Posted by: catapultam\_habeo

> “I am a generous god.”

-   The Vision of Ayonae now lets you lower your level, then restore up to previous max
-   Cost: 500pp per level changed

## Tue Dec 31 2024 (13:04:17) — Posted by: catapultam\_habeo

-   Experimental change for /baz crash
-   Experimental change for crash-on-zone

## Tue Dec 31 2024 (13:17:18) — Posted by: apor1a

-   Enchanter AA Mana Draw → 10min CD w/ Rk3 Hastened Gathering
-   The Sleeper no longer resets to full HP upon roaring
-   Sleeper despawns adds from Phase 4 if players wipe & re-engage later
-   Misc Faction fixes (thanks @Trust)

## Sat Jan 25 2025 (18:41:08) — Posted by: catapultam\_habeo

-   Fixed Guild Member level display (Client patch required)

## Wed Jan 29 2025 (15:32:07) — Posted by: catapultam\_habeo

-   Updated to EQEmu v22.61.1
-   [GitHub Pull 4617](https://github.com/EQEmu/Server/pull/4617)  
     
-   [GitHub Pull 4627](https://github.com/EQEmu/Server/pull/4627)  
     

## Fri Jan 31 2025 (09:56:08) — Posted by: catapultam\_habeo

-   Peridots are no longer NO VALUE
-   Fixed Bag of Bartering prompt sometimes not showing
-   Prompt now sorted by item stats/value, might truncate large lists

## Thu Feb 02 2025 (23:05:58) — Posted by: apor1a

-   Echo of the Past for Nagafen’s Lair, Permafrost, Velketor is inside those zones
-   If you see an Echo in Lavastorm/Everfrost, ignore it & just zone in
-   Great Divide Echo moved near succor spot, for Great Divide itself

## Mon Feb 03 2025 (12:58:44) — Posted by: catapultam\_habeo

*Posted early because it went out early*

-   Updated Default Maps (@Lachadan)
-   Added Dark Mode maps option in the map window (@Lachadan)

## Thu Feb 06 2025 (18:47:43) — Posted by: catapultam\_habeo

> “THIS CHANGELOG IS FOR LUCLIN RELEASE AND IS NOT COMPLETE”

-   Updated to EQEmu 22.62.2
-   “Improved netcode” (@Akkadius)
-   Players gain temporary immunity to silence after being silenced
-   (Further notes incomplete)

## Sat Feb 08 2025 (16:12:01) — Posted by: apor1a

**Pending Reboot** (Reference to 10th Ring War, etc.)

## Thu Feb 13 2025 (01:06:58) — Posted by: apor1a

-   Doppelganger rework in progress: trying to let it use your current spells + original nukes
-   Thanks for your patience

## Thu Feb 13 2025 (18:51:19) — Posted by: catapultam\_habeo

-   Fixed regression in zone scaling (mobs no longer heal if someone enters/leaves)
-   Worg pets no longer visually hold weapons
-   Speculative fix for more stable glamour illusions
-   Adjusted Doppelganger spell priority/stacking
-   Adjusted pet aggro distribution (pet taunt toggles)

## Mon Feb 17 2025 (12:44:44) — Posted by: catapultam\_habeo

-   Consolidated Echo of Aegolism, Echo of the Grove, Echo of the Brood, Echo of Focus, Echo of Koadiac → Echo of Power
-   Replaced Knight’s Rebuke with Knight’s Return Strike (an existing AA)
-   Fixed Valentine’s Day event script errors
-   Prevented Forlorn Follower of Erolisi from replacing certain NPCs

## Thu Mar 6 2025 — Posted by: drakesward

- Small change to fix an ongoing issue with zoning into NRO

---

<p id="bottom"> </p>

---

![pagebreak5.webp](/pagebreak5.webp){.align-center}