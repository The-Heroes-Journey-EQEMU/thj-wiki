---
title: FAQ Landing Page
description: A landing page for the various FAQ Pages
published: true
date: 2025-03-13T01:36:45.137Z
tags: faq, leveling path, leveling guide
editor: markdown
dateCreated: 2025-02-27T16:57:41.957Z
---

![faq2banner.webp](/faq2banner.webp){.align-center}

# **Frequently Asked Questions (FAQs)**

This FAQ serves as a comprehensive guide to The Heroes Journey (THJ), covering everything from game mechanics and troubleshooting to community features and customization options. Whether you're looking for technical support, gameplay tips, or information on specific in-game systems, you'll find answers here. Topics are organized alphabetically for easy navigation.

---

## **Table of Contents**

### **A**
- [Alternate UIs](#alternate-uis)
- [Armor Models](#armor-models)
- [Augments](#augments)

### **B**
- [Basic AA Recommendations for Each Class](#basic-aa-recommendations-for-each-class)
- [Basic Macros](#basic-macros)
- [Boss Not Spawning in DZ?](#boss-not-spawning-in-dz)
- [Bug Report](#bug-report)
- [Buying Spells](#buying-spells)

### **C**
- [Camera Views](#camera-views)
- [Troubleshooting: Can't Find File Specified](#troubleshooting-cant-find-file-specified)
- [Troubleshooting - Can't Unmem a Spell After Class Swap](#troubleshooting-cant-unmem-a-spell-after-class-swap)
  
### **D**
- [Do I Share AAs with Alts?](#do-i-share-aas-with-alts)
- [Do We Have a Wiki?](#do-we-have-a-wiki)

### **E**
- [Echoes of Memory](#echoes-of-memory)
- [EverQuest in Windowed Mode](#everquest-in-windowed-mode)
- [Expeditions/Dynamic Zones](#expeditions-dynamic-zones)

### **F**
- [Forum Activation Email for EQEmu](#forum-activation-email)

### **G**
- [Glamours for Weapons and Armor](#glamours-for-weapons-and-armor)
- [How Group Experience on THJ Works](#group-experience-on-thj)

### **H**
- [Having Lag/Stuttering Issues in Game?](#having-lag-stuttering-issues-in-game)
- [Heroic Stats](#heroic-stats)
- [How to Copy UI files between characters](#how-to-copy-ui-files)

### **I**
- [Incomplete Maps?](#incomplete-maps)
- [IP Exemptions](#ip-exemptions)

### **L**
- [Leveling Paths](#leveling-paths)

### **M**
- [Macro Items - The /Useitem Command](#macro-items-the-useitem-command)
- [Making a Trader](#i-want-to-make-a-trader)
- [More Teleport Options?](#more-teleport-options)
- [Mythbusting: Decapitate](#mythbusting-decapitate)

### **P**
- [Play on Mac](#play-on-mac)
- [Playing a Triple Pet/Minion Master](#playing-a-triple-pet-minion-master)

### **Q**
- [Quest Guides](#quest-guides)

### **S**
- [So You Want to Donate?](#so-you-want-to-donate)
- [Support Forum](#support-forum)
- [Sympathetic Strike/Healing](#sympathetic-strike-healing)

### **T**
- [The First Quest, What Do I Do?](#the-first-quest-what-do-i-do)
- [THJ Install Commands Explanation](#thj-install-commands-explanation)
- [Tentative Launch Schedule](#tentative-launch-schedule)
- [Titles](#titles)
- [Tracking: Situational Awareness and Tune of Pursuance](#tracking-situational-awareness-and-tune-of-pursuance)
- [Tribute](#tribute)
- [Troubleshooting: Can't Find File Specified](#troubleshooting-cant-find-file-specified)
- [Troubleshooting - Can't Unmem a Spell After Class Swap](#troubleshooting-cant-unmem-a-spell-after-class-swap)

### **U**
- [4K Upscaling](#4k-upscaling-lossless-scaling)

### **W**
- [Want to Play on Steam Deck?](#want-to-play-on-steam-deck)
- [What Are Some of the Custom Commands on THJ?](#what-are-some-of-the-custom-commands)
- [What Do Different Classes Do Well?](#what-do-different-classes-do-well)
- [What Does CA/CS Mean?](#what-does-ca-cs-mean)

### **Y**
- [Yes, We Support Linux!](#yes-we-support-linux)

---

![pagebreak1.webp](/pagebreak1.webp){.align-center}

---
# FAQs
## 4K Upscaling: Lossless Scaling

<details>
 <summary>Lossless Scaling Guide</summary>

#### Purchase and Install the App:

- Search for **"Lossless Scaling"** in the Steam store and purchase it.

- Install the app from your Steam library.

#### Launch the App:

- Open the **Lossless Scaling** app from your Steam library.

- It will run in the background.

#### Configure the App Settings:

- Customize settings such as:

 - **Scaling mode** (Integer Scaling, FSR, Lanczos).

 - **Hotkeys** for easier control.

- Choose the scaling mode that best suits your needs.

#### Launch Your Game:

- Set the game to a **lower resolution** than your monitor’s native resolution before scaling.

- This allows the app to properly upscale the game.

[Lossless Scaling on Steam](https://store.steampowered.com/app/993090/Lossless\_Scaling/)
</details>

---

## Alternate UIs

<details>
  <summary>Anyone got a UI that works?</summary>

Sure do! Check out [**THJ UI Stuff**](https://discord.com/channels/1204418766318862356/1304678503693942875) or go to **Options > General Tab > Load UI Skin** to see what we have included with the patcher!  

You can also visit [**#screenshots**](https://discord.com/channels/1204418766318862356/1204418768185331763) and check the **pinned messages** for other player-made UIs that might improve your experience.

If a UI works for the **RoF2 client**, it often works here. If it doesn’t, you may need some minor tweaks. **Catapultam** might help, but no guarantees!
</details>

---

## Armor Models

<details>
  <summary>Armor Models</summary>

EverQuest has famously stable (and occasionally complicated) armor graphics. Here’s some info about enabling various textures:

---

### **Velious Armors with Luclin Graphics**  
If you want to use Velious textures with Luclin models, it’s technically possible but unsupported. It can cause crashes or artifacting. **Use at your own risk!**
```
LoadVeliousArmorsWithLuclin=FALSE
```
### Enabling Velious Armor for Classic Models
Add the following to the defaults section of eqclient.ini in your THJ folder.
Make sure LoadVeliousArmor=TRUE is there as well:
```
LoadVeliousArmor=TRUE
LoadArmor17=TRUE  # Cloth
LoadArmor18=TRUE  # Ringmail
LoadArmor19=TRUE  # Scalemail
LoadArmor20=TRUE  # Leather
LoadArmor21=TRUE  # Chain
LoadArmor22=TRUE  # Plate
LoadArmor23=TRUE  # Monk
LoadArmor240=TRUE # Customized Helmets
```
Each line above represents a specific armor type. Toggle them individually if needed.

### Obtaining Helmets with Custom Velious Graphics
Certain helmets (Thurgadin, Kael, Skyshrine) have special Velious graphics. For example:

Thurgadin Helmets
Kael Drakkel Helmets
Skyshrine Helmets
Make sure your glamour stone or ornament is the customized variant when buying or converting these!

### The TIM Layer (Toggle Improved Models)
Use ```#tim``` in-game to switch between classic and newer character models.

### Classic Model Collection, Sponsored by Xackery
Check out the #community-tools discord channel for additional tweaks and updates, on the THJ discord.

</details>

---

## Augments

<details>
  <summary>Augments, What Are They?</summary>

Augments are like **WoW gems**—little pebbles you slot into gear. Some require specific slot types. **Inspect your item** to see the available slots, pick up the augment from your inventory, then drop it in to socket it.

You can buy **basic weapon augments** from the **Aug merchant in the Bazaar**, and **dropped armor augments** from other players.  
You **cannot** slot two of the same gem type into one weapon.

To remove augments, buy a **Perfected Augmentation Distiller** from the aug merchant.  
Note that **Augments do not bind to you**—you can trade them between alts!

---

### **Removing Augments**
- Purchase a **Perfected Augmentation Distiller**.  
- Left-click the augment in your item while the distiller is in your inventory.  
- It will prompt you to remove the augment.

</details>

---

## Basic AA Recommendations for Each Class

<details>
  <summary>Basic AA Recommendations for Each Class</summary>

Below is a sampling of recommended AAs for various classes, compiled by the THJ community:

---

### **Literally Everyone**
- Combat Agility
- Combat Stability
- Natural Durability
- Mastery of the Past (if you have any spellcasting)

---

### **All Melee DPS**
- Combat Fury
- Veteran’s Wrath
- Ferocity
- Ambidexterity (if dual wield)
- Punishing Blade (if 2h)
- Ingenuity
- Weapon Affinity

---

### **All Damage Spellcasters**
- Spell Casting Fury
- Fury of Magic
- Destructive Fury
- Gift of Mana

---

### **All DoT Spellcasters**
- Critical Affliction
- Destructive Cascade
- Gift of Mana

---

### **All Priest-Type Casters**
- Call of the Ancients / Nature’s Boon / Exquisite Benediction
- Radiant Cure

---

### **All Multi-Pet Builds**
- Dire Charm (Ench/Necro with undead) or appropriate version
- Mage - Frenzied Burnout & Host of Elements
- Everyone - Mastery of the Past, Flurry
- Beastlord - Spell Casting Fury, Destructive Fury (Rank 1), Fury of Magic
- Elemental Alacrity / Warder Alacrity for multi-pet synergy

---

### **Proc Builds (War/Bst/Clr, etc.)**
- Bloodlust, Rage of Rallos Zek
- Spell Casting Reinforcement (2?)
- Ingenuity 6
- Combat Fury 6
- Destructive Fury (max)
- Steadfast (avoid stuns)
- Spell Casting Fury / Fury of Magic
- Gelic Claw
- Weapon Affinity
- Divine Avatar (Max)
- Combat Agility / Combat Stability to 18
- Sturdiness 5, various healing CDs, etc.

---

### **All Tank Classes**
- Physical Enhancement

---

### **Class-Specific Recommendations**

#### **Rogue**
- Virulent Venom
- Envenomed Blades
- Anatomy
- Precision
- Triple Backstab
- Strikethrough

#### **Wizard**
- Spell Casting Fury Mastery
- Arcane Destructive Fury
- Improved Familiar
- Cryomancy / Pyromancy

#### **Ranger**
- Flaming Arrows
- Archery Mastery 3
- Trick Shot
- Ranged Finesse
- Precision of the Pathfinder
- Hunter’s Attack Power
- Guardian of the Forest
- Lightning Strikes
- Auspice of the Hunter

#### **Enchanter**
- Doppelganger / Doppelganger’s Beckon
- Eldritch Rune, Veil of Mindshadow
- Mental Contortion
- Dire Charm

#### **Paladin**
- Combat Fury
- Slay Undead
- Healing Gift
- Ferocity
- Knight’s Advantage
- Radiant Cure, Purification
- Speed of the Knight (2h builds)

#### **Monk**
- Way of Steel
- Technique of Master Wu
- Imitate Death
- Hastened Death
- Strikethrough
- Heightened Awareness
- Rapid Strikes
- Purification of Body

#### **Necromancer**
- Cascade of Decay
- Theft of Life
- Death’s Peace
- Army of the Dead, Wake the Dead
- Dire Charm (Undead only)

#### **Shaman**
- Malosinete
- Rabid Bear
- Hastened Rabidity
- Turgur’s Swarm

#### **Berserker**
- Tactical Mastery
- Blur of Axes
- Frenzied Volley
- Blood Pact

#### **Druid**
- Wrath of the Wild
- Spirit of the White Wolf / Black Wolf

#### **Shadow Knight**
- Touch of the Cursed
- Theft of Life
- Soul Abrasion
- Mortal Coil
- Leech Touch

#### **Beastlord**
- Bloodlust (Procs)
- Bestial Alignment
- Bite of the Asp
- Paragon of Spirit
- Warder Alacrity
- Hobble Spirit

#### **Mage**
- Elemental Alacrity
- Elemental Agility / Durability
- Host of Elements
- Servant of Ro
- Frenzied Burnout
- Mend Companion

#### **Cleric**
- Divine Avatar
- Celestial Regen
- Exquisite Benediction
- Hastened Purification
- Bestow Divine Aura

#### **Bard**
- Funeral Dirge (+Hastened Funeral Dirge)
- Song of Stone
- Jam Fest
- Instrument Mastery, Singing Mastery
- Harmonious Attack, Dance of Blades

#### **Warrior**
- Flurry
- Gut Punch
- Stalwart Endurance
- Tactical Mastery
- Rage of Rallos Zek
- Sturdiness (1k HP at max rank)

</details>

---
## Basic Macros
<details>
  <summary>Basic Macros - Loot/Sell Macros</summary>

### Loot Macro
Bind a key to “target nearest corpse,” and also use a macro:
```plaintext
/pause 5, /loot
/notify LootWnd LW_LootAllButton leftmouseup
/notify ConfirmationDialogBox CD_Yes_Button leftmouseup
```
Now pressing that key will both target the nearest corpse and loot it automatically.

---

**Sell Macro**
```plaintext
/notify MerchantWnd MW_Sell_Button leftmouseup
/notify QuantityWnd QTYW_Accept_Button leftmouseup
```
Open the merchant window, click an item, press the macro to sell quickly.

---

**Destroy Macro**
```plaintext
/notify IW_InvPage IW_Destroy leftmouseup
/notify ConfirmationDialogBox CD_YES_Button leftmouseup
```
Open your character page, pick up an item, press the macro. If you have confirmations off, you can omit the second line.

</details>

---
## Bug Report
<details>
  <summary>Bug Report</summary>

NPC steal your items? NPC not there? NPC despawn? Quest broken? Spell Broken? Anything broken?

If you suspect a bug, please visit [**🔴｜in-game-bugs**](https://discord.com/channels/1204418766318862356/1301933112430825575) (Discord) and search to see if it’s already reported. If not, take a screenshot of the issue and open a new thread.

</details>

---
## Buying Spells
<details>
  <summary>Buying Spells</summary>

**Where do I buy spells?**  
You can find trainers for every class in the Bazaar, selling spells up to level 50. Use your **“Bazaar and Back”** AA to get there, then locate your trainer. After 50, you’ll need to search `/baz` for dropped spells, or check **Firiona Vie / The Overthere (Kunark)**. Necro and SK spells 51–60 can also be bought in **Cabilis (Kunark)**. Some classes have alternative Iksar quest lines in Cabilis, too.

For certain older expansions, you can also check **Rushkla Deklamoor** in the EC tunnel.

</details>

---
## Camera Views
<details>
  <summary>Camera Views, Field of View, Viewport</summary>

During gameplay, you can view your character from different camera angles, zoom in/out, or pan up/down. Press **F9** to cycle views.

- First-person (default)  
- Overhead (rotating)  
- Rear (rotating)  
- Overhead (fixed)  
- Rear (fixed)  

Press **F10** to toggle the interface, useful for screenshots.

---

**Field of View**  
Use `/fov number` (45 to 90) to adjust your field of view. For example, `/fov 45`.

**Pan and Zoom**  
`Alt + arrow keys` or right-click drag to move the camera. `F12` toggles mouse panning.

Useful keys:
- Numpad 5/Home: Re-center  
- Numpad 9/3 or PgUp/PgDn: Pitch up/down  
- Numpad 7/1 or Insert/Delete: Zoom in/out  

---

**Viewport Command**  
EverQuest was designed for 4:3. Widescreens can cause vertical cropping. You can run the game in 4:3 or use `/viewport` to adjust.

**Example Viewport Settings:**  
```
/viewport 171 0 1024 768   (768p)
/viewport 240 0 1440 1080  (1080p)
/viewport 320 0 1920 1440  (1440p)
```

</details>

---
## Troubleshooting - Can't find file Specified
<details>
  <summary>Can’t find the file specified error?</summary>

This usually indicates an incomplete download. Possible fixes:

1. Add exceptions for your antivirus—some might be interfering with downloads.  
2. Turn off real-time protection in Windows Security.

Afterward, **redownload** the game.

**Windows Security steps:**  
*Start > Settings > Update & Security > Windows Security > Virus & Threat Protection > Manage Settings*. Toggle real-time protection Off, confirm, then re-download.

</details>

---
## Troubleshooting - Can't unmem a spell after class swap
<details>
  <summary>Cannot Unmem a Spell after Class Change</summary>

If you changed classes and can’t unmemorize a spell (error: “none of your classes are eligible...”), speak to **Ayonae, Composer of Fate** in the Bazaar and say `unmem` to her. That will remove those spells from your gems.

</details>

---
## How to: Create Item Links or Look up Items
<details>
  <summary>Creating Item Links and Looking up Items</summary>

**Can you link the (Legendary) Version of (Item)?**  
From the Bazaar, use your **Bazaar and Back** AA, then type `/buyer` to open the Barter Buyer window. In the bottom-left search box, enter an item name and hit search to see if any version of that item is recognized.

For instance, if you have a base version of “Shield of the Immaculate” but want to see the Legendary version, simply search for it in /buyer. You might see listings or be able to link it even if you don’t own it physically.

**Linking Items in Chat:**  
Shift + Left Click an item in your inventory or on a merchant to create a clickable link in chat. This also works in the #myskills or #mystats windows if they support linking.

</details>

---
## Mythbusting: Decapitate
<details>
  <summary>Do berserkers get decapitate here?</summary>

Nope! We improved **Frenzy** instead.

</details>

---

## What do different classes do well

<details>
 <summary>What does each class do well?</summary>
  
  The classes in your trio are entirely up to you and you're likely to be incredibly strong with any three classes. There are a few core mechanics worth describing in each class, many of which comes from powerful Alternative Advancement abilities. Generally damage comes in 2 flavors, spell based (blue), and skill based (white) and different classes excel at one or both. Furthermore spell damage can either be direct or over time. 

Spell boosting AA from archetype
Healing AAs- [Bst, Clr, Dru, Pal, Shm, Rng] If you have these, your heals will be much more powerful, including in your build definately helps survivability
Direct Damage Critical AAs - [Mag, Nec, Wiz, Clr, Shm, Dru, Bst] including will boost all spell damage vastly, including procs. Wizard stacks with the other classes in the list if you add both.
Damage over Time Critical AAs - [Dru, Enc, Nec, Shm] boost damage over time spells enabling massive damage with them these.

As for the classes themselves, each one is unique bringing many powerful abilities.

Berserker - King of skill based white damage, defensively offers stun immunity, but does not offer the mitigation that Warriors, Knights, or even other hybrids offer.
Bard - Very power mitigation via songs, adds procs, fading memories, DDD is the highest damaging AoE in game at the moment, passively buffs entire group and self via songs. Tracking
Beastlord - Bloodust (guaranteed procs 18s/1min), powerful pet, heals and disease cures
Cleric - Divine Avatar (2min/10min) best white damage boost in game and massive proc rate boost, 30s/5min battle frenzy 100% crit chance and additional damage, powerful heals and status cures.
Druid - DoT focus, Spirit of Black Wolf (7.5min/10min +50% dd/dot crit dmg and 10% dd/dot crit chance), heals, some status cures including RGC. Weak pet
Enchanter - Illusions of Grandeur (2min/10min) 100% more DD/DoT damage, +10% crit chance on both; best blue damage boost in game for the entire party.  Mana restoring abilities, runes, strong debuffs, charming, has a decent baseline pet.
Magician - King of pets, has a 15 slot equipable pet, resist debuffs, strong offensive/defensive CDs
Monk - Skill based white damage, Immate Death (mobs blur every Feign Death), highest skill mit in game
Necromancer - Dot focus, strong pet, Feign Death, life taps and lifetap dots, very survivable, resist debuffs 
Paladin - Heals, Stuns, proc rate boost abilities, stun immunity. Status cures and tank in one stop shop.
Rogue - Skill based white damage with backstab, Shroud of Stealth, proc rate boost on ALL spell based procs, poisons, lethality 40% passively boost all skill damage
Ranger - Archery based white damage, boost skill based damge with spells, tracking. Archery tends to work very well with procs due to how arrows interact with these.
Shadow Knight - lifetaps, stun immunity, Feign Death, incredible passive sustain. very weak pet
Shaman - dots, heals, good defensives, resists debuffs, best slow in game, weak pet
Warrior - Best AC mitigation in game, excellent skills, stun immunity, 6sec/60sec auto proc, Battle Leap is a great damage boost for any white damage build.
Wizard - king of blue damage, crit AA will boost any blue damage build and completely stack with other classes crit AA 

</details>
---
## Do I share AA’s with alts?
<details>
  <summary>Do I share AA’s with alts?</summary>

Nope! But you do earn AA at an increased rate on alts (**Veteran experience**).  
Check out the [*AA Veterancy Mechanism*](https://discord.com/channels/1204418766318862356/1317702999480471552) for more details.

</details>

---
## Do we have a wiki?
<details>
  <summary>Do we have a wiki?</summary>

Yes! The official wiki is a **work in progress**:  
[https://wiki.heroesjourneyemu.com/](https://wiki.heroesjourneyemu.com/)

We also have a **player-made wiki** anyone can edit:  
[https://theheroesjourney.wiki/](https://theheroesjourney.wiki/)

</details>

---
## Echoes of Memory
<details>
  <summary>Echoes of Memory</summary>

**Echoes of Memory (EoM)** are the donation **“gift” currency** you receive for supporting the server via Ko-Fi.

When donating, put your **character name** in the “name/nickname” box. The system automatically sends you **EoM in-game** once the donation processes!

**EoM also drop (rarely) from mobs**—about **1,000 per day server-wide**.  
You don’t loot them; they simply appear in your inventory if you’re the lucky killer.

</details>

---
## Everquest in Windowed Mode
<details>
  <summary>EverQuest in Windowed Mode</summary>

EverQuest can run **full screen or windowed**.  
Press **ALT + ENTER** to toggle between modes.

You can also change this in the **Options window** via a toggle.  
Post-Omens of War, **ALT + TAB** works in full screen.

**Note:** If you use external parsers like **GAMParse** or **GINA**, their overlays won’t appear in full screen mode.

</details>

---
## Server & Gameplay Information

<details>
  <summary>Server & Gameplay Information</summary>

### **Expedition/Dynamic Zones**
An **Expedition** (or **Dynamic Zone**) is a unique instance of a zone for your group/raid. You can add/remove players freely.

#### **Expedition Interface (Alt + Z)**
Displays:
- Assigned Expedition (which zone you’re in)
- Leader name
- Members list
- Player count / max players
- Quit Expedition (1-minute timer to port you out)
- Outstanding Expedition Timers
- Leader Options

#### **Leader Options**
Affect the “Player Targeted” field:
- Add Player
- Remove Player
- Make Leader

#### **Expedition Commands**
Use `/dz` as shorthand for “dynamic zone”:
- `/dzHelp`, `/dzListTimers`, `/dzPlayerList`
- `/dzAddPlayer`, `/dzRemovePlayer`, `/dzMakeLeader`
</details>

---

## **Forum Activation Email**
<details>
  <summary> Forum Activation Email </summary>
If your forum activation email never arrived, request another here:  
[**EQEmu Forum Activation Request**](https://www.eqemulator.org/forums/register.php?do=requestemail)
</details>

---
## **Getting Around**
<details>
  <summary> Getting Around </summary>
To move around quickly, head to the **middle building** in the **Bazaar** and look for **Tearel** (the elf in purple).  
Target Tearel, press **H** to hail, and follow the menu options.

You can **attune the map** to different locations. Some teleports may cost **EoM** to unlock for your account.  
Then click the **giant floating map** by his head and pick **“Self”** or **“Group”** teleport.
</details>

---

## **Glamours for Weapons and Armor**
<details>
  <summary>Glamours for Weapons and Armor </summary>
Visit the **Purveyor of Glamour** in the Bazaar (near the stables) for cosmetic items.


### **Random Weapon Glamours**

 Random Weapon Glamours
Give **2 EoM** for a **random weapon glamour** (could be anything from Rusty Sword to an Epic 2.0 look).

### **Convert an Existing Item**
Give the **weapon or armor + 5,000 pp** to the Purveyor to receive a **glamour version** of the same appearance.

### **Additional Cosmetic Items**
For **illusions and mounts**, visit the **Gambling Halfling** near the **East Bank** in the Bazaar.  
**5,000 platinum** or **2 EoM** per gamble attempt.
</details>

---

## **Group Experience on THJ**
<details>
  <summary>Group Experience on THJ</summary>
XP is **split evenly** among group members, but individual XP modifiers still apply.

#### **Order of operations:**
1. Base XP is gained.
2. It’s split evenly among group members.
3. Individual modifiers (**AA count, level, potions**) apply last.

</details>

---

## Having lag/stuttering issues in game?
<details>
  <summary>Having lag/stuttering issues in game?</summary>
If your system can handle bigger games but EQ stutters, try the following:

1.  **Edit eqclient.ini**: `CPUAffinity0 = -1` (use all CPU cores) `UseLitBatches = FALSE` (use your GPU a bit more)
2.  **NotCPUCores**: [Download here](https://github.com/rcmaehl/NotCPUCores/releases). Let you manually set affinity for eqgame.exe and ensure all cores are utilized.
3.  **4GB Patch**: [https://ntcore.com/4gb-patch/](https://ntcore.com/4gb-patch/) Patch eqgame.exe for large address awareness. - There is a video on how to install [here](https://discord.com/channels/1204418766318862356/1314594496427851856/1317721681942544386)
</details>

---

## Heroic Stats

<details>
  <summary>Heroic Stats</summary>

These are stats on Legendary items with a “+#” next to them. They can offer unique effects. For more info, see:

[Heroic Stats Wiki](https://wiki.heroesjourneyemu.com/en/classes-and-abilities/heroic-stats)
</details>

---
---
## How to copy UI files

<details>
  <summary>How to copy UI files</summary>

So You've made your first alt, now you wish it had the spiffy UI files that your first character had. This is easy to accomplish by press start R to pull up the run command in windows and adding
>   cmd /c copy "c:\THJ\UI_Originalname_thj.ini" "c:\THJ\UI_Newname_thj.ini"```
If you want to copy the actual spell configs over, etc, you can 
>   cmd /c copy "c:\THJ\Originalname_thj.ini" "c:\THJ\Newname_thj.ini"```
  You simply need to replace Originalname with the original character's name. and Newname with the new characters name and the command should work. Also, if You've put THJ folder in a different location, you need to type that alternative filepath.
</details>
---
## I want to make a trader!

<details>
  <summary>I want to make a trader!</summary>
Head to [EQEmu forum](http://www.eqemulator.org/account/?CreateLS) and create a second login account. Run the client again with this account to make a trader. If you leave the Bazaar, the trader disconnects. If you need multiple accounts for multiple people at your home, request an IP exemption from the Guides.

Use `/trader` in-game to begin. You’ll need **trader satchels**, must be standing in the trader stalls, and you set item prices in the pop-up window.
</details>

---

## Incomplete Maps?

<details>
  <summary>Incomplete Maps?</summary>

If you enter zones like Halls of Betrayal or Dulak and find them blank, you can grab third-party maps. For example:

[eq-map-files](https://www.eqmaps.info/eq-map-files/)

**How to Install:**

1.  Download the ZIP file of the maps.
2.  Unzip the contents.
3.  Find your EverQuest folder, typically `C:\THJ if you followed the Getting Started`
4.  Create `C:\THJ\maps\Brewall`
5.  Copy the unzipped map files into that folder.
6.  Log into EQ, open your map window, and choose “Brewall” in the upper-left dropdown.
</details>

---

## IP Exemptions

<details>
  <summary>IP Exemptions</summary>

For an IP Exemption (to allow more than the normal limit of simultaneous logins from the same IP), see [**#ip-exemption**](https://discord.com/channels/1204418766318862356/1341481810001133569) in Discord. The process is partially automated.
</details>

---

## Leveling Paths

<details>
  <summary>Leveling Paths</summary>

Below is a general leveling guide. Adjust as needed to suit your class and gear:

### Leveling Guide

#### 1–8

-   Crushbone
-   Field of Bone

#### 8–25

-   Unrest
-   Kurn’s Tower
-   Befallen
-   Upper Guk
-   Cazic Thule
-   Najena
-   Infected Paw
-   Permafrost

#### 25–40

**Recommended:** Level lock at 30, grind AAs (0–150+)

-   **Lower Guk**  
    Great for Slay Undead; high mob density/low HP mobs.
-   **Gulf of Gunthak (req Kunark)**  
    Great for Assassinate/Headshot.
-   **Dulak’s Harbor (req Kunark)**  
    Great for Assassinate/Headshot.
-   **City of Mist (req Kunark)**
-   **Mistmoore**  
    Great for Slay Undead.
-   **Solusek A**  
    Great for Assassinate/Headshot.
-   **Tower of Frozen Shadow (req Velious)**  
    Great for Slay Undead.
-   **Thurgadin / Kael Drakkel / Skyshrine (req Velious)**  
    Great for faction farming while leveling for class armor sets.

#### 40–50

**Recommended:** Level lock at 40, grind AAs (150–300+)

-   **Howling Stones (req Kunark)**  
    Great for Slay Undead.
-   **Veksar (req Kunark)**  
    Great for Slay Undead.
-   **The Hole (Ruins of Old Paineel)**  
    Undead tower area in the back is great for Slay Undead.
-   **Nagafen’s Lair**  
    Great for Assassinate/Headshot.
-   **Chardok (req Kunark)**  
    Great for Assassinate/Headshot.
-   **Velketor’s Labyrinth (req Velious)**  
    Maze-like, but multiple small packs of low HP mobs for AOE farming.

#### 50–60

**Recommended:** Level lock at 50, grind AAs (300–500+)

-   **Crypt of Nadox (req Kunark)**  
    Ideal at 49–51; amazing mob density for AOE.
-   **Torgiran Mines (req Kunark)**  
    Great for Assassinate/Headshot.
-   **Hate’s Fury (req Kunark)**  
    Great for Assassinate/Headshot.
-   **Veksar (req Kunark)**  
    Great for Slay Undead.
-   **Dragon Necropolis (req Velious)**  
    High ZEM (~2.8x), lower HP mobs around level 60+.
-   **Halls of Betrayal (Chardokb) (req Kunark)**  
    High ZEM; great for Slay Undead and Assassinate/Headshot.
-   **Plane of Hate**  
    Great for Slay Undead and Assassinate/Headshot.

  
 

Lock levels if you want to farm AAs around 30, 40, and 50 to build up a strong foundation.   
  
**Once you get to level 60 with 500-750 AAs,**  
you should be in a good place to stop focusing on grinding AAs and start farming best-in-slot gear upgrades.   
</details>

---

## Macro Items - the /useitem command

<details>
  <summary>Macro Items (/useitem command)</summary>

**/useitem 'slot' \[subindex\]**  
Use this command to click items in specific slots (inventory or worn).

**Example: /useitem 16**  
This clicks your right ring. Add `/pause 6, /useitem 16` in a macro to give it half a second to cast before the next line executes.

To click an item in a bag slot (bag #, position #), you do something like `/useitem 23 0` if it’s in bag slot 23, position 0. Bag slots count upward left-to-right, top-to-bottom.

Item Slot Codes: • Charm = 0 • Left Ear = 1 • Head = 2 • Face = 3 • Right Ear = 4 • Neck = 5 • Shoulders = 6 • Arms = 7 • Back = 8 • Left Wrist = 9 • Right Wrist = 10 • Range = 11 • Hands = 12 • Primary = 13 • Secondary = 14 • Left Ring = 15 • Right Ring = 16 • Chest = 17 • Legs = 18 • Feet = 19 • Waist = 20 • Power Source = 21 • Ammo = 22 • Bag 1 = 23 • Bag 2 = 24 • ... • Bag 10 = 32
</details>

---

## Play on Mac

<details>
  <summary>Play on Mac</summary>
Some have had success running THJ with a *Windows VM* or *Wine*.

1.  Install directx9 (e.g., [directx9 redist](https://www.microsoft.com/en-us/download/details.aspx?id=8109)).
2.  Run the THJ .exe in “administrator” mode inside the VM if possible.

*Wine64 on modern macOS sometimes doesn’t support 32-bit clients, so you may need a special environment or a VM approach.*
</details>

---

## Playing a Triple Pet/Minion Master

<details>
  <summary>Playing a Triple Pet/Minion Master</summary>

*(Necromancer, Beastlord, Mage Playstyle Guide)*  
@Duhr (nec/mag/bst) wrote this whole guide on the basics of the gameplay for the 3x pet classes playstyle guide. This is meant to be a general guide to get you comfortable with petcuck playstyle.

We also have a 3-pet pet window for you to add to your favorite UI down at the bottom.

---

## Trash Pulls

**Engage:**

-   Send in pets and ensure each mob is hit by your pets at least one.
-   Use your highest-level Beastlord heal to keep pets alive.

**Pet Maintenance:**

-   Utilize the Staff of Symbols paired with sympathetic heals to grant a one-hit immune shield and heal all pets.
-   Use Host of the Elements (short cooldown) for higher damage when pulling more mobs or speeding up tougher kills.

**Aggro Control:**

-   Use Host in the Shell to draw aggro to pets before healing them. Host in the Shell is a long-term absorb that will help mitigate incoming damage to your pets.
-   Pair Summon Companion with Death’s Peace to transfer all aggro to pets.
-   Ensure pets hit all mobs before standing up.

**Sustain:**

-   Heal yourself with taps.
-   Maintain Death’s Peace to clear aggro on yourself while you are healing your pets as needed.

---

## Boss Fights

**Preparation:**

-   If splitting the boss is required, use Death’s Peace and Pet Hold commands to position effectively.
-   Once in place, send in pets and let them work.

**Cooldown Usage, use all including;**

-   Servant of Ro (long cooldown, high DPS).
-   Frenzied Burnout, Swarm of Decay, Army of the Dead.
-   Wake the Dead (if corpses are nearby).
-   Rotate short-duration cooldowns as you would for trash pulls.

**Healing & Buffs:**

-   Use Mage Pet HoT (Primal Remedy) to protect pets from dispels and provide minor healing.
-   Use the Staff of Symbols for shield protection and minor heals.
-   Beastlord pet heals remain your primary healing source.

**Additional DPS:**

-   When pet DPS slows, apply dots for extra damage.

---

## Leveling Tips

**Pet Upkeep:**

-   Keep pets max level and ensure taunt is active to manage aggro.
-   Use Beastlord pet heals for major recovery.

**Buff Rotation:**

-   Apply pet buffs in this order: Beastlord → Mage → Necromancer to maximize stacking.
-   Add the Beastlord proc buff for the best pet mitigation.

**Weapons:**

-   Equip your pets with summoned proc weapons:
-   Use the sychronobags to equip them with weapons, a muzzle, and something else juicy!
-   Use Dimensional Armory after level 50 for your Mage pet.
-   Switch to Rune of Swords when available.

**AA Grinding:**

-   Pause at level 30 to farm AA in zones like Lower Guk.
-   Stop again at 48, where pets can effectively handle Plane of Hate mobs.
-   Push for your epic weapon, then the game opens up.
-   Note: AA gains slow significantly at level 60.
</details>

---

## Quest Guides

<details>
  <summary>Quest Guides</summary>

**Where can I find info about \[quest\]?**  
Recommended resources:

-   [EQProgression.com](https://www.eqprogression.com/)
-   [P99 Quest Wiki](https://wiki.project1999.com/Category:Quests)

Check  [thjdi.cc](https://thjdi.cc/) to verify spawns and item drops.
</details>

---

## So you want to donate?

<details>
  <summary>So you want to donate?</summary>

**That’s awesome!**

Consider making it monthly if you want to support ongoing development. Use [https://ko-fi.com/theheroesjourney](https://ko-fi.com/theheroesjourney) to donate.

**Interested in EoM?**  
Donate as a guest and enter your character name (first name only) in the “name” field. We’ll automatically send you the EoM gift in-game!

**Bitcoin?** Sure! `bc1q6khn0nuwh3gxn6ku63etva56vnn3r5xww9am47`
</details>

---

## Support Forum

<details>
  <summary>Support Forum</summary>

Can’t log in? Technical issues? Download trouble? Go to [**🟡｜tech-support-forum**](https://discord.com/channels/1204418766318862356/1299429412902670397), search for existing threads, or open a new one with screenshots.
</details>

---

## Sympathetic Strike/Healing

<details>
  <summary>Sympathetic Strike/Healing</summary>

There's ranks of the effect. All are clicky buffs. 

The sympathetic heal ranks have varying minimum requirements for mana and spell level to trigger. Eg. Sympathetic heal 1 triggers from any beneficial (buff or heal) spell with a mana cost of 10 or above, but Symp Heal 4 requires level 30+ spell *and* 75+ or 100+ mana. 

Sympathetic Healing lists a minimum spell level for a required proc. Please remember *other classes* may get the spell at an earlier level than you and so for your class.. that spell might not proc. 

The effect of this is an extra heal that scales based on the rank of the buff and your +healing stat (healing AAs also boost this). The extra heal will land on your current target when your triggering spell finishes casting. 

Symp strike requires minimum of 10 mana to trigger on a detrimental damaging spell (dot or DD) for all ranks. 

This is an extra nuke that lands when your triggering spell finishes casting. Damage increases with rank of the buff. 

Here is a thread where its discussed, and a [list of all the items](https://docs.google.com/spreadsheets/d/1viwIXFigtKHnQIg8Cw5bSGN8cUQkbG3jGR1LRtE-WPQ/edit?usp=sharing): 
</details>

---

## The First Quest, what do I do?

<details>
  <summary>The First Quest, what do I do?</summary>

Press **Alt+Q** for your quest journal to see “The Heroes’ Journey... The Journey of a Thousand Miles...”

Well, alt+q should bring up your quest journal, and you'll see your introduction to **The Heroes' Journey**... The Journey of a Thousand Miles...

This quest will tell you to:

-   Use **Bazaar and Back** to travel to The Bazaar. Bazaar and Back is an Alternate Advancement Ability, it is located in your Alternate Advancement Window.
-   Hit I to open your inventory, and then click alt. advancement in the bottom left. When it pops up, the general tab on the top left should let you scroll to see Bazaar and Back.. make a hotkey for it, and then use that ability!
-   Deliver 1 Faded Writ to a Fading Memory in your bag should be a Faded Writ. When you click on it the item will be on your cursor, you can hand items on your cursor to NPCs, and that is what you will have to do, hand it to a Fading Memory.
-   **Where is the Fading Memory?** Well, the fading memory is in the Bazaar! He is standing by the souther-western bank, by the wall. **He is nearly invisible**! So don't miss him. He'll get you setup and on your way!  
     
</details>

---

## More Teleport Options?

<details>
  <summary>More Teleport Options?</summary>

You’ll have to explore and discover them yourself! Except for the starter/trivial areas:

[Teleport Wiki Page](https://wiki.heroesjourneyemu.com/en/exploration-and-combat/teleport)

Our official Wiki and the player-made Wiki both list teleport locations:  
[https://theheroesjourney.wiki/index.php?title=Teleport\_locations](https://theheroesjourney.wiki/index.php?title=Teleport_locations)
</details>

---

## THJ Install Commands Explanation

<details>
  <summary>THJ Install Commands Explanation</summary>

## Steam Console Commands & Steam Depots

Several people have asked about the console commands and such we have to type in when getting the steam-depots, so here is a breakdown:

### The command *steam://open/console*

A Steam protocol link that, when run in the Windows “Run” window (Win + R), opens Steam’s built-in console. This console allows you to input various commands for debugging, downloading specific depot files, accessing hidden Steam settings, and other advanced Steam-related tasks.

### How to Use It:

1.  Press Win + R to open the “Run” dialog.
2.  Enter `steam://open/console` and press Enter.
3.  Steam will open, and you'll see a new Console tab in the client.

### What You Can Do With the Steam Console:

-   Check hidden app info using commands like `app_info_print 'AppID'`.
-   Download specific game versions (useful for rolling back updates).
-   Access hidden Steam settings.
-   Monitor Steam logs and errors.

---

### The command: `download_depot 205710 205711 1926608638440811669`

Used in Steam’s console to manually download a specific version of a game’s files. Let’s break it down:

### Understanding the Command

-   **download\_depot** → This is the Steam console command to download a specific game’s depot.
-   **205710** → This is the AppID of the game (in this case, Torchlight II).
-   **205711** → This is the DepotID, referring to a specific set of game files (e.g., base files, DLC, or a particular platform version).
-   **1926608638440811669** → This is the Manifest ID, corresponding to a specific version (patch/update) in that depot.

### What Happens When You Run It?

Steam will download the specific depot (game files) with that manifest version. The files will be stored in:

```plaintext
Steam\steamapps\content\app_'AppID'\depot_'DepotID'
```

Example path:

```plaintext
C:\Program Files (x86)\Steam\steamapps\content\app_205710\depot_205711
```

This does not replace your currently installed game files; you must manually copy/move them if you want to use them.

### Why Would You Use This?

-   Downgrade a game to an older version if a new update causes issues.
-   Retrieve missing or deleted files without reinstalling the entire game.
-   Extract specific game assets (for modding or debugging).
  </details>

---

## Titles

<details>
  <summary>Titles</summary>

**Mob Slayer Titles** (kill X of a mob type):

-   Hunter: 500
-   Slayer: 5,000
-   Destroyer: 10,000
-   Exterminator: 50,000
-   Annihilator: 1,000,000

**Gambler Titles**: Awarded for gambling certain amounts or hitting rare jackpots. 

**God-Slayer**: Chance to get this by landing the killing blow on a god. 

**Event Titles**: Earned through holiday events or Twitch events. Watch [**#announcements**](https://discord.com/channels/1204418766318862356/1288875607509172234). 

**Easter Egg Titles**: Hidden in various ways, you have to find them!
</details>

---

## Tracking: Situational Awareness and Tune of Pursuance

<details>
  <summary>Tracking: Situational Awareness and Tune of Pursuance</summary>
Both *Tune of Pursuance* and *Situational Awareness* add an **invisible bonus** to your Tracking skill—like +50 or +75 skill points. This doesn’t show in your character window or #myskills, but it is working.

For example, if your base Tracking is 175/175, and you get +75 from these AAs, the UI will still show 175/175, but you effectively have 250.
</details>

---

## Tribute

<details>
  <summary>Tribute</summary>

**Tribute - Temporary Personal Buffs and Focus Effects**

## What is Tribute?

The Tribute system is active on THJ and available from Classic Era and onwards. This was added in the Gates of Discord expansion to allow players to sacrifice items or platinum in exchange for Favor. Players may then spend Favor to acquire various buffs, including focus effects, extra stats or AC, resists, and even the option to automatically resurrect upon dying.

Note that when you turn an item or platinum in for Favor that thing is lost forever as if you had destroyed it.

## How do I use Tribute?

You will need to visit a Tribute Master to select what buffs you want and donate items for Tribute Points. The easiest tribute master to find is Aeyln D\`sai, located in The Bazaar at the Shadowhaven side bank.

First, let's obtain some Favor. Select items that you do not want from your inventory and press Donate. This will consume the item and increment your Current Favor and Career Favor.

-   **Your Current Favor** is how much you have to spend on buffs. The active cost of your buffs will be subtracted from this value every 10 minutes while Tribute is active.
-   **Your Career Favor** is a cumulative representation of the total favor you have earned. This is not spendable, instead just a big number to show off.

Next, we will select some buffs that we want. Buffs come in tiers which have increasing costs and level requirements. As you upgrade a buff to a higher rank, it provides a stronger benefit. We'll select a buff from the Available Benefits tab and then press Upgrade to move it to our Active Benefits tab.

The last thing is for us to actually activate the Tribute and receive. The default keybind to pull up our Tribute window is Alt+U.

Press Activate and your buffs will turn on, subtract the current cost from your current favor, and then the 10-minute timer will count down. When the timer reaches 0, you will pay the active cost again and your buffs will keep running.

To deactivate our Tribute, we use the same Alt+U window and press Deactivate. This stops the clock, stops consuming our favor, and immediately takes away our buffs.

## How do I get items to donate for Tribute?

A good rule for items is that if they're wearable, rare, and worth a lot of vendor platinum then they might Tribute for a lot. This rule can start to break down in later expansions when the platinum value of items decreases, but it gives you an idea of how to approach Tribute.

**Excellent zones for farming Tribute are:**

-   Veksar
-   Crypt of Nadox

Because these are later zones, the items from these places do not have much vendor value, but some pieces can have extraordinary Tribute value for the difficulty in acquiring them.

**Decent zones for farming Tribute are:**

-   Sebilis (Kunark class armor, notably breastplates from Trakanon)
-   The Hole (Loam visible pieces, the robe especially)
-   Karnor's Castle (Kunark class armor, notably leggings from Venril Sathir)

## Tips for getting the most out of your Tribute

-   Carefully weigh the value of an item before you donate it. You can use Ctrl+Shift+Left Click to instantly search the Bazaar to see what an item might be worth to other players. It might Tribute for a lot, but it could also sell for a lot, too!
-   If you find a good item to Tribute, consider checking the Bazaar to see if anyone is selling it for cheap. It might be easier to buy several items instead of going to farm them.|
-   There may be certain instances where you can get away with using lower tier focus effects instead of the maximum. Improved Damage IV works on spells up to level 65. Improved Damage III works on spells up to 60.
-   Try not to forget to turn your Tribute off if you don't need it anymore, or avoid going AFK overnight if you leave it on a lot. It will keep ticking and consuming your favor.
</details>

---

## What are some of the custom commands?

<details>
  <summary>What are some of the custom commands?</summary>

-   **#zoneshard** – Teleport between Bazaar shards.
-   **#mystats** – Shows extended stats. If you have a pet targeted, shows the pet’s stats.
-   **#myskills** – Extended skill info beyond the normal UI.
-   **#tim** – Toggle improved models (classic/new).
-   **#help** – Lists more custom commands!
  </details>

---

## What does CA/CS mean?

<details>
  <summary>What does CA/CS mean?</summary>
They refer to the AAs **Combat Agility** (CA) and **Combat Stability** (CS). CA increases the chance mobs will miss you; CS reduces incoming damage. Each has 18 ranks. They’re essential for any melee or tank build.

You can stop at 9/18 and 9/18 and finish them later, or even just go ahead and slam through-- which I always do.
</details>

---

## Tentative Launch Schedule

<details>
  <summary>Tentative Launch Schedule</summary>

-   **Oct 30/31** – THJ Beta ends; final wipe and pre-launch patch.
-   **Nov 1, 2024 (7:00 PM)** – Official Launch, Classic only.
-   **Nov 29** – Kunark + LoY unlocked. Must complete progression to access Kunark content.
-   **Dec 27** – Velious unlocked.
-   **Feb 7** – Luclin unlocked.
-   **Mar 21** – Planes of Power unlocked (8-week lock).

God, OoW, DoN will follow, schedule may shift based on player feedback. Seasonal plays (SSF, HC, Fabled) may appear between expansions.

*Dates subject to change based on dev schedules.*
</details>

---

## Want to play on Steam Deck?

<details>
  <summary>Steam Deck Install</summary>

One of our community members got THJ working on Steam Deck and wrote a full guide in [**The Heroes (Mobile) Journey - Steam Deck**](https://discord.com/channels/1204418766318862356/1313567827566788670) channel. Check it out and show them some love!
</details>

---

## Boss Not Spawning in DZ

<details>
  <summary>Boss Not Spawning in DZ</summary>

Mobs with a spawn timer of 2+ hours usually only appear in a **non-respawning** version of the zone. This includes **Plane of Sky** and many bosses.

Check out [THJDI](https://thjdi.cc/) for more details on spawn rules.
</details>

---

## Yes, we support linux!

<details>
  <summary>Yes, we support Linux!</summary>

Check out our [linux](/getting-started/linux) install page.

</details>

![pagebreak4.webp](/pagebreak4.webp){.align-center}