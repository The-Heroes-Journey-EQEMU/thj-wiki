---
title: THJ Tips
description: Are you new to THJ? Here are some tips
published: true
date: 2025-05-02T14:45:48.468Z
tags: 
editor: markdown
dateCreated: 2025-02-27T18:13:46.567Z
---

![gettingstartedbanner.webp](/gettingstartedbanner.webp){.align-center}
# THJ Tips & Tricks

Welcome to a quick rundown of must-know tips for The Heroes’ Journey server (THJ). This guide covers **sympathetic items**, **skill leveling**, **bag farming**, **Bazaar NPCs**, and a short **FAQ** on faction and item leveling.

Check out [this video](https://youtu.be/mtYqxXW5C-c?si=CcJZSmbxj5OXMFoq) by a youtuber named: Ion Blaze Gaming for some really, really good information!

---

> Some reminders, tips, and tricks to help in **your** Heroes' Journey experience.

## 1) Sympathetic Items – Big Boosts to Damage & Healing

Sympathetic effects provide significant bonuses to both **damage** and **healing**. Here are some highlights:

-   **Tutorial Ring:** Gains *Minor Sympathetic Strike* once it becomes **Legendary**.
-   **Pal/Clr Summoned Hammers:** Come with *Sympathetic Healing I*.

### Farmable Sympathetic Items (1–50)

-   **Sacrificial Dagger (Strike II):**  
    \- Dropped in Mistmoore from a demon near the GY/crypt area (PH involved).  
    \- *Alternative:* Mithril Quill in SolA’s gnome castle area.
-   **Fine Steel Warhammer (Heal II):**  
    \- Ideal if dropped as Legendary, but any version is still worth watching for.
-   **Black Tome with Silver Runes (Strike III):**  
    \- Dropped by Frog Tactician in LGuk (live side, King room).  
    \- Likely the easiest Strike III item in Classic.
-   **Prayer Shawl (Healing III):**  
    \- Supposedly drops from Estrella in Kedge. (*Unconfirmed*).

**Pro Tip:** Use *RetributionEQ Alla* to search for items and effects. On the Ret server, “Apocryphal” = “Legendary.” Items must be **Apoc/Legendary** to gain special effects like Sympathetic Strike.

For this server, you can use a fan-made site: [THJ DI](https://www.thjdi.cc).   
Example item link: [https://www.thjdi.cc/item/2013400](https://www.thjdi.cc/item/2013400)  
 

---

## 2) Skill Leveling + Sympathetic Items Synergy

To maximize synergy between skill leveling and sympathetic items:

1.  **Spam low-level spells (Lvl 1-ish)** as you go:
    -   Adds extra damage.
    -   Keeps your spell skills and channeling high.
2.  **Equip sympathetic items** to benefit from extra damage/healing procs *and* keep skills up.

---

## 3) Bags – A Must-Have for Capacity & Weight Reduction

Bags **cannot** be upgraded in the power slot, but **Enchanted/Legendary** bags often have:

-   Increased capacity
-   Weight reduction (WR)

### LGuk Farming Options

-   **Supplier Bags:** not lore; farm multiple.
-   **Evil Eye Bags:** also not lore; grab as many as you can.

**Pro Tip:** If you’re leveling in LGuk (any side), kill these mobs regularly to pick up extra bags.

### Bazaar Vendor Option

There’s a bag vendor in the Bazaar selling **super cheap 20-slot large bank boxes**. Stock up for more storage!

---

## 4) Bazaar NPCs of Note

### Spell Vendors/Trainers

-   Located on the **north side** of the Bazaar.
-   Offer spells up to **Level 50** (with a few exceptions).
-   **Tip:** Buy spells in bulk for multiple level ranges (10–25, 25–40, etc.).

### Tearel (Teleport NPC)

-   Hail Tearel, choose a destination, then *click the map* to teleport.
-   **Pro Tip:** Look for **glowing stones** while exploring to unlock more teleport options.

### Vision of Ayonae (Class Reset NPC)

-   Found on the **east side** of the Bazaar.
-   Allows you to remove one class to add another.
-   **Cooldown:** 15–30 days (TBD after launch).
-   **Cost:** Requires *Essence of Might (EoM)*.

### SW Bank NPCs

-   **Parcels NPC:** for mail/parcel service.
-   **Fading Memory Quest NPC:** for a specific quest line.

## 5) Helpful Commands
### Outputfile
The /outputfile command generates a file containing specific game-related information.

Usage: `/outputfile <content>.<file_ext>`

Available Content Types:

- Guild – Guild information
- Raid – Raid details
- Spellbook – Your learned spells
- Inventory – Items in your inventory
- Guildbank – Guild bank contents
- Realestate – Owned real estate
- Guildhall – Guild hall details
- Missingspells – Spells you haven't learned

**Example:**
- `/outputfile missingspells Greg.txt`

This creates a file named Greg.txt in the root of your THJ installation folder.

### Rewind
Moves your character back to the last safe location if stuck.

Usage: `/rewind`

Can only be used periodically (cooldown applies).
Won't work in combat or if recently moved.

### Corpsefix
Attempts to reposition nearby corpses if inaccessible.

Usage: `#corpsefix`

Useful if your corpse is stuck in geometry or unreachable.
If unsuccessful, seek assistance from a Guide/GM on Discord.

### Hidecorpse
Controls corpse visibility around you.

Usage: `/hidecorpse <option>`

Available Options:

all – Hides all existing corpses.
looted – Hides only looted corpses.
none – Shows all corpses.
always – Hides all corpses permanently until toggled off.

**Example:**
 - `/hidecorpse looted`

### Mystats
Displays detailed statistics about your character.

Usage: `#mystats`

Shows attributes like HP, mana, AC, resistances, and attack power and pet details.
Useful for monitoring buffs, debuffs, and gear effects.
Pet information will appear as a text dump in your chat window.  

### Myskills

Displays all of your character’s skill levels.

Usage: `#myskills`

Shows current value for each skill (e.g., 1H Blunt, Evocation, Defense).
Useful for tracking skill progress and identifying untrained skills.
Especially helpful after level-ups or gear changes.

### Zoneshard
Reveals the shard (server instance) your current zone is running on.

Usage: `#zoneshard`

Useful for reporting zone-specific issues or lag.
Helps admins identify backend server performance.
Displays shard ID for technical support or troubleshooting.

### Mapfilter
Controls what appears on your in-game map.

Usage: `/mapfilter <option> [on|off|default]`

Description:
The /mapfilter command allows you to filter or customize icons, labels, and markers shown on your map, helping you reduce clutter and focus on relevant NPCs, items, or objects.

#### Common Options:
| Option     | Description                                        |
|------------|----------------------------------------------------|
| all        | Toggles all filters on or off.                     |
| npc        | Show/hide non-player characters (mobs).            |
| pc         | Show/hide other players.                           |
| corpse     | Show/hide player and NPC corpses.                  |
| ground     | Show/hide ground items.                            |
| name       | Show/hide names for filtered entities.             |
| target     | Highlights your current target.                    |
| cast       | Highlights NPCs casting spells.                    |
| trader     | Show/hide trader characters.                       |
| pet        | Show/hide pets.                                    |
| timer      | Show/hide campfire and other timed markers.        |


`/mapfilter ground on`
Shows all ground items on the map.

`/mapfilter all default`
Resets all map filters to default settings.

**Bonus Tip:** Check out the center of the Bazaar for more merchants and items!
---

![pagebreak1.webp](/pagebreak1.webp){.align-center}

## Frequently Asked Questions

### How does Starting Faction work?

-   Based on **class, race, and deity**.
-   Affects guard KOS status and epic quest progression.
-   **Recommendation:** Choose Agnostic if possible.
-   If you plan a specific trio of characters, pick your race first; go Agnostic if available.

### How does Item Leveling work?

1.  Only items in the **Power Slot** receive XP.
2.  **Bags and Augs** do not level.
3.  If you can’t equip it, you can’t level it.
4.  Once an item gains XP, it becomes **NO TRADE**.
5.  Item leveling does not reduce your personal XP gain.
6.  **Leveling speed:**
    -   More stats = slower leveling.
    -   Sympathetic items take even longer.
    -   Approx. 4x Regular = 1x Enchanted, 4x Enchanted = 1x Legendary.
7.  Use the *“Consume Item”* AA to handle extra items — it’s essential!

### Lore/No Drop on Items?

-   Many items normally flagged **No Drop** or **Lore** are **tradeable** here.
-   Includes many **epic quest** drops — good for pre-Kunark farming.
-   **Pro Tip:** Sell or give away Phinny drops you don’t need!
-   Equipping normal/enchanted gear **doesn’t attune** it unless:
    -   You *use a clicky* on it, or
    -   You *kill a monster* with it in the **Power Slot**.

### Options for Faction Issues/Turn-ins?

-   **Sneak** (without Hide) behind an NPC to become indifferent.
-   **Feign Death (FD)** can help with turn-ins similarly.
-   **Legendary Masks** (e.g., *Mask of Deception* from LGuk assassin) become All/All, useful for:
    -   Fixing faction problems.
    -   Bypassing locked doors.

---

<h1>AA Veterancy Mechanism</h1>
<h2>Introduction</h2>
<p>The AA Veterancy Mechanism rewards players with an <strong>AA bonus cap</strong> based on their existing characters' spent AAs. This system allows you to level up new characters' AAs more quickly while encouraging you to maintain multiple active characters.</p>
<hr>
<h2>Table of Contents</h2>
<ol>
  <li><a href="https://chatgpt.com/c/67bf95fc-b1a0-8009-a9ba-37cc9d6b7b6e#overview">Overview</a></li>
  <li><a href="https://chatgpt.com/c/67bf95fc-b1a0-8009-a9ba-37cc9d6b7b6e#detailed-calculation">Detailed Calculation</a></li>
  <li><a href="https://chatgpt.com/c/67bf95fc-b1a0-8009-a9ba-37cc9d6b7b6e#example">Example</a></li>
  <li><a href="https://chatgpt.com/c/67bf95fc-b1a0-8009-a9ba-37cc9d6b7b6e#bonus-mechanic">Bonus Mechanic Explained</a></li>
  <li><a href="https://chatgpt.com/c/67bf95fc-b1a0-8009-a9ba-37cc9d6b7b6e#tips-tricks-and-strategies">Tips, Tricks, and Strategies</a></li>
</ol>
<hr>
<h2>Overview</h2>
<p>The AA Veterancy system calculates a special <strong>AA bonus cap</strong> for your characters based on how many <strong>additional</strong> characters you have leveled. Only characters other than the one currently logged in are counted toward this total.</p>
<ul>
  <li><strong>Subtract 150</strong> from each character's spent AAs.</li>
  <li>If the result is <strong>negative</strong>, treat it as <strong>0</strong>.</li>
  <li><strong>Add all the positive results</strong> together to get the <strong>total bonus</strong>.</li>
  <li>This total becomes your new <strong>AA bonus cap</strong> if it exceeds 150.</li>
</ul>
<hr>
<h2>Detailed Calculation</h2>
<p>Below is a step-by-step outline of how to calculate your AA Veterancy total:</p>
<ol>
  <li><strong>Check each alt character’s spent AAs.</strong></li>
  <li>Apply <strong>(Spent AAs - 150)</strong> for each alt.</li>
  <li>If any result is below <strong>0</strong>, count that as <strong>0</strong> instead.</li>
  <li>Add all resulting values to get your <strong>total potential AA bonus cap</strong>.</li>
  <li>If that sum is <strong>greater than 150</strong>, it overrides the default bonus cap.</li>
</ol>
<hr>
<h2>Example</h2>
<p>Consider the following three characters and their spent AAs:</p>
<ul>
  <li><strong>Character A:</strong> 200 spent AAs</li>
  <li><strong>Character B:</strong> 300 spent AAs</li>
  <li><strong>Character C:</strong> 150 spent AAs</li>
</ul>
<p>After applying the formula <strong>(Spent AAs - 150)</strong> (treat negatives as 0):</p>
<ul>
  <li><strong>Character A:</strong> (200 - 150) = <strong>50</strong></li>
  <li><strong>Character B:</strong> (300 - 150) = <strong>150</strong></li>
  <li><strong>Character C:</strong> (150 - 150) = <strong>0</strong></li>
</ul>
<p><strong>Total = 50 + 150 + 0 = 200</strong></p>
<p>Since <strong>200</strong> is greater than the default <strong>150</strong>, your new AA bonus cap is <strong>200</strong>.</p>
<hr>
<h2>Bonus Mechanic Explained</h2>
<p>You receive a <strong>300% uncapped bonus EXP</strong> for your AA Veterancy Bonus. However, this <strong>300% bonus</strong> gradually scales down as you approach your maximum Veterancy <strong>(i.e., as you near the end of your Veteran AA).</strong></p>
<p><strong>Important Note:</strong> The <strong>currently logged-in character</strong> is <strong>not</strong> counted toward the total. Only additional characters (alts) contribute to your bonus cap.</p>
<hr>
<h2>Tips, Tricks, and Strategies</h2>
<p><strong>Level Multiple Characters:</strong> Having more alts with AAs above 150 helps push your total bonus higher.</p>
<p><strong>Balance Your Playtime:</strong> Keep your alts progressing so their spent AAs increase over time.</p>
<p><strong>Use the Bonus Wisely:</strong> Plan to grind AAs on new characters when your total Veterancy is high.</p>
<hr>


![pagebreak2.webp](/pagebreak2.webp){.align-center}