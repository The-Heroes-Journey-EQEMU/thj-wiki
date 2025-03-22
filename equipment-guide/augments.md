---
title: Augments
description: A filterable augment list for THJ
published: true
date: 2025-03-22T15:29:28.775Z
tags: 
editor: markdown
dateCreated: 2025-03-22T05:37:35.756Z
---

<div class="container">
        <h1>EverQuest Augment Browser</h1>
        <div class="controls">
            <div class="control-group">
                <label for="searchInput">Search:</label>
                <input type="text" id="searchInput" placeholder="Search augments...">
            </div>
            <div class="control-group">
                <label for="statFilter">Filter by Stat:</label>
                <select id="statFilter">
                    <option value="">All Stats</option>
                    <option value="Strength">Strength</option>
                    <option value="Stamina">Stamina</option>
                    <option value="Agility">Agility</option>
                    <option value="Dexterity">Dexterity</option>
                    <option value="Intelligence">Intelligence</option>
                    <option value="Wisdom">Wisdom</option>
                    <option value="Charisma">Charisma</option>
                    <option value="HP">HP</option>
                    <option value="Mana">Mana</option>
                    <option value="Endurance">Endurance</option>
                </select>
            </div>
            <div class="control-group">
                <label for="resistFilter">Filter by Resist:</label>
                <select id="resistFilter">
                    <option value="">All Resists</option>
                    <option value="Magic Resist">Magic</option>
                    <option value="Fire Resist">Fire</option>
                    <option value="Cold Resist">Cold</option>
                    <option value="Disease Resist">Disease</option>
                    <option value="Poison Resist">Poison</option>
                </select>
            </div>
            <div class="control-group">
                <label for="sortBy">Sort By:</label>
                <select id="sortBy">
                    <option value="name">Name</option>
                    <option value="hp">HP</option>
                    <option value="mana">Mana</option>
                    <option value="endurance">Endurance</option>
                </select>
            </div>
            <div class="control-group">
                <label>&nbsp;</label>
                <button id="toggleAllBtn" class="toggle-btn">Expand All</button>
            </div>
        </div>
        <div class="aug-grid" id="augmentGrid">
            <!-- Augment cards will be inserted here by JavaScript -->
        </div>
    </div>