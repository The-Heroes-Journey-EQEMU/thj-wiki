---
title: Zone Guide
description: Discover how to get from zone A to B.
published: true
date: 2025-03-03T15:39:38.024Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:33:55.088Z
---

<h2>Find Shortest Path Between Zones</h2>
<form id="searchForm">
  <label for="from">From Zone</label>
  <select id="from"></select>

  <label for="to">To Zone</label>
  <select id="to"></select>

  <div>
    <input type="checkbox" id="isBazaarPortalAllowed" checked>
    <label for="isBazaarPortalAllowed">Allow Bazaar Portal?</label>
  </div>

  <button type="submit">Find Path</button>
</form>

<div id="results"></div>

<select id="zones" style="display: none;"></select>

<script>
  let isBazaarAllowed = true;

  class World {
    constructor() {
      this.adjacencyList = {};
      this.fullNames = {};
      this.notes = {};
    }

    addZone(shortName, fullName) {
      if (!this.adjacencyList[shortName]) {
        this.adjacencyList[shortName] = [];
        this.fullNames[shortName] = fullName;
      }
    }

    addZoneLine(source, destination, weight, note = '') {
      this.adjacencyList[source].push({ node: destination, weight, note });
      this.notes[source + destination] = note;
    }

    addBiZoneLine(source, destination, weight, note = '') {
      this.addZoneLine(source, destination, weight, note);
      this.addZoneLine(destination, source, weight, note);
    }

    findShortestPath(start, end) {
      const nodes = new PriorityQueue();
      const distances = {};
      const previous = {};
      let shortestPath = [];
      let smallest;

      for (let node in this.adjacencyList) {
        distances[node] = node === start ? 0 : Infinity;
        nodes.enqueue(node, distances[node]);
        previous[node] = null;
      }

      while (!nodes.isEmpty()) {
        smallest = nodes.dequeue().val;
        if (smallest === end) {
          while (previous[smallest]) {
            shortestPath.push(smallest);
            smallest = previous[smallest];
          }
          break;
        }

        if (smallest || distances[smallest] !== Infinity) {
          for (let neighbor of this.adjacencyList[smallest]) {
            let candidate = distances[smallest] + neighbor.weight;
            if (candidate < distances[neighbor.node]) {
              distances[neighbor.node] = candidate;
              previous[neighbor.node] = smallest;
              nodes.enqueue(neighbor.node, candidate);
            }
          }
        }
      }
      return shortestPath.concat(smallest).reverse();
    }
  }

  class PriorityQueue {
    constructor() {
      this.values = [];
    }
    enqueue(val, priority) {
      this.values.push({ val, priority });
      this.values.sort((a, b) => a.priority - b.priority);
    }
    dequeue() {
      return this.values.shift();
    }
    isEmpty() {
      return this.values.length === 0;
    }
  }

  const w = new World();
  w.addZone("qeynos", "South Qeynos");
  w.addZone("qeynos2", "North Qeynos");
  w.addBiZoneLine('qeynos', 'qeynos2', 2);
  w.addBiZoneLine('qeynos', 'blackburrow', 2);
  
  let searchForm = document.getElementById("searchForm");
  searchForm.addEventListener("submit", (e) => {
    e.preventDefault();
    let from = document.getElementById("from").value;
    let to = document.getElementById("to").value;
    isBazaarAllowed = document.getElementById("isBazaarPortalAllowed").checked;
    if (!from || !to) {
      document.getElementById("results").innerHTML = "Please select both zones.";
      return;
    }
    if (from === to) {
      document.getElementById("results").innerHTML = `You are already in <b>${w.fullNames[from]}</b>!`;
      return;
    }
    let nav = w.findShortestPath(from, to);
    if (!nav.length) {
      document.getElementById("results").innerHTML = `No route found.`;
      return;
    }
    let output = `<b>Route from ${w.fullNames[from]} to ${w.fullNames[to]}:</b><ol>`;
    let src = from;
    for (let i = 1; i < nav.length; i++) {
      output += `<li>${w.fullNames[src]} → ${w.fullNames[nav[i]]}</li>`;
      src = nav[i];
    }
    output += "</ol>";
    document.getElementById("results").innerHTML = output;
  });

  let zonesList = document.getElementById("zones");
  for (let zone in w.fullNames) {
    let option = document.createElement("option");
    option.value = zone;
    option.text = w.fullNames[zone];
    document.getElementById("from").appendChild(option.cloneNode(true));
    document.getElementById("to").appendChild(option);
    zonesList.appendChild(option.cloneNode(true));
  }
</script>
