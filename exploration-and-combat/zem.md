---
title: ZEM
description: ZEM
published: true
date: 2025-04-30T16:37:54.239Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:27:21.918Z
---

<!-- New info section -->
<div class="zem-explanation">
  <h2>Zone Experience Modifiers (ZEM) Overview</h2>
  <p>If all were equal, killing two mobs of the same level in different zones would give the same amount of XP. 
     However, in EverQuest (EQ) some zones grant more (or less) experience than others for mobs of the same level. 
     These multipliers are known as ZEMs.</p>

  <p>
    Originally, the EQ developers introduced ZEMs to reward players for tackling riskier or more complex zones. 
    Dungeons often receive higher ZEMs, while outdoor zones typically have lower ones. 
    <br><br>On <strong>The Heroes Journey</strong>, we share these values so you can plan your leveling path accordingly.
  </p>
</div>

<!-- Existing hero + zone layout -->
<div class="zones-page">
  <div class="zones-hero">
    <h2>Zone Experience Modifiers (ZEM)</h2>
    <p>Search by zone name or short name below to see the ZEM, or peruse the list below:</p>
    <br>
    <input type="text" id="zonesSearchInput" placeholder="Type to filter zones..." />
  </div>
  <div id="zonesContainer"></div>
</div>

<script>
// Zone data extracted from WikiPage.md
const zones = [
  { id: 291, long_name: "The Plane of Time", short_name: "potimea", zem: 3.00 },
  { id: 292, long_name: "The Plane of Time", short_name: "potimeb", zem: 3.00 },
  { id: 297, long_name: "The Plane of Water", short_name: "powater", zem: 3.00 },
  { id: 27, long_name: "Bastion of Thunder", short_name: "bothunder", zem: 2.75 },
  { id: 426, long_name: "Vex Thal", short_name: "vexthal", zem: 2.75 },
  { id: 281, long_name: "The Plane of Disease", short_name: "podisease", zem: 2.50 },
  { id: 286, long_name: "The Plane of Justice", short_name: "pojustice", zem: 2.50 },
  { id: 288, long_name: "The Plane of Nightmares", short_name: "ponightmare", zem: 2.50 },
  { id: 289, long_name: "The Plane of Storms", short_name: "postorms", zem: 2.50 },
  { id: 290, long_name: "Drunder, the Fortress of Zek", short_name: "potactics", zem: 2.50 },
  { id: 293, long_name: "Torment, the Plane of Pain", short_name: "potorment", zem: 2.50 },
  { id: 295, long_name: "The Plane of Valor", short_name: "povalor", zem: 2.50 },
  { id: 43, long_name: "The Howling Stones", short_name: "charasis", zem: 2.50 },
  { id: 355, long_name: "The Caverns of Exile", short_name: "soldungc", zem: 2.50 },
  { id: 356, long_name: "The Tower of Solusek Ro", short_name: "solrotower", zem: 2.50 },
  { id: 113, long_name: "The Plane of Fear", short_name: "fearplane", zem: 2.50 },
  { id: 388, long_name: "The Temple of Veeshan", short_name: "templeveeshan", zem: 2.50 },
  { id: 143, long_name: "The Plane of Growth", short_name: "growthplane", zem: 2.50 },
  { id: 170, long_name: "The Halls of Honor", short_name: "hohonora", zem: 2.50 },
  { id: 171, long_name: "The Temple of Marr", short_name: "hohonorb", zem: 2.50 },
  { id: 193, long_name: "Kedge Keep", short_name: "kedge", zem: 2.50 },
  { id: 254, long_name: "The Lair of Terris Thule", short_name: "nightmareb", zem: 2.50 },
  // ... (add all other rows as needed) ...
];

function renderZonesTable(zonesToShow) {
  const table = document.createElement('table');
  table.className = 'zem-table';
  table.innerHTML = `
    <thead>
      <tr>
        <th>Zone Name</th>
        <th>Short Name</th>
        <th>ZEM</th>
      </tr>
    </thead>
    <tbody>
      ${zonesToShow.map(z => `
        <tr>
          <td>${z.long_name}</td>
          <td>${z.short_name}</td>
          <td>${z.zem.toFixed(2)}</td>
        </tr>
      `).join('')}
    </tbody>
  `;
  const container = document.getElementById('zonesContainer');
  container.innerHTML = '';
  container.appendChild(table);
}

function filterZones() {
  const input = document.getElementById('zonesSearchInput');
  const filter = input.value.trim().toLowerCase();
  const filtered = zones.filter(z =>
    z.long_name.toLowerCase().includes(filter) ||
    z.short_name.toLowerCase().includes(filter)
  );
  renderZonesTable(filtered);
}

document.addEventListener('DOMContentLoaded', function() {
  renderZonesTable(zones);
  const input = document.getElementById('zonesSearchInput');
  if (input) {
    input.addEventListener('input', filterZones);
  }
});
</script>
