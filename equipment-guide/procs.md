---
title: Proc Weapons
description: Quick Reference list of Proc Weapons in The Heroes' Journey
published: true
date: 2025-03-20T01:07:56.219Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:33:24.343Z
---

<!-- "Proc Weapons by Class" Page -->
<div class="proc-weapons-page">
  <!-- Hero / Header area -->
  <div class="proc-hero">
    <h2>Proc Weapons by Class</h2>
    <p>
      This page lists various equippable weapons that feature special “proc” effects,  
      along with the classes that can use them on The Heroes Journey EQEmu server.
    </p>
    <p>
      You can filter by class and/or search for a specific weapon, zone, or effect.
    </p>
    <div class="filter-container">
      <label><input type="checkbox" value="ALL" class="filter-checkbox" checked> ALL</label>
      <label><input type="checkbox" value="BER" class="filter-checkbox"> BER</label>
      <label><input type="checkbox" value="BRD" class="filter-checkbox"> BRD</label>
      <label><input type="checkbox" value="BST" class="filter-checkbox"> BST</label>
      <label><input type="checkbox" value="CLR" class="filter-checkbox"> CLR</label>
      <label><input type="checkbox" value="DRU" class="filter-checkbox"> DRU</label>
      <label><input type="checkbox" value="ENC" class="filter-checkbox"> ENC</label>
      <label><input type="checkbox" value="MAG" class="filter-checkbox"> MAG</label>
      <label><input type="checkbox" value="MNK" class="filter-checkbox"> MNK</label>
      <label><input type="checkbox" value="NEC" class="filter-checkbox"> NEC</label>
      <label><input type="checkbox" value="PAL" class="filter-checkbox"> PAL</label>
      <label><input type="checkbox" value="ROG" class="filter-checkbox"> ROG</label>
      <label><input type="checkbox" value="RNG" class="filter-checkbox"> RNG</label>
      <label><input type="checkbox" value="SHD" class="filter-checkbox"> SHD</label>
      <label><input type="checkbox" value="SHM" class="filter-checkbox"> SHM</label>
      <label><input type="checkbox" value="WAR" class="filter-checkbox"> WAR</label>
      <label><input type="checkbox" value="WIZ" class="filter-checkbox"> WIZ</label>
    </div>
    <!-- Search bar -->
    <input type="text" id="searchInput" placeholder="Search by weapon name, zone, or proc effect..." />
  </div>
  <!-- Container where JS will dynamically append proc-weapon cards -->
  <div id="procWeaponsContainer"></div>
</div>
