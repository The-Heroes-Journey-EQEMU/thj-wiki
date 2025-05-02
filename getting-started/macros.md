---
title: Macros
description: 
published: true
date: 2025-05-02T14:09:46.251Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:27:56.853Z
---

<div class="banner-container">
    <img src="/gettingstartedbanner.webp" alt="Getting Started Banner" class="banner-image">
</div>

<!-- Macros Guide -->
<section class="intro-section" id="macros">
<!-- Table of Contents -->
<div class="jump-buttons">
  <a href="#macros" class="jump-button">Macros</a>
  <a href="#how-to-macro" class="jump-button">How To Macro</a>
</div>
    <h1>Macros</h1>
    <p>
        These macros can be quickly copy-pasted in-game by setting the <strong>Paste From Clipboard</strong> hotkey:
        <ul>
            <li>Press <strong>ALT+O</strong>, select <strong>Keys</strong> → <strong>UI</strong>, and set <em>Paste From Clipboard</em> to <strong>CTRL+V</strong>.</li>
        </ul>
    </p>
</section>
<div class="jump-buttons">
  <a href="#one" class="jump-button">Sell Items</a>
  <a href="#two" class="jump-button">Auto Bank</a>
  <a href="#three" class="jump-button">Tradeskill Combines</a>
  <a href="#four" class="jump-button">Destroy Item on Cursor</a>
  <a href="#five" class="jump-button">Loot Corpse</a>
  <a href="#six" class="jump-button">Mass Item Turn-In</a>
  <a href="#seven" class="jump-button">Accept from Parcel</a>
  <a href="#eight" class="jump-button">Convert Currency</a>
  <a href="#nine" class="jump-button">Donate to Tribute Merchant</a>
  <a href="#ten" class="jump-button">Set Trader Prices</a>
</div>
<!-- Sell Item to Merchant -->
<section class="content-section">
    <h2 id="one">Sell Item To Merchant</h2>
    <p class="section-description">Useful for quickly selling multiple items.</p>
    <div class="macro">/notify MerchantWND MW_Sell_Button leftmouseup</div>
    <div class="macro">/notify QuantityWnd QTYW_Accept_Button leftmouseup</div>
</section>
<!-- Auto Bank -->
<section class="content-section">
    <h2 id="two">Auto Bank</h2>
    <div class="macro">/hotbutton Autobank /notify BigBankWnd AutoButton leftmouseup</div>
</section>

<!-- Tradeskill Combines -->
<section class="content-section">
    <h2 id="three">Tradeskill Combines</h2>
    <div class="macro">/notify TradeskillWnd CombineButton leftmouseup</div>
    <div class="macro">/pause 1, /autoinv</div>
</section>

<!-- Destroy Item On Cursor -->
<section class="content-section">
    <h2 id="four">Destroy Item On Cursor</h2>
    <div class="macro">/notify IW_InvPage IW_Destroy leftmouseup</div>
    <div class="macro">/notify ConfirmationDialogBox CD_Yes_Button leftmouseup</div>
</section>

<!-- Loot Corpse -->
<section class="content-section">
    <h2 id="five">Loot Corpse</h2>
    <p>Disable Loot All Confirmation: ALT+O → General settings.</p>
    <div class="macro">/loot</div>
    <div class="macro">/notify LootWnd LW_LootAllButton leftmouseup</div>
    <div class="macro">/notify ConfirmationDialogBox CD_Yes_Button leftmouseup</div>
</section>

<!-- Mass Item Turn-in -->
<section class="content-section">
    <h2 id="six">Mass Item Turn-in</h2>
    <p>Rebind "Use centerscreen" to <strong>CTRL+Z</strong>.</p>
    <div class="macro">/itemnotify in pack1 1 leftmouseup</div>
    <div class="macro">/notify GiveWnd GVW_Give_Button leftmouseup</div>
</section>

<!-- Accept Items From Parcel -->
<section class="content-section">
    <h2 id="seven">Accept Items From Parcel</h2>
    <div class="macro">/notify MerchantWnd MW_MerchantSubwindows tabselect 2</div>
    <div class="macro">/notify MerchantWnd MW_ItemlistMail listselect 1</div>
    <div class="macro">/notify MerchantWnd MW_Retrieve_Button leftmouseup</div>
</section>

<!--Currency Conversion -->
<section class="content-section">
    <h2 id="eight">Currency Conversion Macros</h2>
  	<h2>Convert Copper to Silver</h2>
    <div class="macro">/notify InventoryWnd IW_Money3 leftmouseup</div>
    <div class="macro">/notify QuantityWnd QTYW_Accept_Button leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money2 leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money3 leftmouseup</div>
    <h2>Convert Silver to Gold</h2>
    <div class="macro">/notify InventoryWnd IW_Money2 leftmouseup</div>
    <div class="macro">/notify QuantityWnd QTYW_Accept_Button leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money1 leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money2 leftmouseup</div>
    <h2>Convert Gold to Platinum</h2>
    <div class="macro">/notify InventoryWnd IW_Money1 leftmouseup</div>
    <div class="macro">/notify QuantityWnd QTYW_Accept_Button leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money0 leftmouseup</div>
    <div class="macro">/notify InventoryWnd IW_Money1 leftmouseup</div>
</section>

<!-- Donate to Tribute Merchant -->
<section class="content-section">
    <h2 id="nine">Donate to Tribute Merchant</h2>
    <div class="macro">/notify TributeMasterWnd TMW_DonateButton leftmouseup</div>
</section>

<!-- Set Trader Prices -->
<section class="content-section">
    <h2 id="ten">Set Trader Prices</h2>
    <p>Hotkey "Set" to 1 and "Save" to 2 for efficient pricing.</p>
    <div class="macro">/hotbutton Set /notify BazaarWnd BZW_Clear_Button leftmouseup</div>
    <div class="macro">/notify BazaarWnd BZW_Money0 leftmouseup</div>
    <div class="macro">/notify BazaarWnd BZW_SetPrice_Button leftmouseup</div>
</section>

![pagebreak4.webp](/pagebreak4.webp){.align-center}

<!-- How to Macro -->
<section class="content-section">
<!-- Table of Contents -->
<div class="jump-buttons">
  <a href="#macros" class="jump-button">Macros</a>
  <a href="#how-to-macro" class="jump-button">How To Macro</a>
</div>
    <h2 id="how-to-macro">How to Macro</h2><br>
    <p>
        Macros, also called <strong>Socials</strong>, are small scripts within the game that execute up to five commands with a single click or keypress.
    </p>
    <p>
        To view or edit your macros, open the <strong>Actions Window</strong> (visible by default) and click the <strong>"Socials Page"</strong> tab. Each button represents a macro, executed by left-clicking and edited by right-clicking. By default, the first page contains 12 macros with various simple commands. Right-click a macro button to open the editing window:
    </p><br>
    <div class="image-container">
        <img src="/macros/macros-edit1.png" alt="Macro Editing Window Example" class="section-image">
    </div>
    <br><p>
        The text box in the top left sets the macro’s name, while the buttons on the right choose a color to display the macro's name.
    </p>
    <p>
        The bottom five lines contain the macro’s commands. Each line accepts one slash command. For example, a simple macro might look like:
    </p><br>
    <div class="image-container">
        <img src="/macros/macros-dance.png" alt="Macro Editing Window Example" class="section-image">
    </div>
    <br><p>
        Clicking this macro would cause your character to <strong>/dance</strong>, then say <em>"I'm dancing!"</em>. Plenty of example commands are below so you can make your own macros!
    </p>
</section>


<!-- Cast Spell -->
<section class="content-section">
    <h2>/cast</h2>
    <p class="section-description">Casts a spell from your spell slots (1-12).</p>
    <div class="macro">/cast 7 - Casts the spell in your spell slot #7.</div>
</section>

<!-- Do Ability -->
<section class="content-section">
    <h2>/doability</h2>
    <p class="section-description">Performs an ability from the Abilities (1-6) or Combat Page (7-10).</p>
    <div class="macro">/doability 1 - Uses the ability in your first "Abilities" slot.</div>
</section>

<!-- Pause -->
<section class="content-section">
    <h2>/pause</h2>
    <p class="section-description">Pauses macro execution briefly. See earlier macro examples for usage.</p>
</section>

<!-- Activate AA -->
<section class="content-section">
    <h2>/alt activate</h2>
    <p class="section-description">Activates an Alternate Advancement (AA) ability.</p>
    <div class="macro">/alt activate 47 - Activates the Shaman AA Cannibalization.</div>
</section>

<!-- Target -->
<section class="content-section">
    <h2>/target</h2>
    <p class="section-description">Targets a nearby player, NPC, or corpse.</p>
    <div class="macro">/target Zliz - Targets the player or NPC "Zliz".</div>
    <div class="macro">/target orc_pawn - Targets NPC named "orc pawn".</div>
</section>

<!-- Invite -->
<section class="content-section">
    <h2>/invite</h2>
    <p class="section-description">Invites a player to your group.</p>
    <div class="macro">/invite - Invites your current target to join your group.</div>
    <div class="macro">/invite Zliz - Invites player Zliz to your group.</div>
</section>

<!-- Follow -->
<section class="content-section">
    <h2>/follow</h2>
    <p class="section-description">Automatically follows another player.</p>
    <div class="macro">/follow - Begins auto-following your current target.</div>
</section>

<!-- Assist -->
<section class="content-section">
    <h2>/assist</h2>
    <p class="section-description">Targets the target of your target.</p>
    <div class="macro">/assist - Assists your current target.</div>
    <div class="macro">/assist Zliz - Assists player Zliz.</div>
</section>

<!-- Timer -->
<section class="content-section">
    <h2>/timer</h2>
    <p class="section-description">Sets a macro button cooldown.</p>
    <div class="macro">/timer 100 - Sets a 10-second cooldown timer on the macro button.</div>
</section>

<!-- Discipline -->
<section class="content-section">
    <h2>/discipline</h2>
    <p class="section-description">Activates a discipline.</p>
    <div class="macro">/discipline Diamondpalm Discipline Rk. II - Activates Monk discipline.</div>
</section>

<!-- Bandolier -->
<section class="content-section">
    <h2>/bandolier</h2>
    <p class="section-description">Switches weapon sets from your bandolier.</p>
    <div class="macro">/bandolier 2HB - Equips your saved "2HB" bandolier set.</div>
</section>

<!-- Auto Inventory -->
<section class="content-section">
    <h2>/autoinventory</h2>
    <p class="section-description">Moves items from cursor to inventory automatically.</p>
    <div class="macro">/autoinventory</div>
</section>

<!-- Pet Attack -->
<section class="content-section">
    <h2>/pet attack</h2>
    <p class="section-description">Commands your pet to attack a target.</p>
    <div class="macro">/pet attack - Pet attacks your current target.</div>
    <div class="macro">/pet attack a_skeleton - Pet attacks nearby NPC named "a skeleton".</div>
</section>

![pagebreak5.webp](/pagebreak5.webp){.align-center}