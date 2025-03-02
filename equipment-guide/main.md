---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:40:07.611Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

<style>
  /* Ensure the iframe container is hidden by default */
  .iframe-container {
    display: none; /* Hidden initially */
    width: 100%;
    height: 80vh; /* Adjusted height for better visibility */
  }

  /* Ensure the iframe fills the container */
  .responsive-iframe {
    width: 100%;
    height: 100%;
    border: none;
  }
</style>

<div class="iframe-container" id="iframeWrapper">
  <iframe 
    id="scaledIframe"
    src="https://www.thjdi.cc/items" 
    class="responsive-iframe" 
    onload="fixIframeScaling()">
  </iframe>
</div>

<script>
  function checkScreenSize() {
    var iframeContainer = document.getElementById("iframeWrapper");
    var screenWidth = window.innerWidth;

    // Show iframe only if screen width is >1400px or <768px
    if (screenWidth > 1400 || screenWidth < 768) {
      iframeContainer.style.display = "block"; // Show iframe
    } else {
      iframeContainer.style.display = "none"; // Hide iframe
    }
  }

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

  // Run function on page load
  checkScreenSize();

  // Run function whenever window is resized
  window.addEventListener("resize", checkScreenSize);
</script>


