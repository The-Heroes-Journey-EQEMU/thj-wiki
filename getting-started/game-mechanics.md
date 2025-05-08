---
title: Game Mechanics
description: 
published: true
date: 2025-05-08T14:38:32.218Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:27:41.914Z
---

<article class="game-mech-wrapper">

![statsandclasses.webp](/classes-and-abilities/statsandclasses.webp){.hero-banner}

# Game Mechanics

<p class="divider"></p>

## Introduction
Welcome to the **Game Mechanics** guide for *The Heroes Journey*! This page covers essential gameplay mechanics, including how various stats influence your character, item upgrading, and advanced combat techniques like flurry and procs.  

> Whether you're looking to maximize your spell damage, understand how healing modifiers work, or optimize your tribute points, this guide provides a comprehensive breakdown to help you get the most out of your adventures. Dive in and explore the mechanics that shape the world of THJ!

<nav class="toc" aria-label="Table of Contents">
<ul>
<li><a href="#spell-damage"                  class="toc-link">Spell Damage</a></li>
<li><a href="#heal-amount"                   class="toc-link">Heal Amount</a></li>
<li><a href="#flurry"                        class="toc-link">Flurry</a></li>
<li><a href="#upgrading-items"              class="toc-link">Upgrading&nbsp;Items</a></li>
<li><a href="#upgrading-bags-and-augs"      class="toc-link">Upgrading&nbsp;Bags&nbsp;and&nbsp;Augs</a></li>
<li><a href="#tribute"                       class="toc-link">Tribute</a></li>
<li><a href="#ui-tips-and-tricks"            class="toc-link">UI&nbsp;Tips&nbsp;and&nbsp;Tricks</a></li>
<li><a href="#procs"                         class="toc-link">Procs</a></li>
<li><a href="#macros"                        class="toc-link">Macros</a></li>
<li><a href="#pet-mechanics"                 class="toc-link">Pet Mechanics</a></li>
<li><a href="#maps"                          class="toc-link">Maps</a></li>
<li><a href="#aas"                           class="toc-link">AA's</a></li>
<li><a href="#resists"                       class="toc-link">Resists</a></li>
<li><a href="#dispelling-mobs"               class="toc-link">Dispelling&nbsp;Mobs</a></li>
</ul>
</nav>

---

## Spell Damage {#spell-damage}

- Gear with int on it (regular, enchanted, and legendary) tends to have spell damage on legendary gear.  
- Spell damage has a cap of 750  
- Spell damage increases single target DoT spells with a 2 to 1 ratio (2 spell damage = 1 damage increase)  
- Spell damage does not influence bard song AE dots  
- Spell damage is found in your inventory window, on the stats page.  
- Spell damage increases proc DD spell effect damage amount with a 1 to 1 ratio  
- Spell damage increases sympethic strike DD damage amount with a 1 to 1 ratio  
- Spell damage increases AE DD spell damage amount with a 1 to 1 ratio  

## Heal Amount {#heal-amount}

- Gear with wis on it (regular, enchanted, and legendary) tends to have heal amount on legendary gear.  
- Heal amount has a cap of 750  
- Heal amount increases single target heal spells heal amount with a 1 to 1 ratio  
- Heal amount is found in your inventory window, on the stats page.  
- Heal amount affects runes, their absorption amount is increased with a 1 to 1 ratio  
- Heal amount affects sympethic healing value amount with a 1 to 1 ratio  

## Flurry {#flurry}

- Warriors and Berserkers get an AA called flurry  
- You must have the triple attack skill and succeed a roll to trigger flurry  
- You must succeed a roll on: double attack, triple attack.  
  - Two rolls are then executed for flurry; if you succeed each roll, you can attack up to 5 times in a single round  

## Upgrading Items {#upgrading-items}

- If an item can be placed in your power slot, you will find that mobs that give you experience will also give item experience  
- If you use the Consume Item AA while holding the same item as the one in your power slot of any quality, it will be destroyed to increase the level of the item in your power slot  
- If you do level up an item via the power slot, it immediately becomes **NO TRADE**  
- To upgrade a regular item to enchanted, it requires 3 regular items to be merged with an existing one (4 total)  
- To upgrade an enchanted item to legendary, it requires 3 enchanted items to be merged with an existing one (4 total)  

## Upgrading Bags and Augs {#upgrading-bags-and-augs}

- Augs and Bags are intentionally flagged to not be able to go into the power slot  
- Items not in the power slot cannot be leveled or use the consume item AA to level them up  
- This was a design decision, to make legendary bags and legendary augs more valuable  

## Tribute {#tribute}

- In the bazaar at the east bank near a Mischievous Halfling, you'll find **Aeyln D`Sai** (Tribute Master)  
- Many items can be given to this NPC to gain a point system called **favor**  
- This NPC also lets you set various focus effects and stat bonuses that favor will cost to maintain  
- Press **ALT+U** to open your tribute window  
  - Press **Activate** to turn on tribute. Press **Deactivate** to disable it  
- Tribute will consume the *Active Cost* amount every 10 minutes until turned off. *Current Favor* shows your remaining tribute points  

## UI Tips and Tricks {#ui-tips-and-tricks}

- Pick up a bag and **CTRL + Left-Click** another bag to transfer all items from the held bag into the target bag  
- **SHIFT + Right-Click** a corpse to auto-loot all contents  
- **SHIFT** while pressing *Sell* sells the full stack of the highlighted item (also works when buying)  
- **CTRL** while pressing *Sell* sells a single item from the stack (also works when buying)  

## Procs {#procs}

- Weapon and aug procs do **not** have a PPM limit timer  
- Two-handed and ranged weapons only tap into the “double proc” mechanic if the weapon has a proc **and** at least one aug has a proc  
- Spell buffs have a PPM timer and are prioritized by buff slot ID (lower IDs first)  
- **Buff-proc priority** on a single attack:  
  1. Permanent AAs (no timer)  
  2. Spell-buff procs (timer)  
  3. Ranged-attack procs (timer)  
  4. AA melee procs (timer)  
  5. One-shot poison / *apply poison* effects  
- When a buff proc succeeds it increments a counter; after 4 successes the spell-proc loop ends  
- **Weapon-proc order** per swing: built-in weapon → slot 1 aug → slot 2 aug  

## Macros {#macros}

- [Macros were moved to it's own page](/getting-started/macros)

## Pet Mechanics {#pet-mechanics}

> [!tip]- Pet bonds are very strong in this world  
>  
> In The Heroes Journey universe, pets are much more strongly tied to their owners. So much so that NPC's will sometimes be able to detect this connection. For example, if you command your pet to attack, your enemies may very well ignore the pet and come for its owner, **YOU!** You may need to instruct your pets to taunt these enemies. Beware, if a pet dies, the severed connection will most likely disrupt the stasis state known as Feign Death.  
>  
> [!tip]- Pet specific spells affect all summoned pets  
>  
> You may attune yourself to up to three pets so long as your class selections support this (one pet per class). Because of the strong ties to your pets, many of the pet-specific magicks will affect all of them. While worldy charmed pets will benefit from many spells that specialize on pets, they do not share the same Pet Affinity that summoned pets share in order to receive the benefits of general group spells.  
>  
> [!tip]- You can issue commands to all pets simultaneously or to a single pet  
>  
> By default, your pets will operate in harmony: attacking as a group, holding as a group, even releasing the bonds formed with you as a group. If you wish for a particular pet to execute a command on its own, you must direct your full attention to it by targeting the pet before issuing its command. Note that if you issue a stance command such as taunt or guard to a single pet, then issue the same command to all pets, they will harmoniously remain out of sync.  
>  
> [!tip] - Check the status of those pets and the bling they're carrying!  
>  
> You can check the status of your pets, including the stats, weapons, and armor equipped etc. by using the command:  
> `/say #mystats`

## Maps {#maps}

> [!tip]- Making use of your map  
>  
> On your map, you can see a location of mobs moving around the map. Some MQ2 functionality was imported into THJ, one of these being the `/mapfilter` command. You can do `/mapfilter named` and it will filter out other mobs; you can also do `/mapfilter custom` to enter the name of a specific named mob `(/mapfilter custom Slate)`. Now, when I'm in East Commons, I can open my map and track Sergeant Slate in real time. In addition, if the mob is within range to you, you can right-click it on the map to target it as well, making it a very handy tool for pacify and the sort!  

Note, when you make a new character, go to your skills tab and open the **Track** window one time, and you will be able to see the names of the mobs on your map within range of your track skill as normal, with increased range for higher skill ranks.

## AA's {#aas}

> [!tip]- AA's that stack  
>  
> We always want to look for synergy with our AA's, but we also can't ignore the little, yet arguably more important. Everyone gets **Run 5** as an AA, and that gets you up to *Spirit of the Wolf* speed. **Bard** gets two additional ranks of run with *Fleet of Foot*. **Monk** gets 3 additional ranks via *Weightless Steps*. You get a combined **Run 10**, which is on par with Selo's using Naggy drums. Keep an eye out for class AA's that stack in that way.

## Resists {#resists}

- 2 resists equates to roughly 1 % chance to resist  
- Player resists go up to 550 base. If you're above this number, subtract your heroic resists (the gold +#) from the total, and if that's less than 550, you get benefit from normal resist buffs and gear still. Otherwise, heroic is the only way to increase them.  
- Spells can have *min resists* and *max resists* fields set to modify final resist checks  
- A dice is rolled of 0 to 200 to determine if a spell lands, and returns partial landings as well. The enemy's natural resists, and factors noted below, among some other edge cases are used  

### Outgoing damage spell landing

When you cast a spell on an NPC:

- An enemy with a level greater than yours adds a +1 to all resists with a cap of +9  
- An enemy with a level lower than yours adds a −1 to all resists until the cap of −9  
- An enemy with a level lower than 20 levels of yours adds −1000 to all resist checks  
- Each point of heroic charisma adds −1 to resist check  

### Incoming damage spell landing

When an NPC casts on you:

- An enemy with a level greater than yours adds −1 to all resists with a cap of −15  

## Dispelling Mobs {#dispelling-mobs}

This is just to bring to attention a trend I've seen about bards being able to dispel Innoruuk DS vs others, and a deep dive into how **Cancel Magic** works as a whole.

- Dispel doesn't use resists in any manner.  
- `TryDispel` is a function that takes a player's caster level, the buff level, and a level_modifier.  
- When you try to dispel a mob, the server iterates all buffs on the target mob, and rolls a d100 vs every buff.  

The formula for dispel is as follows:  

- Start with a dispel chance of 32 %  
- Take your caster level, and subtract the enemy's level to get a `level_diff`  
  - There are two ways to modify your caster level: **Jamfest AA** (+6 caster level) and the spell's **level mod** (values below)  
- If `level_diff` > 0, `level_diff` × 7 is added to dispel chance (each level above → +7 %)  
- If `level_diff` < 0, `level_diff` × 2 is added (each level below → −2 %)  
- If `dispel_chance` ≥ 100, success  
- If `dispel_chance` < 10, set to 10 % minimum  
- Roll a d100 vs the final value; success on roll ≤ chance  

**Dispel spells & level mods**

- Cancel Magic +1 level (1 try)  
- Syvelian's Anti-Magic Aria +4 level (1 try)  
- Nullify Magic +4 level (2 tries)  
- Annul Magic +9 level (2 tries)  
- Abolish Magic +9 level (3 tries)  
- Purge Magic +9 level (2 tries)  
- Recant Magic +9 level (4 tries)  
- Pillage Magic +9 level (4 tries)  

#### Scenario 1: Non-bard **Cancel Magic**
To show this in action, if I'm level 60, non-bard and fight Innoruuk (who is level 70)

- dispel_chance = 32 // baseline 32% chance
- my_level = 60 // my level is 60
- my_level += 1 // add cancel magic level mod 1
- level_diff = my_level-70 = -9 // i'm 9 levels below Innoruuk with cancel magic bonus 1
- dispel_chance += level_diff * 2 = 18 // since it's lower than 0, we lower chance by x2 of diff

So any time I use cancel magic, I have a 18% chance to land vs innoruuk


#### Scenario 2: Bard with Jamfest uses Cancel Magic
If I'm a level 60, bard with Jamfest max, and fight Innoruuk (who is level 70)

- dispel_chance = 32 // baseline 32% chance
- my_level = 60 // my level is 60
- my_level += 6 // add jamfest level mod 6
- my_level += 1 // add cancel magic level mod 1
- level_diff = 67-70 =  -3 // i'm 4 levels below Innoruuk with the jamfest +6
- dispel_chance += level_diff * 2 = 26 // since it's lower than 0, we lower chance by x2 of diff

So any time a bard uses cancel magic, they have a 26% chance to land vs innoruuk


#### Scenario 3: Non-bard Annul Magic
- dispel_chance = 32 // baseline 32% chance
- my_level = 60 // my level is 60
- my_level += 9 // add annul magic level mod 9
- level_diff = my_level-70 = -1 // i'm 1 level below Innoruuk with annul magic bonus 9
- dispel_chance += level_diff * 2 = 30 // since it's lower than 0, we lower chance by x2 of diff

So any time I use annul magic, I have a 30% chance to land vs innoruuk, but two rolls, so roughly ~ 51% chance to land (2x30%)

- If an ally puts a debuff on a mob, it has a ~32% chance to be dispelled, since they're equal level to you
- Using higher levels of cancel magic give you multiple rolls per cast, look at the SPA data and how many slots have cancel magic, and that's how many times you are rolling vs each buff/debuff on a target

</article>