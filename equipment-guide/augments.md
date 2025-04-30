---
title: Augments
description: A filterable augment list for THJ
published: true
date: 2025-04-30T22:11:45.591Z
tags: 
editor: markdown
dateCreated: 2025-03-22T05:37:35.756Z
---

<div class="header">
  <img src="/equipment-guide/augment_banner.webp" alt="Augments Catalog" class="augment-banner" />
  <p>Search by Name, Stat, Resist, or Zone</p>
<div class="filter-row">
  <input type="text" id="search-box" placeholder="Search name..." />

  <select id="stat-filter" class="filter-button">
    <option value="">Filter by Stat</option>
    <option value="strength">Strength</option>
    <option value="stamina">Stamina</option>
    <option value="agility">Agility</option>
    <option value="dexterity">Dexterity</option>
    <option value="intelligence">Intelligence</option>
    <option value="wisdom">Wisdom</option>
    <option value="charisma">Charisma</option>
    <option value="ac">AC</option>
    <option value="hp">HP</option>
    <option value="mana">Mana</option>
    <option value="endurance">Endurance</option>
  </select>

  <select id="resist-filter" class="filter-button">
    <option value="">Filter by Resist</option>
    <option value="magicResist">Magic</option>
    <option value="fireResist">Fire</option>
    <option value="coldResist">Cold</option>
    <option value="diseaseResist">Disease</option>
    <option value="poisonResist">Poison</option>
    <option value="corruptionResist">Corruption</option>
  </select>

  <select id="zone-filter" class="filter-button">
    <option value="">Filter by Zone</option>
    <option value="Bazaar">Bazaar</option>
    <option value="Gunthak">Gunthak</option>
    <option value="Howling Stones">Howling Stones</option>
    <option value="Kaesora">Kaesora</option>
    <option value="Lavastorm">Lavastorm</option>
    <option value="Lower Guk">Lower Guk</option>
    <option value="Nadox">Nadox</option>
    <option value="Plane of Time">Plane of Time</option>
    <option value="Sanctus Seru">Sanctus Seru</option>
    <option value="Skyfire Mountains">Skyfire Mountains</option>
    <option value="SolA">SolA</option>
    <option value="Ssra Temple">Ssra Temple</option>
    <option value="Upper Guk">Upper Guk</option>
    <option value="Veeshan's Peak">Veeshan's Peak</option>
  </select>

  <select id="rarity-filter" class="filter-button">
    <option value="">Filter by Rarity</option>
    <option value="normal">Normal</option>
    <option value="enchanted">Enchanted</option>
    <option value="legendary">Legendary</option>
  </select>
</div>

</div>
<div class="container">
  <div id="augments-container" class="augments-grid"></div>
</div>
