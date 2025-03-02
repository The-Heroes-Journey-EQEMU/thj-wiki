---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:38:02.531Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

<style>
  /* Default: Hide iframe by default */
  .iframe-container {
    display: none;
  }

  /* Show for screens over 1400px */
  @media (min-width: 1400px) {
    .iframe-container {
      display: block;
      width: 100%;
      height: 80vh; /* Adjusted height for better visibility */
    }

    .responsive-iframe {
      width: 100%;
      height: 100%;
      border: none;
    }
  }

  /* Show for screens under 768px */
  @media (max-width: 768px) {
    .iframe-container {
      display: block;
      width: 100%;
      height: 80vh;
    }

    .responsive-iframe {
      width: 100%;
      height: 100%;
      border: none;
    }
  }
</style>

<div class="iframe-container">
  <iframe 
    id="scaledIframe"
    src="https://www.thjdi.cc/items" 
    class="responsive-iframe" 
    onload="fixIframeScaling()">
  </iframe>
</div>

<script>
  function fixIframeScaling() {
    var iframe = document.getElementById("scaledIframe");

    try {
      var iframeDoc = iframe.contentDocument || iframe.contentWindow.document;
      var iframeBody = iframeDoc.body;

      // Scale down the iframe content to fit inside the container
      iframeBody.style.transform = "scale(0.9)"; /* Adjust this value as needed */
      iframeBody.style.transformOrigin = "top left"; /* Ensures scaling happens from top left */
      iframeBody.style.width = "111%"; /* Expands width slightly to compensate for scaling */
    } catch (error) {
      console.log("Cross-origin restriction prevents direct styling inside the iframe.");
    }
  }
</script>

