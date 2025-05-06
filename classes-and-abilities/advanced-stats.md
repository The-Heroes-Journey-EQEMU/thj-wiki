---
title: Advanced Stats
description: Advanced Stats for THJ
published: true
date: 2025-05-06T13:25:31.079Z
tags: 
editor: markdown
dateCreated: 2025-05-06T13:11:26.422Z
---

<div class="page-wrapper">
  <!-- ────────── Header Card ────────── -->
  <div class="heroic-header-card">
    <img src="/classes-and-abilities/statsandclasses.webp"
         alt="Stats and Classes Banner"
         class="heroic-banner">
    <h1>Advanced Stats</h1>
  </div>
<!-- ────────── TOC (updated) ────────── -->
<section class="stat-section">
  <h2>Table of Contents</h2>
  <ul class="toc">
    <li>
      <a href="#spell-shield">Spell&nbsp;Shield</a>
      <a href="#shielding">Shielding</a>
      <a href="#damage-shield">Damage&nbsp;Shield</a>
      <a href="#dot-shielding">DoT&nbsp;Shielding</a>
      <a href="#damage-shield-mitigation">Damage&nbsp;Shield&nbsp;Mitigation</a>
      <a href="#avoidance">Avoidance</a>
      <a href="#accuracy">Accuracy</a>
      <a href="#stun-resist">Stun&nbsp;Resist</a>
      <a href="#strikethrough">Strikethrough</a>
      <a href="#heal-amount">Heal&nbsp;Amount</a>
      <a href="#spell-damage">Spell&nbsp;Damage</a>
      <a href="#clairvoyance">Clairvoyance</a>
    </li>
  </ul>
</section>
<hr>
  <!-- ────────── STAT BLOCKS ────────── -->
  <section class="stat-block" id="spell-shield">
    <h3>Spell Shield</h3>
    <p><strong>Spell Shield</strong> is a worn item stat that reduces direct spell damage (non-DoT) <em>before</em> any spell runes or absorptions apply. It functions as flat percentage mitigation against incoming harmful spellcasts&mdash;nukes, AE spells, and direct magical attacks.</p>
    <p>This effect stacks with other forms of mitigation such as <em>Mitigate&nbsp;Spell&nbsp;Rune</em> and <em>Absorb&nbsp;Magic</em>, but is <strong>applied first</strong>, helping preserve rune-based defenses. It does <em>not</em> reduce DoT (damage-over-time) effects&mdash;DoT Shielding handles that separately.</p>
    <ul>
      <li>Example: With <strong>25&nbsp;% Spell Shield</strong>, an incoming 1000-damage nuke is reduced to 750 before any runes are checked.</li>
      <li>Capped at <strong>35&nbsp;%</strong> total mitigation.</li>
      <li>Useful against magic-heavy NPCs, spellcasting PvP opponents, or AE boss encounters.</li>
    </ul>
    <h4>Important Notes</h4>
    <ul>
      <li>Spell Shield does <em>not</em> absorb damage; it simply reduces the raw value of the spell hit.</li>
      <li>Especially powerful when paired with threshold or mitigation runes that would otherwise deplete too quickly.</li>
    </ul>
  </section>
  <section class="stat-block" id="shielding">
    <h3>Shielding</h3>
    <p><strong>Shielding</strong> (also shown as <em>Melee Mitigation</em> on items) reduces the flat damage bonus that NPCs add to their melee attacks. This bonus is separate from the damage that comes from the normal DI (damage interval) roll (also called base damage) and is commonly referred to as the mob’s minimum hit or bonus damage.</p>
    <p>When an enemy makes a melee attack, the game calculates a damage roll between two values:</p>
    <ul>
      <li><strong>Base damage</strong>&nbsp;&mdash; a roll from 1.0&nbsp;to&nbsp;2.0 against the mob’s DI value.</li>
      <li><strong>Bonus damage</strong>&nbsp;&mdash; a fixed value added from the mob’s damage table. <em>This</em> is the part Shielding affects.</li>
    </ul>
    <p>The Shielding stat <strong>reduces only the bonus damage portion, not the base damage roll</strong>.</p>
    <p><code>Reduced&nbsp;Bonus&nbsp;=&nbsp;Bonus&nbsp;Damage&nbsp;×&nbsp;(1&nbsp;−&nbsp;Shielding&nbsp;%)</code></p>
    <p>Example: A mob has a hit range of 110–310 (DI&nbsp;10&nbsp;+&nbsp;100&nbsp;bonus). With <strong>5&nbsp;% Shielding</strong>, the bonus damage becomes 95, so the new range is <strong>105–305</strong>.</p>
    <p>The actual mitigation depends entirely on the mob’s bonus damage. If an NPC has no bonus damage, Shielding has no effect.</p>
    <h4>Important Notes</h4>
    <ul>
      <li>Only affects melee and ranged <em>physical</em> damage&mdash;not spells, DoTs, or abilities.</li>
      <li>Capped by <code>ItemShieldingCap&nbsp;=&nbsp;35&nbsp;%</code>.</li>
      <li>Effectiveness is mob-dependent: great vs. large bonus damage, negligible vs. none.</li>
      <li>Does not reduce critical hits, special attacks, procs, or spell-based damage.</li>
    </ul>
  </section>
  <section class="stat-block" id="damage-shield">
    <h3>Damage Shield</h3>
    <p>The <strong>Damage Shield</strong> worn item stat causes attackers to take non-melee damage when they land a melee hit on the wearer. This triggers passively; the player need not act.</p>
    <p>Unlike spell-based damage shields (negative values interpreted as outgoing damage), <em>item</em> Damage Shield bonuses are added on top of existing spell shields. On their own, item bonuses cause no damage unless the player already has a spell- or AA-granted shield active.</p>
    <p>Once a shield is active, item bonuses increase its total damage. That final value is then reduced by the attacker’s mitigation before applying damage.</p>
    <ul>
      <li>Requires an active DS from a spell or AA to function.</li>
      <li>Item bonuses stack additively with spell/AA sources.</li>
      <li>Reflects non-melee reactive damage on melee hits only.</li>
      <li>Does <em>not</em> affect damage you deal; only reflects on attackers.</li>
      <li>Does not trigger on spell hits, procs, or ranged attacks.</li>
    </ul>
    <h4>Important Notes</h4>
    <ul>
      <li>Mobs may have defenses that mitigate incoming DS damage.</li>
      <li>Off-hand (dual-wield) swings can trigger reduced DS damage.</li>
      <li>Some enemies appear “resistant” even when the shield is active.</li>
    </ul>
  </section>
  <section class="stat-block" id="dot-shielding">
    <h3>DoT Shielding</h3>
    <p>The <strong>DoT Shielding</strong> worn item stat reduces damage taken from damage-over-time (DoT) effects&mdash;poisons, diseases, curses, and magical DoTs that tick over time.</p>
    <p>When affected by a DoT, the server calculates total mitigation as:</p>
    <pre><code>total_DoTShielding =
  item_DoTShielding +
  spell_MitigateDotRune% +
  AA_MitigateDotRune%</code></pre>
    <p>(Only the item portion is visible in item stats.)</p>
    <p>Each tick uses:</p>
    <pre><code>reduced_damage = damage − (damage × total_DoTShielding ÷ 100)</code></pre>
    <p>Example: A 100-damage tick with <strong>20&nbsp;% DoT Shielding</strong> becomes 80 damage.</p>
    <h4>Important Notes</h4>
    <ul>
      <li>Applies to periodic ticks only; not to any initial “front-load” damage.</li>
      <li>Stacks additively with spell/AA mitigation (not shown in UI).</li>
      <li>Capped at <strong>35&nbsp;%</strong> on this server.</li>
      <li>Rune-style DoT absorbs are separate and stack with DoT Shielding.</li>
    </ul>
  </section>
  <section class="stat-block" id="damage-shield-mitigation">
    <h3>Damage Shield Mitigation</h3>
    <p><strong>Damage Shield Mitigation</strong> reduces the damage you take when striking an enemy that has an active damage shield. It only matters when <em>you</em> are the attacker receiving reactive DS damage.</p>
    <p>The item stat works in two parts:</p>
    <ul>
      <li><strong>Flat reduction</strong> &mdash; subtracts a fixed amount first.<br>
          <em>Example:</em> 60-point DS &minus; 20 flat mitigation ⇒ 40.</li>
      <li><strong>Percentage reduction</strong> &mdash; then lowers the remaining damage.<br>
          <em>Example:</em> 40 × (1 − 0.25) ⇒ 30 damage.</li>
    </ul>
    <p>Flat and percentage values stack but are applied sequentially. Off-hand swings use their own mitigation values, letting dual-wield builds specialize.</p>
    <h4>Important Notes</h4>
    <ul>
      <li>Does <em>not</em> reduce damage from your own DS or incoming spells.</li>
      <li>Flat first, then percent &mdash; always applied in that order.</li>
      <li>Extremely valuable vs. high-DS raid bosses or caster-type NPCs.</li>
      <li>Off-hand mitigation applies only to secondary-weapon swings.</li>
    </ul>
  </section>
  <section class="stat-block" id="avoidance">
    <h3>Avoidance</h3>
    <p><strong>Avoidance</strong> is a worn item stat that passively improves your chance to avoid incoming melee attacks by lowering the attacker’s chance to hit.</p>
    <p>Implemented as a “Mod2” item stat, it adds directly to the defender’s avoidance roll:</p>
    <ul>
      <li>Scaled by <code>PCAccuracyAvoidanceMod2Scale</code>. On THJ, <strong>1 point = −1</strong> to enemy hit chance (before other modifiers such as the attacker’s Accuracy).</li>
      <li>The final roll weighs attacker Accuracy, RNG, positioning, skills, etc.</li>
      <li>Applies only to melee and ranged hits; does not affect spell accuracy or procs.</li>
    </ul>
    <h4>Important Notes</h4>
    <ul>
      <li>Avoidance is simply added; it has no special stacking rules.</li>
      <li>Works in tandem with the attacker’s Accuracy.</li>
      <li>Indirect boosts: Heroic Agility, avoidance-focused buffs, etc.</li>
      <li>Not the same as Dodge, Block, or Parry&mdash;those fire <em>before</em> this hit-chance roll.</li>
    </ul>
    <p><em>Roll order example:</em> Riposte → Dodge → &hellip; → final hit/miss check (where Avoidance vs. Accuracy applies). Very high attacker Accuracy can soft-cap the benefit of Avoidance.</p>
  </section>
  <section class="stat-block" id="accuracy">
    <h3>Accuracy</h3>
    <p>The <strong>Accuracy</strong> worn item stat increases your chance to land melee attacks, directly opposing the target’s Avoidance <em>after</em> active defenses (Riposte, Block, Parry, Dodge) have failed.</p>
    <p>Accuracy adds a flat bonus to your final to-hit roll:</p>
    <ul>
      <li>Each point yields a small but tangible increase.</li>
      <li>Example: Base hit chance 60&nbsp;%. Add 50 Accuracy ⇒ final hit chance ≈ 65&nbsp;% (other modifiers apply).</li>
      <li>Factors into a larger equation of base accuracy, skill bonuses, HitChance effects, and enemy Avoidance.</li>
    </ul>
    <h4>Important Notes</h4>
    <ul>
      <li>Applies to melee, archery, and throwing; does <em>not</em> affect spellcasting or procs.</li>
      <li>Diminishing impact vs. extremely high Avoidance targets, but it is still a flat modifier &mdash; not a sequential roll.</li>
      <li>Not all sources stack equally; buffs, spells, items, and AAs may share caps or overwrite.</li>
    </ul>
  </section>
</div>
<!-- ───────── ADDITIONAL STAT BLOCKS ────────── -->
<section class="stat-block" id="stun-resist">
  <h3>Stun Resist</h3>
  <p>The <strong>Stun&nbsp;Resist</strong> worn item stat increases a character’s chance to resist melee-based stun effects, such as those triggered by Bash, Kick (Warriors), or stun-triggering procs and abilities. This stat provides a passive percentage-based chance to avoid being stunned once a stun effect has successfully landed.</p>
  <p>Stun&nbsp;Resist is applied <em>after</em> the stun attempt has bypassed all other requirements&mdash;valid attack angle, stun-immunity flags, skill prerequisites, and the base stun chance. It does <strong>not</strong> prevent interrupts or other secondary effects, but it directly negates the stun state itself if the resistance check succeeds.</p>
  <ul>
    <li>When a stun-capable attack lands, the game performs a roll against your total Stun&nbsp;Resist bonus (items + spells + AAs).</li>
    <li>If the random roll is ≥ your Stun&nbsp;Resist value, the stun is resisted (e.g., <em>30&nbsp;Stun&nbsp;Resist</em> ⇒ 30 % chance to avoid the stun).</li>
    <li>This check happens <em>after</em> any Frontal Stun Resist bonus is applied and <em>before</em> the stun effect is finalized.</li>
  </ul>
  <h4>Important Notes</h4>
  <ul>
    <li>Applies only to physical/melee stuns&mdash;spell-based stuns use separate saving throws.</li>
    <li>Stacks additively with Frontal Stun Resist, but each is checked independently.</li>
    <li>Binary outcome: it doesn’t shorten stun duration, it simply resists or fails.</li>
    <li>Some races/classes have inherent stun immunities that bypass this system entirely.</li>
  </ul>
</section>
<section class="stat-block" id="strikethrough">
  <h3>Strikethrough</h3>
  <p>The <strong>Strikethrough</strong> worn item stat gives a player the ability to bypass defensive avoidance checks (Riposte, Parry, Block, Dodge). When an opponent successfully performs one of these maneuvers, Strikethrough provides a chance for the attack to <em>still</em> land, partially negating that avoidance.</p>
  <p>This effect applies to melee or physical skill-based attacks&mdash;not spells, damage shields, or procs. It is an <em>offensive</em> stat that enhances consistency against evasive targets with high Avoidance or Heroic Agility.</p>
  <ul>
    <li>After an attack is dodged/blocked/parried/riposted, a roll ≤ your Strikethrough&nbsp;% (capped at 35) lets the swing connect anyway.</li>
    <li>The salvaged hit lands for <strong>1&nbsp;damage</strong>, but still triggers downstream effects (procs, augments, hate generation).</li>
  </ul>
  <h4>Important Notes</h4>
  <ul>
    <li>Rolled <em>after</em> standard avoidance checks have already ruled the swing avoided.</li>
    <li>No skill-type restriction: because the check occurs post-avoidance, Archery and Throwing can Strikethrough too.</li>
    <li>Does not increase base hit chance; it only rescues otherwise-avoided swings.</li>
    <li>Chat text “You strike through your opponent’s defenses!” appears on success.</li>
  </ul>
</section>
<section class="stat-block" id="heal-amount">
  <h3>Heal Amount</h3>
  <p>The <strong>Heal&nbsp;Amount</strong> worn item stat increases the base healing of your direct heal spells (and, in some scenarios, runes). It allows healers—and hybrids who heal—to scale output beyond the raw spell value, which is crucial in high-throughput or group-healing situations.</p>
  <p>The intuitive idea is that Heal&nbsp;Amount simply adds to a spell’s base heal, but in code it actually scales by the spell’s mana cost, level, and other conditions. The exact formula is complex, yet the bottom-line effect is more healing per cast as your Heal&nbsp;Amount rises.</p>
</section>
<section class="stat-block" id="spell-damage">
  <h3>Spell Damage</h3>
  <p>The <strong>Spell&nbsp;Damage</strong> stat increases the amount of damage dealt by your offensive spells. This bonus is additive and is especially effective for frequent, lower-damage spells such as DoTs, procs, and quick nukes.</p>
  <p>At face value, it looks like 100 % inheritance to direct-damage spells and ~50 % to DoTs, yet these figures can shift depending on how developers fine-tune class features. Always review patch notes or the change-log to see if inheritance values have been adjusted for your class.</p>
</section>
<section class="stat-block" id="clairvoyance">
  <h3>Clairvoyance</h3>
  <p>The <strong>Clairvoyance</strong> worn item stat provides a chance to recover mana after casting a spell. It doesn’t lower the upfront cost; instead, it refunds a portion afterward, effectively reducing net mana spent.</p>
  <p>When casting any spell within <em>5 levels</em> of your current level:</p>
  <ul>
    <li>The game rolls 1–100.</li>
    <li>That roll is treated as a percentage of your total Clairvoyance value.</li>
    <li>The resulting amount is refunded, up to the spell’s total mana cost.</li>
  </ul>
  <p><strong>Example</strong>: You have 200 Clairvoyance and cast a 100-mana spell. The roll is 30 ⇒ 30 % of 200 = 60 mana refunded ⇒ final cost = 40.</p>
  <h4>Important Notes</h4>
  <ul>
    <li>Cannot refund more than the spell costs—never produces net mana gain.</li>
    <li>Works only on spells ≤ 5 levels below you.</li>
    <li>Random by nature: high Clairvoyance may still yield low refunds on some casts.</li>
    <li>Only worn stats count—AA or spell effects do not boost Clairvoyance.</li>
    <li>Benefits high-frequency casters (healers, nukers) the most.</li>
  </ul>
</section>
<!-- ────────── Decorative footer image ────────── -->
<img src="/pagebreak4.webp" alt="Decorative footer" class="align-center">
