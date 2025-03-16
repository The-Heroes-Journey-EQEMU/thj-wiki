---
title: AA
description: AA Breakdown
published: true
date: 2025-03-16T21:34:10.832Z
tags: 
editor: markdown
dateCreated: 2025-03-02T07:32:20.006Z
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Heroes Journey AA Ability Tracker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>The Heroes Journey AA Ability Tracker</h1>
        <h3>Select up to 3 classes to view their abilities.</h3>
        <p>Selecting <strong>"Class Selection"</strong> shows you the abilities for the classes you selected.</p>
        <p><strong>Click the # after Spell ID</strong> to visit the Spell page for that ability on thjdi.cc.</p>
    </header>
    <div class="controls">
        <div class="filter-options">
            <button class="mode-button active" data-mode="all">All Abilities</button>
            <button class="mode-button" data-mode="selection">Class Selection</button>
            <button class="mode-button" data-mode="none">No Abilities</button>
        </div>
        <div class="class-buttons" id="classButtons">
            <!-- Class buttons will be added here by JavaScript -->
        </div>
    </div>
    <div class="stats" id="stats">
        Showing all abilities (0)
    </div>
    <div class="abilities-container" id="abilitiesContainer">
        <!-- Abilities will be added here by JavaScript -->
    </div>
    <script src="script.js"></script>
</body>
</html>
