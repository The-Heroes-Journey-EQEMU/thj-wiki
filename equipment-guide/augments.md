---
title: Augments
description: A filterable augment list for THJ
published: true
date: 2025-03-31T02:58:59.562Z
tags: 
editor: markdown
dateCreated: 2025-03-22T05:37:35.756Z
---

<div class="header">
  <img src="/equipment-guide/augment_banner.webp" alt="Augments Catalog" class="augment-banner" />
  <p>Search by Name, Stat, or Resist</p>
  <div class="filter-row">
    <input type="text" id="search-box" placeholder="Search name..." />
    <select id="stat-filter">
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
    <select id="resist-filter">
      <option value="">Filter by Resist</option>
      <option value="magicResist">Magic</option>
      <option value="fireResist">Fire</option>
      <option value="coldResist">Cold</option>
      <option value="diseaseResist">Disease</option>
      <option value="poisonResist">Poison</option>
      <option value="corruptionResist">Corruption</option>
    </select>
<select id="zone-filter">
  <option value="">Filter by Zone</option>
  <option value="Sanctus Seru">Sanctus Seru</option>
  <option value="Veeshan's Peak">Veeshan's Peak</option>
  <option value="Plane of Time">Plane of Time</option>
</select>
    <select id="rarity-filter">
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
