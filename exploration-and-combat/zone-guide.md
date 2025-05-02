---
title: Zone Guide
description: A Zone Guide and Pathfinder for THJ, or just EverQuest
published: true
date: 2025-05-02T20:51:21.241Z
tags: 
editor: markdown
dateCreated: 2025-03-03T17:27:36.001Z
---

<div class="container">
  <h1>Search For Zone Links</h1>

  <!-- help text -->
  <p class="finder-explainer">
    Pick your <strong>From</strong> and <strong>To</strong> zones below.<br>
    The tool auto-completes names and finds the shortest route.
    <em>Tip&nbsp;►</em> Tick <strong>Allow Bazaar Portal</strong> to include the Bazaar teleporter in paths.
  </p>
  <form action="" id="searchForm">
    <div class="checkbox-group">
      <input type="checkbox" id="isBazaarPortalAllowed" name="isBazaarPortalAllowed" checked>
      <label for="isBazaarPortalAllowed">Allow Bazaar Portal</label>
    </div>
    From: <input list="zones" name="from" id="from" placeholder="Origin zone">
    To:   <input list="zones" name="to"   id="to"   placeholder="Destination zone">
    <datalist id="zones"></datalist>
    <button type="submit">Submit</button>
  </form>
  <div id="results"></div>
</div>
<h2 id="world-map">Interactive World Map</h2>
<div class="map-wrapper">
  <img id="thjZoneMap" src="/map/thj-waypoints.png" alt="THJ Zone Map">
</div>
