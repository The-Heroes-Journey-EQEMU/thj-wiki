---
title: Player Mechanics
description: Player Mechanics, like /shield, attack mode, pet commands, and more.
published: true
date: 2025-04-16T17:31:01.184Z
tags: 
editor: markdown
dateCreated: 2025-04-16T17:14:33.135Z
---

![gettingstartedbanner.webp](/gettingstartedbanner.webp){.align-center}

<!-- Player Mechanics Page -->
# Player Mechanics



<div class="card-container">

  <!-- Attack Mode Card -->
  <div class="card">
    <h2>Attackmode Toggle</h2>
    <p>
      The <code>#attackmode</code> command lets you choose whether your character autoattacks with ranged or melee weapons. It also updates your visual weapon display to show the appropriate equipped weapon.
    </p>
    <h3>Available Modes</h3>
    <ul>
      <li><strong>#attackmode toggle</strong>  
         Swaps between your <em>melee weapon</em> for autoattacks 
         (default mode), or your <em>bow</em>, even while in melee range.
      </li>
    </ul>
  </div>

  <!-- Autoskill Card -->
  <div class="card">
    <h2>#Autoskill System Guide</h2>
    <p>
      As per the change-log, you can make use of the <code>#autoskill</code> command to automatically use certain skill-based attacks in combat.
    </p>
    <h3>Basic Syntax</h3>
    <pre><code>#autoskill &lt;skill name&gt; enable
#autoskill &lt;skill name&gt; disable
#autoskill list
</code></pre>
    <h3>Example Usage</h3>
    <pre><code>#autoskill flying kick enable
#autoskill backstab enable
#autoskill list
</code></pre>
    <p>
      You can disable a specific autoskill like this:
    </p>
    <pre><code>#autoskill backstab disable
</code></pre>
    <h3>Supported Skills</h3>
    <ul>
      <li>Backstab</li>
      <li>Bash</li>
      <li>Tiger Claw</li>
      <li>Eagle Strike</li>
      <li>Dragon Punch / Tail Rake</li>
      <li>Flying Kick</li>
      <li>Round Kick</li>
      <li>Kick</li>
      <li>Frenzy</li>
      <li>Taunt</li>
    </ul>
    <p>
      <strong>Important Notes:</strong>  
      <em>No timer deconfliction is handled by the system. 
      If you enable multiple skills that share the same cooldown, they may interfere with each other.</em>
    </p>
  </div>

  <!-- Shield Card -->
  <div class="card">
    <h2>Using /Shield</h2>
    <p>
      Warriors of level 30 and above can serve as a living shield for another player, redirecting a portion of damage.
    </p>
    <h3>Important Mechanics</h3>
    <ul>
      <li>The effect of <code>/shield</code> lasts for 12 seconds.</li>
      <li>The shielding warrior takes 75% of the incoming damage, while the original target takes 50%.</li>
      <li>Using <code>/shield</code> can be risky if your own HP and mitigation are inadequate.</li>
    </ul>
    <h3>Strategy</h3>
    <p>
      Pairing <code>/shield</code> with a physical shield and certain "rune" effects (e.g. Enchanter spells) can significantly reduce incoming damage on the protected ally.
  </div>
</div>

