---
title: Player Mechanics
description: Player Mechanics, like /shield, attack mode, pet commands, and more.
published: true
date: 2025-04-16T17:43:28.548Z
tags: 
editor: markdown
dateCreated: 2025-04-16T17:14:33.135Z
---

![gettingstartedbanner.webp](/gettingstartedbanner.webp){.align-center}

<!-- Header Card -->
<div class="card heading-card">
  <h2 style="text-align: center;">Player Mechanics</h2>
  <p style="text-align: center;">
    <a href="/wiki/player-mechanics">Go to Player Mechanics</a> &nbsp;•&nbsp;
    <a href="/wiki/pet-mechanics">Go to Pet Mechanics</a>
  </p>
</div>

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

<!-- Pet Mechanics Page -->
<!-- Header Card -->
<div class="card heading-card">
  <h2 style="text-align: center;">Pet Mechanics</h2>
  <p style="text-align: center;">
    <a href="/wiki/player-mechanics">Go to Player Mechanics</a> &nbsp;•&nbsp;
    <a href="/wiki/pet-mechanics">Go to Pet Mechanics</a>
  </p>
</div>
<div class="card-container">

  <!-- Attack Mode Card -->
  <div class="card">
    <h2>Attack Mode Toggle</h2>
    <p>
      The <code>#attackmode</code> command lets you choose whether your character autoattacks with ranged or melee weapons. It also updates your visual weapon display to show the appropriate equipped weapon.
    </p>
    <h3>Available Modes</h3>
    <ul>
      <li><strong>#attackmode toggle</strong><br>
        Swaps between your <em>melee weapon</em> for autoattacks (default mode),
        or your <em>bow</em>, even while in melee range.
      </li>
    </ul>
  </div>

  <!-- Autoskill Card -->
  <div class="card">
    <h2>Autoskill System Guide</h2>
    <p>
      As per the change-log, you can use the <code>#autoskill</code> command to automatically use certain skill-based attacks in combat.
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
      Disable a specific autoskill:
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
      <strong>Important Note:</strong><br>
      No timer deconfliction is handled by the system. If you enable multiple
      skills that share the same cooldown or animation lock, they can interfere
      with each other.
    </p>
  </div>

  <!-- Shield Card -->
  <div class="card">
    <h2>Using Shield</h2>
    <p>
      Warriors of level 30 and above can serve as a living shield for another player,
      redirecting a portion of damage.
    </p>
    <h3>Important Mechanics</h3>
    <ul>
      <li>The effect of <code>/shield</code> lasts for 12 seconds.</li>
      <li>The shielding warrior takes 75% of the incoming damage, while the original target takes 50%.</li>
      <li>Using <code>/shield</code> can be risky if your own HP and mitigation are inadequate.</li>
    </ul>
    <h3>Strategy</h3>
    <p>
      Pairing <code>/shield</code> with a physical shield and certain "rune" effects (e.g. Enchanter spells)
      can significantly reduce incoming damage on the protected ally.
    </p>
    <h3>Sample Macro</h3>
    <pre><code>/bandolier activate NameOfWeaponSetHere
/shield
/gsay Shielding %t! Stay close!
</code></pre>
  </div>

  <!-- Pet Commands Card -->
  <div class="card">
   <h2>Multi-Pet Command System Guide</h2>
    <p>
      All these commands now work with <code>/pet</code> as well as <code>#petcmd</code>.
    </p>
   <h3>Basic Information</h3>
   <h4>What is the Multi-Pet Command System?</h4>
    <p>
      This system allows players to control their pets individually or in groups, with
      advanced targeting options based on class.
    </p>
   <h4>How do I control my pets?</h4>
    <p>
      You can use text commands to issue orders to your pets. Commands can be directed
      to individual pets, all pets, or pets belonging to specific classes.
    </p>
    <p>
      For instance, <code>/pet health</code> and <code>#petcmd health</code> let you view
      your pet’s health. 
    </p>
   <h3>Class-Based Targeting</h3>
    <p>
      You can target pets based on their class. Direct commands to all pets, or only certain classes.
    </p>
   <h4>Class-Based Targeting Examples</h4>
    <ul>
      <li><code>#petcmd all attack</code> → All pets will attack</li>
      <li><code>#petcmd necro follow</code> → Only Necromancer pets will follow</li>
      <li><code>#petcmd magician hold</code> → Only Magician pets will enter hold mode</li>
    </ul>
    <h4>Available Class Targets</h4>
    <table>
      <thead>
        <tr>
          <th>Class Name</th>
          <th>Command Target</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>All Pets</td><td>all</td></tr>
        <tr><td>Magician</td><td>magician</td></tr>
        <tr><td>Beastlord</td><td>beastlord</td></tr>
        <tr><td>Necromancer</td><td>necromancer</td></tr>
        <tr><td>Enchanter</td><td>enchanter</td></tr>
        <tr><td>Shaman</td><td>shaman</td></tr>
        <tr><td>Druid</td><td>druid</td></tr>
        <tr><td>Bard</td><td>bard</td></tr>
        <tr><td>Shadow Knight</td><td>shadowknight</td></tr>
        <tr><td>Warrior</td><td>warrior</td></tr>
        <tr><td>Cleric</td><td>cleric</td></tr>
        <tr><td>Paladin</td><td>paladin</td></tr>
        <tr><td>Ranger</td><td>ranger</td></tr>
        <tr><td>Monk</td><td>monk</td></tr>
        <tr><td>Rogue</td><td>rogue</td></tr>
        <tr><td>Wizard</td><td>wizard</td></tr>
        <tr><td>Berserker</td><td>berserker</td></tr>
      </tbody>
    </table>
    <p>
      You can even chain commands to send different orders to different classes.
    </p>
    <pre><code>#petcmd necromancer attack
#petcmd magician hold
</code></pre>
   <h3>Advanced Multi-Pet Command Usage</h3>
   <h4>Scenario 1: Coordinated Multi-Pet Combat</h4>
    <p>
      You have a Magician, Necromancer, and Beastlord, each with their own pets. You want:
    </p>
    <ul>
      <li>Necromancer pet to attack and tank</li>
      <li>Magician pet to hold and not engage</li>
      <li>Beastlord pet to assist but return when low HP</li>
    </ul>
    <pre><code>#petcmd necromancer attack
#petcmd magician hold
#petcmd beastlord attack
#petcmd beastlord health
</code></pre>
   <h4>Scenario 2: Defensive Positioning and Pet Guarding</h4>
    <ul>
      <li>Magician and Necromancer pets guard the entrance</li>
      <li>Beastlord pet follows you</li>
    </ul>
    <pre><code>#petcmd magician guard
#petcmd necromancer guard
#petcmd beastlord follow
</code></pre>
   <h4>Scenario 3: Emergency Retreat and Regrouping</h4>
    <pre><code>#petcmd all back
#petcmd all regroup
#petcmd all hold
</code></pre>
   <h4>Scenario 4: Selective Combat Engagement</h4>
    <ul>
      <li>Magician &amp; Necromancer pets attack one enemy</li>
      <li>Beastlord pet attacks a different enemy</li>
      <li>All pets stop casting spells (spellhold)</li>
    </ul>
    <pre><code>#petcmd magician attack
#petcmd necromancer attack
#petcmd beastlord attack
#petcmd all spellhold
</code></pre>
   <h3>Macro Examples</h3>
    <p>
      Below are some specific macro commands for controlling multiple pets in various combat situations.
    </p>
   <h4>Macro 1</h4>
    <pre><code>#petcmd back hold on
</code></pre>
    <p>
      A “back off” command that instructs all pets to cease attacking, clear their queue,
      and return to you. Particularly useful if you need to pull pets off a target to prepare for a new one.
    </p>
   <h4>Macro 2</h4>
    <pre><code>/pause 2, /assist nabuser
#petcmd attack
</code></pre>
    <p>
      This macro targets whatever your Mage pet is focused on and instructs other pets to engage that
      same target. You’ll need to replace <code>nabuser</code> with your Mage pet’s name.
    </p>
   <h4>Macro 3</h4>
    <pre><code>#petcmd nec enc attack
</code></pre>
    <p>
      This adds targets only to your DPS pets (e.g. Necromancer and Enchanter) while leaving the Mage pet’s
      attack queue alone. Useful to control where DPS pets focus without disrupting your main pet’s target.
    </p>
   <h4>Macro 4</h4>
    <pre><code>#petcmd nec enc back
#petcmd nec enc attack
</code></pre>
    <p>
      Instructs Enchanter and Necromancer pets to clear their current targets
      and re-engage a newly selected enemy. Lets the Mage pet maintain aggro on
      the boss without them interfering.
    </p>
   <h4>Macro 5</h4>
    <pre><code>#petcmd enc nec taunt off focus on hold on
#petcmd mag taunt on focus on hold on
</code></pre>
    <p>
      This macro line disables Taunt for Enchanter/Necromancer pets while enabling Focus
      and Hold. The second line enables Taunt, Focus, and Hold for the Magician pet,
      helping maintain controlled aggression in multi-pet fights.
    </p>
  </div><!-- end Pet Commands Card -->
</div><!-- end card-container -->