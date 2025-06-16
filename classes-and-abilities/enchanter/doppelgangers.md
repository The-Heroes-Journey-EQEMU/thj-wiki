---
title: Doppelgangers
description: Doppelganger and You (and you, and you)
published: false
date: 2025-06-16T17:39:22.615Z
tags: abilities, enchanter, aa, ability, spell, pet, swarm pet
editor: markdown
dateCreated: 2025-06-16T16:47:57.048Z
---

<article class="class-wrapper">
<header class="hero-card">
<img src="/classes-and-abilities/statsandclasses.webp" alt="Classes & Stats Banner" class="hero-banner">
<div class="title-card"><h1 class="hero-title"><span>Enchanter — Doppelgangers</span></h1><img src="/enchanter.gif" alt="Enchanter Flair" class="class-gif"></div>
</header>
  <body>
  <h1>Enchanter Doppelganger AI Behavior</h1>
  <br><h2>Overview</h2>
  <p>
    The Enchanter’s Doppelganger is an AI-controlled pet that automatically casts spells using the Enchanter’s memorized spells. 
    The Doppelganger operates intelligently, prioritizing healing and support for the group while efficiently managing harmful spells on enemies.
  </p>

  <br><h2>Core Behavior</h2>
  <br><h3>Spell Casting Priority System</h3>
  <p>The Doppelganger follows a strict priority system when selecting spells to cast:</p>

  <strong>Beneficial Spells (Priority Order):</strong>
  <ol>
    <li><strong>Heal Over Time (HoT) spells</strong> - Highest priority</li>
    <li><strong>Direct healing spells</strong> - Second priority</li>
    <li><strong>Protective runes</strong> - Third priority</li>
    <li><strong>Other beneficial spells</strong> - Lowest priority</li>
  </ol>

  <strong>Harmful Spells (Priority Order):</strong>
  <ol>
    <li><strong>Resistance debuffs</strong> - Highest priority</li>
    <li><strong>Other debuffs</strong> - Second priority</li>
    <li><strong>Damage over Time (DOT) spells</strong> - Third priority</li>
    <li><strong>Direct damage spells</strong> - Fourth priority</li>
  </ol>

  <br><h2>Healing Behavior</h2>
  <br><h3>Target Selection</h3>
  <p>The Doppelganger will attempt to heal the following targets in order:</p>
  <ul>
    <li>The Enchanter (owner)</li>
    <li>Group members</li>
    <li>All pets (owner’s pets and group members’ pets)</li>
  </ul>

  <br><h3>Healing Logic</h3>
  <ul>
    <li><strong>Critical Healing (Below 50% HP):</strong> Prioritizes direct heal spells</li>
    <li><strong>Regular Healing (50–75% HP):</strong> Uses Heal over Time spells</li>
    <li><strong>No Healing (Above 75% HP):</strong> Will not cast healing spells</li>
  </ul>

  <br><h3>Smart Healing Features</h3>
  <ul>
    <li><strong>Spell Interruption:</strong> Will interrupt current healing spell if:
      <ul>
        <li>Direct heal being cast and target’s HP rises above 75%</li>
        <li>HoT being cast and target’s HP drops below 40% (switches to direct healing)</li>
      </ul>
    </li>
    <li><strong>Swarm Coordination:</strong> Multiple Doppelgangers will not cast the same type of healing spell on the same target simultaneously</li>
    <li><strong>Buff Stacking:</strong> Checks existing buffs to avoid overwriting or redundant casting</li>
  </ul>

  <br><h2>Combat Behavior</h2>
  <br><h3>Harmful Spell Casting</h3>
  <ul>
    <li>Casts debuffs and damage spells on the Enchanter’s current target</li>
    <li><strong>DOT Spreading:</strong> Will cast DOT spells on additional enemies that are aggressive toward the owner</li>
    <li><strong>Stackable DOTs:</strong> Multiple Doppelgangers can apply the same DOT spell to the same target</li>
    <li><strong>Non-stackable Debuffs:</strong> Only one instance per target regardless of caster</li>
  </ul>

  <br><h3>Spell Cooldown Management</h3>
  <ul>
    <li>Respects individual spell recast timers</li>
    <li>Manages global cooldown periods between spell casts</li>
    <li>Tracks cooldowns per spell to optimize casting rotation</li>
  </ul>

  <br><h2>Positioning System</h2>
  <br><h3>Swarm Coordination</h3>
  <p>When multiple Doppelgangers are active:</p>
  <ul>
    <li><strong>Equidistant Positioning:</strong> Automatically positions around the target in a circle</li>
    <li><strong>Consistent Formation:</strong> Uses sorted NPC IDs to ensure stable positioning</li>
  </ul>

  <br><h3>Movement Behavior</h3>
  <ul>
    <li>Uses advanced pathing when available</li>
    <li>Falls back to basic movement if advanced pathing is unavailable</li>
    <li>Adjusts Z-coordinate to match target height when possible</li>
  </ul>

  <br><h2>Advanced Features</h2>
  <br><h3>Multi-Target DOT Casting</h3>
  <ul>
    <li>Identifies enemies aggressive toward the owner</li>
    <li>Applies DOT spells to multiple targets beyond the primary target</li>
    <li>Optimizes damage output across multiple enemies</li>
  </ul>

  <br><h3>Spell Interruption System</h3>
  <ul>
    <li>Continuously monitors casting progress every 1 second</li>
    <li>Makes intelligent decisions about when to interrupt spells based on changing conditions</li>
    <li>Prevents wasted mana on unnecessary heals</li>
  </ul>

  <br><h3>Swarm Intelligence</h3>
  <ul>
    <li>Communicates casting intentions between Doppelganger instances</li>
    <li>Prevents duplicate beneficial spell casting</li>
    <li>Allows coordinated harmful spell application</li>
  </ul>
    <br><h2>Limitations</h2>
<br><h3>Spell Access</h3>
<ul>
  <li>Only uses spells currently memorized by the Enchanter</li>
  <li>Cannot cast spells the Enchanter doesn't have access to</li>
  <li>Respects the Enchanter's mana limitations (spell failure will occur if insufficient mana)</li>
</ul>

<br><h3>Target Restrictions</h3>
<ul>
  <li>Will not cast spells on itself (the Doppelganger NPC)</li>
  <li>Cannot heal or buff enemies</li>
  <li>Limited to line-of-sight and spell range restrictions</li>
</ul>

<br><h3>Coordination Limits</h3>
<ul>
  <li>Coordination only works between Doppelgangers of the same type and owner</li>
  <li>Cannot coordinate with other types of pets or AI entities</li>
</ul>

<br><h2>Spell Selection Process</h2>
<ul>
  <li>Gets all memorized spells from the Enchanter using <code>$owner->GetMemmedSpells()</code></li>
  <li>Separates spells by type (beneficial vs harmful)</li>
  <li>Sorts each type by priority using custom priority functions</li>
  <li>Casts the highest priority available spell that meets the current situation</li>
</ul>

<br><h3>Priority System Used</h3>

<strong>Beneficial Spells Priority:</strong>
<ol>
  <li>Heal Over Time spells (priority 1)</li>
  <li>Direct heal spells (priority 2)</li>
  <li>Rune spells (priority 3)</li>
  <li>Other beneficial spells (priority 99)</li>
</ol>

<strong>Harmful Spells Priority:</strong>
<ol>
  <li>Resistance debuffs (priority 1)</li>
  <li>Other debuffs (priority 2)</li>
  <li>Stackable DOTs (priority 3)</li>
  <li>Direct damage spells (priority 4)</li>
</ol>

<strong>Level-Based Sub-Priority:</strong>
<p>Within each category, higher level spells get slightly better priority using this formula:</p>
<pre><code>final_priority = base_priority - (spell_level / 1000)</code></pre>

<br><h3>Example Scenario</h3>
<p>If an Enchanter has these spells memorized in gems 1–8:</p>

<ul>
  <li>Gem 1: Lightning Bolt (direct damage)</li>
  <li>Gem 2: Greater Heal (direct heal)</li>
  <li>Gem 3: Charm (other)</li>
  <li>Gem 4: Regeneration (HoT)</li>
  <li>Gem 5: Slow (debuff)</li>
  <li>Gem 6: Malaise (resist debuff)</li>
  <li>Gem 7: Poison DOT (DOT)</li>
  <li>Gem 8: Rune (protective)</li>
</ul>

<p>The AI would prioritize them as:</p>

<ul>
  <li><strong>Malaise</strong> (resist debuff - priority 1)</li>
  <li><strong>Slow</strong> (debuff - priority 2)</li>
  <li><strong>Poison DOT</strong> (DOT - priority 3)</li>
  <li><strong>Lightning Bolt</strong> (direct damage - priority 4)</li>
  <li><strong>Regeneration</strong> (HoT - priority 1 for beneficial)</li>
  <li><strong>Greater Heal</strong> (direct heal - priority 2 for beneficial)</li>
  <li><strong>Rune</strong> (rune - priority 3 for beneficial)</li>
  <li><strong>Charm</strong> (other - priority 99 for beneficial)</li>
</ul>

<p>
  So spell gem position is completely ignored – the AI makes intelligent decisions based on spell type and effectiveness rather than the arbitrary order the player memorized them.
</p>

</body>