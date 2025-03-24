---
title: Augments
description: A filterable augment list for THJ
published: true
date: 2025-03-24T00:27:05.307Z
tags: 
editor: markdown
dateCreated: 2025-03-22T05:37:35.756Z
---

<div class="header">
  <h1>Augments Catalog</h1>
  <p>Search by name, stat, or resist</p>
  <div class="filter-row">
    <input type="text" id="search-box" placeholder="Search name..." />
    <select id="stat-filter">
      <option value="">Filter by stat</option>
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
      <option value="">Filter by resist</option>
      <option value="magicResist">Magic</option>
      <option value="fireResist">Fire</option>
      <option value="coldResist">Cold</option>
      <option value="diseaseResist">Disease</option>
      <option value="poisonResist">Poison</option>
      <option value="corruptionResist">Corruption</option>
    </select>
  </div>
</div>
<div class="container">
  <div id="augments-container"></div>
</div>
