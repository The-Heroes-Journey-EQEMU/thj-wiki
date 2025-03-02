---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:42:45.760Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

<style>
  /* Hide the iframe container by default */
  .iframe-container {
    display: none; /* Hidden initially */
    position: relative;
    width: 100%;
    padding-top: 56.25%; /* 16:9 aspect ratio */
    overflow: hidden;
  }

  .responsive-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: none;
  }
</style>

<div id="iframeContainer" class="iframe-container">
  <iframe
    id="scaledIframe"
    class="responsive-iframe"
    src="https://www.thjdi.cc/items"
    onload="fixIframeScaling()"
  ></iframe>
</div>

<script>
  /**
   * Checks the window width and shows/hides the iframe container
   * based on breakpoints: <768px or >1400px.
   */
  function checkScreenSize() {
    const iframeContainer = document.getElementById("iframeContainer");
    const screenWidth = window.innerWidth;

    // Show iframe if width < 768 OR width > 1400
    if (screenWidth < 768 || screenWidth > 1400) {
      iframeContainer.style.display = "block";
    } else {
      iframeContainer.style.display = "none";
    }
  }

  /**
   * Attempts to scale the content inside the iframe.
   * This may fail if the iframe is cross-origin with strict security policies.
   */
  function fixIframeScaling() {
    try {
      const iframe = document.getElementById("scaledIframe");
      const iframeDoc = iframe.contentDocument || iframe.contentWindow.document;
      const iframeBody = iframeDoc.body;

      // Example scaling settings – adjust to taste
      iframeBody.style.transform = "scale(0.9)";
      iframeBody.style.transformOrigin = "top left";
      iframeBody.style.width = "111%"; // Expand slightly to compensate for 0.9 scale
    } catch (error) {
      // Cross-origin restrictions may prevent styling iframe contents
      console.log("Unable to style iframe content:", error);
    }
  }

  // Run checks when the page first loads
  checkScreenSize();

  // Also check whenever the window is resized
  window.addEventListener("resize", checkScreenSize);
</script>



