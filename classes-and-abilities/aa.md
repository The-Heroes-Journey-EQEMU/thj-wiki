---
title: AA
description: AA Breakdown
published: true
date: 2025-07-05T15:52:04.921Z
tags: 
editor: markdown
dateCreated: 2025-03-02T07:32:20.006Z
---

![aa_builder.webp](/classes-and-abilities/aa_builder.webp){.aa-builder-banner}

<div id="aa-builder">
  <h1 class="aa-title">The Heroes Journey AA Ability Builder</h1>

  <div class="aa-subtext">
    <p>Select up to <strong>3 classes</strong> to view their abilities.</p>
    <p>Select <strong>General, Archetype, or Class</strong> to see abilities associated with the highlighted classes.</p>
  </div>

  <div class="filter-options">
    <button class="mode-button active" data-mode="general">General</button>
    <button class="mode-button" data-mode="archetype">Archetype</button>
    <button class="mode-button" data-mode="class">Class</button>
  </div>

  <div class="class-buttons" id="classButtons"></div>

  <div class="search-container">
    <input type="text" id="searchInput" placeholder="Search abilities…" class="search-input">
  </div>

  <div class="stats" id="stats">Loading abilities…</div>

  <div id="abilitiesContainer" class="cards"></div>
</div>
