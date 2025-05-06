---
title: Advanced Stats
description: Advanced Stats for THJ
published: true
date: 2025-05-06T13:13:54.082Z
tags: 
editor: markdown
dateCreated: 2025-05-06T13:11:26.422Z
---

![statsandclasses.webp](/classes-and-abilities/statsandclasses.webp){.align-center}

# Advanced Stats

## Spell Shield
**Spell Shield** is a worn item stat that reduces direct spell damage (non-DoT) before any spell runes or absorptions apply. It functions as flat percentage mitigation against incoming harmful spellcasts, including nukes, AE spells, and direct magical attacks.

This effect stacks with other forms of mitigation such as Mitigate Spell Rune and Absorb Magic, but is **applied first**, helping to preserve rune-based defenses. It does not reduce DoT (damage-over-time) effects — DoT shielding handles that separately.

- Example: With 25% Spell Shield, an incoming 1000 damage nuke is reduced to 750 damage before any runes are checked.
- Capped at 35% total mitigation.
- Useful against magic-heavy NPCs, spellcasting PvP opponents, or AE boss encounters.

**Important Notes**
- Spell Shield does not absorb damage, it simply reduces the raw value of a spell hit. 
- It’s especially powerful when paired with threshold or mitigation runes that would otherwise deplete too quickly.

----------------
## Shielding
**Shielding** (also shown as Melee Mitigation on items) reduces the flat damage bonus that NPCs add to their melee attacks. This bonus is separate from the damage that comes from the normal DI (damage interval) roll (also known as base damage) and is commonly referred to as the mob's minimum hit or bonus damage.

When an enemy makes a melee attack, the game calculates a damage roll between two values:

- Every NPC melee attack consists of two parts:
  - Base damage — determined by a roll from 1.0 to 2.0 against the mob’s DI value.
  - Bonus damage — a fixed value added to the attack based on the mob’s damage table. This is the part Shielding affects.
- The Shielding stat **reduces only the bonus damage portion, not the base damage roll**.

The reduction is calculated as:
```Reduced Bonus = Bonus Damage × (Shielding %)```
For example, if a mob has a base hit range of 110–310 (DI of 10 + 100 bonus), and you have 5% Shielding, the bonus damage would be reduced to 95, making your new hit range from that mob 105–305.

The actual mitigation depends entirely on the mob's bonus damage. If an NPC has no bonus damage, Shielding has no effect.

**Important Notes**
- Shielding only affects melee and ranged phsyical damage — not spells, dots, or abilities.
- This reduction is capped by ItemShieldingCap, which is 35% here.
- The effectiveness of Shielding is mob-dependent. It’s highly effective against mobs with large bonus damage values and nearly ineffective against those with none.
- Shielding does not reduce critical hits, special attacks, procs, or spell-based damage.

----------------------
## Damage Shield
The **Damage Shield** worn item stat causes attackers to take non-melee damage when they land a successful melee hit on the wearer. This effect does not require the player to take any action — it passively triggers when struck in melee combat.

Unlike spell-based damage shields, which apply negative values that are interpreted as outgoing damage, item-based Damage Shield bonuses are added on top of existing spell shields. On their own, **item bonuses do not cause damage unless the player already has a spell-based or AA-granted damage shield active**.

Once a shield is active, item bonuses increase its total damage output. This final value is then reduced by the attacker’s mitigation, if any, before applying damage.

- Requires an active damage shield from a spell or AA to function.
- Item bonuses stack additively with spell/AA sources.
- Contributes to non-melee reactive damage when struck by melee attacks.
- Does not affect damage dealt by the player — only reflects damage onto attackers.
- This effect does not trigger on spell hits, procs, or ranged attacks.

**Important Notes**
Attackers may reduce the damage per hit from your damage shield through mitigation effects:

- If mobs have special defenses that specifically mitigate incoming DS damage.
- Offhand attacks from dual-wielding NPCs or players may trigger reduced DS damage.
- Certain enemies might appear "resistant" to DS effects even though the shield is active and other mobs take full damage.

---------------------------
## DoT Shielding
The **DoT Shielding** worn item stat reduces the damage taken from damage-over-time (DoT) effects. This includes effects such as poisons, diseases, curses, and any magical DoTs that deal their damage over a series of ticks.

When you are affected by a DoT, the server calculates the total damage reduction using:
DoT Shielding = 
    item DoTShielding 
  + spell-based mitigation (MitigateDotRune%) 
  + AA-based mitigation (MitigateDotRune%)```
Only the item portion is exposed to players directly via item stats.

The formula applied each tick is:
```reduced_damage = damage - (damage * total_DoTShielding / 100)```
For example, if a **DoT tick would normally deal 100 damage and you have 20% DoT Shielding, you only take 80 damage per tick**.

**Important Notes**
- This only applies to periodic damage ticks, not the initial application of the DoT if it does immediate damage.
- DoT Shielding stacks additively with spell/AA-based mitigation, though these other sources are not shown in the UI.
- The mitigation is capped at a server-defined maximum, which is 35% here.
- Some buffs may apply additional rune-based shielding on top of DoT Shielding that absorb DoT damage in chunks. These are separate from item stats and handled via spell effects.

------------------
## Damage Shield Mitigation
The **Damage Shield Mitigation** worn item stat reduces the amount of damage a character takes when striking an enemy that has an active damage shield. These shields reflect damage back to the attacker when a melee hit lands, and this stat helps reduce that reflected damage.

This mitigation applies only when the player is the attacker and is receiving reactive damage from an opponent’s damage shield.

The item stat works in two parts:

- A flat damage reduction is applied first, subtracting a fixed amount from the incoming damage. For example, if the damage shield would normally reflect 60 damage and the attacker has 20 flat mitigation, the result would be 40 damage taken.
- A percentage-based reduction is applied next, reducing the remaining damage by a specified percent. Using the previous example, if the attacker also had 25% damage shield mitigation, they would then take only 30 damage (25% less than 40).

These two effects — flat reduction and percentage mitigation — are applied together, in sequence, to maximize protection. Offhand attacks (like dual-wielding weapons) apply their own specific mitigation values, allowing some specialization in builds that rely heavily on secondary weapon damage.

**Important Notes**
- This stat does not reduce damage from your own damage shield or incoming spells — only from damage shield effects triggered by melee attacks.
- Flat mitigation and percentage mitigation stack, but are applied in sequence (flat first, then percent).
- Damage Shield Mitigation can be especially valuable when fighting enemies with high damage shield values, such as certain raid bosses or caster-type NPCs.
- Offhand mitigation applies only to attacks made with your secondary weapon, if dual-wielding.

---------------
## Avoidance
**Avoidance** is a worn item stat that passively improves your chances of avoiding incoming melee attacks. It specifically reduces the attacker’s chance to land a successful hit by making their attack roll less likely to succeed.

Avoidance functions as an item-based "Mod2 stat" in code, and is applied as a flat bonus to the defender’s avoidance check during combat resolution.

- The value of Avoidance is scaled by a server rule (PCAccuracyAvoidanceMod2Scale), which adjusts how impactful the stat is. On THJ, each point reduces the enemy’s chance to hit by 1 (which will later be altered by other modifiers, including the attacker's accuracy).
- The roll to see if you can avoid is largely checked against the attackers accuracy but also includes other modifiers that add to hit chance, RNG, positioning, and other class abilities.
- Avoidance is added directly to your evasion score in the math used to resolve that combat check.
- Avoidance only affects melee and ranged hits and does not reduce spell accuracy, or procs.

**Important Notes**
- Avoidance does **not stack** with itself in any special way; it's simply added to the total avoidance roll during combat.
- It works in tandem with Accuracy, which is the opposing stat used by attackers to improve their hit chance.
- Some classes, gear, or buffs may improve Avoidance indirectly via Heroic Agility or avoidance-focused modifiers.
- This stat is not the same as Dodge, Block, or Parry; those are discrete avoidance types checked separately before the hit roll. Avoidance comes into play after those checks, as part of the final hit chance resolution.
  - For example: Active defense skills are checked first (Riposte → Dodge).
  - If none of those fire, the game then calculates whether the attack actually hits or misses based on the attacker’s Accuracy vs. the defender’s Avoidance, among other factors.
  - Avoidance stat influences the final melee and ranged hit chance — making it harder for the attacker to land a blow if they reach this point.

That said, there is an effective cap (or at least soft diminishing returns) if the attacker’s Accuracy is high enough, because Avoidance modifies their hit chance — and that’s subject to all other modifiers like level, ATK, hit chance bonuses, etc.

--------------------
## Accuracy
The **Accuracy** worn item stat increases a character’s chance to land a successful melee attack on an opponent. This stat directly improves your odds of bypassing the target’s Avoidance and landing a hit after any active defensive checks (Riposte, Block, Parry, Dodge) have failed.

Accuracy adds a flat bonus to your calculated hit chance, modifying the final to-hit roll used to determine whether an attack lands or misses.

The stat is one part of a larger calculation involving base accuracy, hit chance effects, skill-based bonuses, and enemy Avoidance.

- Each point of Accuracy increases your hit rate by a small, flat amount.
- For example, if your base hit chance is 60%, and you have 50 Accuracy, your final hit chance could rise to around 65% or more, depending on other modifiers.
- The Accuracy stat is added to the total hit chance after applying class-based bonuses, skill modifiers, and HitChance percentages.

In general, against high Avoidance targets (such as raid bosses), Accuracy helps overcome that higher evasion to ensure more reliable hits.

**Important Notes**
- Accuracy only applies to melee, archery, and throwing skills, but does not affect spellcasting or combat procs.
- Like Avoidance, Accuracy has diminishing impact against enemies with extremely high defensive ratings, but it does not follow a sequential roll — it’s used in a final hit/miss calculation.
- Not all sources of Accuracy stack equally — buffs, spells, items, and AAs may overlap or share caps depending on the source.

----------------------
## Stun Resist
The **Stun Resist** worn item stat increases a character’s chance to resist melee-based stun effects, such as those triggered by Bash, Kick (Warriors), or stun-triggering procs and abilities. This stat provides a passive percentage-based chance to avoid being stunned once a stun effect has successfully landed.

Stun Resist is applied after the stun attempt has bypassed all other requirements: valid angle of attack, stun immunity flags, skill prerequisites, and base stun chance.

It **does not prevent interrupts or other secondary effects**, but it directly negates the stun state itself if the resistance check succeeds.

- When a stun-capable attack lands, the game performs a roll against your total Stun Resist bonus from items, spells, and AAs.
- If the random roll is greater than or equal to your total Stun Resist, the stun is resisted.
- For example, if you have 30 Stun Resist and a stun effect successfully triggers, there is a 30% chance you will avoid being stunned.
- This check happens after any “Frontal Stun Resist” bonus is applied (which occurs first for frontal attacks), and before the stun effect is finalized.

**Important Notes**
- Stun Resist only applies to physical/melee-based stuns — spell stuns use separate saving throw checks.
- It stacks additively with Frontal Stun Resist, but both are checked independently.
- The item bonus does not affect stun durations — it is strictly a binary resist or fail effect.
- Some classes or races have stun immunities that override this system entirely. In those cases, Stun Resist is not checked.

----------------
## Strikethrough
The **Strikethrough** worn item stat gives a player the ability to bypass defensive avoidance checks that would normally cause their melee attack to be completely avoided. These checks include Riposte, Parry, Block, and Dodge. When an opponent successfully performs one of these defensive maneuvers, Strikethrough provides a chance for the attack to still land, partially negating that avoidance.

This effect applies only to melee or physical skill-based attacks, not spells, damage shields, or procs. In addition, Strikethrough is an offensive stat, enhancing a player’s consistency in landing physical attacks against evasive targets, especially those with high avoidance or heroic agility.

- When a melee swing is avoided by a defender (via dodge, block, parry, or riposte), and the attacker has Strikethrough, a percentage-based roll is performed.
- If the roll is less than or equal to the attacker’s total Strikethrough chance, the attack is allowed to go through despite being avoided.
- Strikethrough is capped at 35, so at max value this would give the player a 35% chance to succeed a strikethrough roll.
- **The attack then hits for minimal damage (1), but still allows for downstream effects (e.g., procs, weapon augments, hate generation) to occur**.

**Important Notes**
- Strikethrough is rolled after all standard avoidance checks have already caused the attack to be avoided.
- There is no skill-type restriction for Strikethrough, it's doing a check against avoidance, and while there are skill-based avoidance checks like Parry and Dodge, the check for Strikethrough happens after AvoidDamage fails, so Archery and Throwing would apply.
- It does not increase your chance to hit directly but rather salvages otherwise-deflected attacks.
- The visual cue “You strike through your opponent’s defenses!” will appear when it activates.
- It is especially useful in high-level content where NPCs have inflated avoidance stats or defensive disciplines.

------------------------
## Heal Amount
The **Heal Amount** worn item stat increases the base healing of your direct heal spells (and other effects like Runes in some scenarios). It allows healers—and hybrid casters with healing capabilities—to scale their healing output beyond the raw spell value, making this stat particularly useful in high-output or group healing scenarios.

The simple definition is that it just adds to the base heal amount, but nothing in code supports that (code has it scaling based on mana/level of spell with a bunch of other scaling conditions)

--------------
## Spell Damage
The **Spell Damage** stat increases the amount of damage dealt by your offensive spells. This bonus is additive and is especially effective for frequent, low-damage spells such as damage-over-time (DoT) effects, procs, and fast-cast nukes.

At face valuem, it seems as simple as 100% inheritance to base spell damage for direct spells and 50% for DoTs, but this value can change based on how the developers have dialed in certain class features. I recommend checking the change-log to see if spell damage inheritance has changed for certain features.

------------
## Clairvoyance
The **Clairvoyance** worn item stat provides a chance to recover mana when casting a spell. It doesn’t reduce the base cost of the spell directly but instead returns some portion of that mana after the spell is cast, effectively lowering the net cost.

When casting any level-appropriate spell (**within 5 levels of your current level**), you have a random chance to regain some of the spell’s mana cost.

The amount of mana you can recover per cast is up to your total Clairvoyance stat.

- When you cast a qualifying spell:
  - The game rolls a number between 1 and 100.
  - That roll is used as a percentage of your total Clairvoyance value.
  - The resulting amount is the mana you recover, up to the spell’s total mana cost.
  - You never regain more than the spell costs.
- Example:
  - You have 200 Clairvoyance and cast a 100 mana spell.
  - The game rolls a 30.
  - You recover 30% of 200 = 60 mana.
  - Final mana cost of the spell: 100 - 60 = 40 mana.

**Important Notes**
- Clairvoyance can only return mana up to the spell’s mana cost—it will not generate net mana.
- It only works on spells that are no more than 5 levels below your current level.
- The effect is random, so even with high Clairvoyance you may occasionally recover very little (or no) mana from a cast.
- Only worn item stats contribute; AA or spell effects do not influence Clairvoyance.
- This stat benefits classes with high casting frequency (e.g., healers, nukers) the most, as more spell casts mean more chances to recover mana.

![pagebreak4.webp](/pagebreak4.webp){.align-center}