---
title: Zone Guide
description: A Zone Guide and Pathfinder for THJ, or just EverQuest
published: true
date: 2025-05-02T21:12:15.047Z
tags: 
editor: markdown
dateCreated: 2025-03-03T17:27:36.001Z
---

![zone_guide_map_banner.png](/map/zone_guide_map_banner.png)
<div class="container">
  <h1>Search For Zone Links</h1>
  <p class="finder-explainer">
    Pick your <strong>From</strong> and <strong>To</strong> zones below.<br>
    The tool auto-completes names and finds the shortest route.
    <em>Tip ►</em> Tick <strong>Allow Bazaar Portal</strong> to include the Bazaar teleporter in paths. Gold is 'on'.
  </p>
  <form action="" id="searchForm">
    <div class="checkbox-group">
      <input type="checkbox" id="isBazaarPortalAllowed" name="isBazaarPortalAllowed" checked>
      <label for="isBazaarPortalAllowed">Allow Bazaar Portal</label>
    </div>
    From:
    <input list="zones" name="from" id="from" placeholder="Origin zone">
    To:
    <input list="zones" name="to" id="to" placeholder="Destination zone">
    <datalist id="zones"></datalist>
    <button type="submit">Submit</button>
  </form>
  <div id="results"></div>
</div>
<h2 id="world-map">Interactive World Map</h2>
<p class="map-tip">Click + drag to pan — scroll to zoom (double-click resets).</p>
<h3>By <a href="https://github.com/perotan/thj-waypoints/blob/ad0b7a52305ae81fb4fa319a0d0259a446ee0fa0/thj-waypoints.png" target="_blank" rel="noopener">Perotan</a></h3>
<div class="map-wrapper">
  <img id="thjZoneMap" src="/map/thj-waypoints.png" alt="THJ Zone Map">
</div>
