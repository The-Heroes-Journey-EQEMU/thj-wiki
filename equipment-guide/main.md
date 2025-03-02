---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:18:13.506Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

<style>
  /* Ensures iframe container takes full width */
  .iframe-container {
    width: 100%;
    max-width: 100%;
  }

  /* Ensures iframe fills the space dynamically */
  .responsive-iframe {
    width: 100%;
    min-height: 1200px; /* Ensures it's not too small */
    border: none;
  }
</style>

<div class="iframe-container">
  <iframe 
    id="dynamicIframe" 
    src="https://www.thjdi.cc/items" 
    class="responsive-iframe" 
    onload="adjustIframe()">
  </iframe>
</div>

<script>
  function adjustIframe() {
    var iframe = document.getElementById("dynamicIframe");

    // Attempt to get iframe content height (only works if same-origin)
    try {
      var newHeight = iframe.contentWindow.document.body.scrollHeight;
      iframe.style.height = newHeight + "px";
    } catch (error) {
      // If blocked by CORS, default to a reasonable height
      iframe.style.height = "1200px";
    }

    // Ensure the form inside the iframe scales properly
    var iframeDoc = iframe.contentDocument || iframe.contentWindow.document;
    if (iframeDoc) {
      var forms = iframeDoc.getElementsByTagName("form");
      for (var i = 0; i < forms.length; i++) {
        forms[i].style.width = "100%"; // Ensures the form inside scales to iframe width
      }
    }
  }

  // Resize on window resize for better responsiveness
  window.addEventListener("resize", adjustIframe);
</script>

