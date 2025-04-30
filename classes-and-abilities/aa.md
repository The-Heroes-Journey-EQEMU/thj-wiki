---
title: AA
description: AA Breakdown
published: true
date: 2025-04-30T23:32:00.152Z
tags: 
editor: markdown
dateCreated: 2025-03-02T07:32:20.006Z
---

![aa_builder.webp](/classes-and-abilities/aa_builder.webp){.align-center}

<div id="aa-builder">
  <h1>The Heroes Journey AA Ability Builder</h1>
  <div class="center-text">
    Select up to <strong>3 classes</strong> to view their abilities.<br>
    Select <strong>General, Archetype, or Class</strong> to see abilities associated with the highlighted classes, in the appropriate category.
  </div>
  
  <div class="filter-options">
    <button class="mode-button active" data-mode="general">General</button>
    <button class="mode-button" data-mode="archetype">Archetype</button>
    <button class="mode-button" data-mode="class">Class</button>
  </div>
  
  <div class="class-buttons" id="classButtons">
    <!-- Classes will be populated via JS -->
  </div>
  
  <div class="search-container">
    <input type="text" id="searchInput" placeholder="Search abilities..." class="search-input">
  </div>
  
  <div class="stats" id="stats">
    Loading abilities...
  </div>
  
  <div class="abilities-container" id="abilitiesContainer">
    <!-- Abilities will be populated via JS -->
  </div>
</div>