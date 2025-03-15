---
title: AA
description: AA Breakdown
published: true
date: 2025-03-15T03:16:22.421Z
tags: 
editor: markdown
dateCreated: 2025-03-02T07:32:20.006Z
---

<h1>EverQuest Abilities Database</h1>
<p>Select your class(es) below to view relevant abilities.</p>

<div id="class-selection">
    <h2>Select Classes</h2>
    <div id="class-checkboxes" class="checkbox-container">
        <!-- Checkboxes will be dynamically added here -->
        <div class="loading">Loading classes...</div>
    </div>
    <button id="show-abilities-btn" class="action-button">Show Abilities</button>
</div>

<div id="abilities-display">
    <h2>Abilities</h2>
    <div id="filter-options">
        <input type="text" id="search-input" placeholder="Search abilities...">
        <select id="category-filter">
            <option value="ALL">All Categories</option>
        </select>
        <button id="clear-filters-btn" class="action-button">Clear Filters</button>
    </div>
    <div id="abilities-container">
        <p class="loading">Select classes and click "Show Abilities" to view abilities data.</p>
    </div>
</div>